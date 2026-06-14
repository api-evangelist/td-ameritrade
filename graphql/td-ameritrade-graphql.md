# TD Ameritrade GraphQL Schema

TD Ameritrade was a major US retail brokerage that provided REST APIs for trading equities and options, accessing streaming market data, managing brokerage accounts, and retrieving historical and real-time market data. Following the Charles Schwab acquisition, the TD Ameritrade API was shut down on May 10, 2024. Schwab has ported much of the original functionality into the Schwab Trader API.

This conceptual GraphQL schema models the core domain objects and relationships exposed by the TD Ameritrade REST API suite, covering accounts, orders, market data, instruments, options chains, streaming sessions, and user preferences. It is intended as a reference for teams migrating to the Schwab Trader API or building GraphQL federation layers over brokerage APIs.

## Coverage

The schema covers five primary API surface areas:

- **Accounts and Trading** — account balances, positions, transactions, orders, saved orders, and watchlists
- **Market Data** — real-time quotes, historical price history, options chains, market movers, and market hours
- **Instruments** — symbol search, CUSIP lookup, and fundamental financial data
- **Authentication** — OAuth 2.0 token management and user principal information
- **Streaming** — WebSocket session credentials and subscription management concepts

## Key Design Decisions

- `Account` is an interface implemented by `MarginAccount` and `CashAccount`, reflecting the two account types supported by the TD Ameritrade API.
- Orders use a union type (`PlacedOrder | FilledOrder | CancelledOrder`) to represent the order lifecycle without overloading a single type with nullable fields.
- `OptionChain` aggregates `ExpirationDate` and `OptionData` in a nested structure that mirrors the original REST response shape.
- `UserPrincipals` holds the streaming credentials (`StreamingToken`) needed to initiate WebSocket sessions.
- Enums are used throughout to enforce valid values for order types, asset types, transaction types, and market session identifiers.

## Source

- Developer portal: https://developer.tdameritrade.com/
- Successor platform: https://developer.schwab.com/
- GitHub: https://github.com/td-ameritrade
