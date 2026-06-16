# TD Ameritrade (td-ameritrade)

TD Ameritrade was a US retail brokerage that provided REST APIs for trading equities and options, accessing streaming market data, managing brokerage accounts, and retrieving historical and real-time market data. Following the Charles Schwab acquisition, the TD Ameritrade API was shut down on May 10, 2024. Schwab has ported much of the original functionality into the Schwab Trader API.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/apis.yml)

## Tags

- Brokerage
- Trading
- Finance
- Equities
- Options
- Market Data
- Streaming

## Timestamps

- **Created:** 2024-01-01
- **Modified:** 2026-06-13

## APIs

### TD Ameritrade Accounts and Trading API

Provides REST endpoints for managing TD Ameritrade brokerage accounts, including retrieving account balances, positions, and transaction history. Supports placing, modifying, replacing, and canceling orders for equities and options. Also includes saved orders, watchlists, and user preferences.

- **Human URL:** [https://developer.tdameritrade.com/account-access/apis](https://developer.tdameritrade.com/account-access/apis)
- **Base URL:** `https://api.tdameritrade.com/v1`

#### Tags

- Accounts
- Orders
- Trading
- Watchlists
- Transactions

#### Properties

- [Documentation](https://developer.tdameritrade.com/account-access/apis)
- [OpenAPI](https://developer.tdameritrade.com/account-access/apis) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Authentication](https://developer.tdameritrade.com/authentication/apis)
- [Graph Q L](graphql/td-ameritrade-graphql.md)

### TD Ameritrade Market Data API

Provides REST endpoints for accessing real-time and historical market data. Includes current quotes for single and multiple symbols, historical price history for equities and ETFs, options chains with full contract details, top movers by index, and market hours for equities, options, futures, forex, and bond markets.

- **Human URL:** [https://developer.tdameritrade.com/market-data/apis](https://developer.tdameritrade.com/market-data/apis)
- **Base URL:** `https://api.tdameritrade.com/v1`

#### Tags

- Market Data
- Quotes
- Options Chains
- Price History
- Movers
- Market Hours

#### Properties

- [Documentation](https://developer.tdameritrade.com/market-data/apis)
- [Authentication](https://developer.tdameritrade.com/authentication/apis)

### TD Ameritrade Instruments API

Provides REST endpoints for searching and retrieving instrument details by symbol or CUSIP. Supports searching by symbol or description and retrieving fundamental data including financial ratios, earnings, and dividend information for equities.

- **Human URL:** [https://developer.tdameritrade.com/instruments/apis](https://developer.tdameritrade.com/instruments/apis)
- **Base URL:** `https://api.tdameritrade.com/v1`

#### Tags

- Instruments
- Equities
- Fundamentals
- Securities

#### Properties

- [Documentation](https://developer.tdameritrade.com/instruments/apis)
- [Authentication](https://developer.tdameritrade.com/authentication/apis)

### TD Ameritrade Authentication API

Implements OAuth 2.0 token-based authentication as described in RFC6749 section 1.3.1. Applications registered on the TD Ameritrade Developer Portal receive a Consumer Key (client_id). Access tokens are valid for 30 minutes; refresh tokens are valid for 90 days and may be used to generate new access and refresh tokens.

- **Human URL:** [https://developer.tdameritrade.com/authentication/apis](https://developer.tdameritrade.com/authentication/apis)
- **Base URL:** `https://api.tdameritrade.com/v1`

#### Tags

- Authentication
- OAuth 2.0
- Access Tokens

#### Properties

- [Documentation](https://developer.tdameritrade.com/authentication/apis)
- [Getting Started](https://developer.tdameritrade.com/content/getting-started)
- [Authentication F A Q](https://developer.tdameritrade.com/content/authentication-faq)

### TD Ameritrade Streaming Market Data API

Provides a WebSocket-based streaming API that delivers up-to-the-second market data including real-time Level 1 and Level 2 quotes, time and sales data for equities, options, and futures, as well as order book depth data. Streaming sessions are initiated using credentials obtained from the User Principals endpoint.

- **Human URL:** [https://developer.tdameritrade.com/content/streaming-data](https://developer.tdameritrade.com/content/streaming-data)
- **Base URL:** `wss://streamer-ws.tdameritrade.com/ws`

#### Tags

- Streaming
- WebSocket
- Real-Time
- Level 2
- Market Data

#### Properties

- [Documentation](https://developer.tdameritrade.com/content/streaming-data)
- [Authentication](https://developer.tdameritrade.com/authentication/apis)

## Common Properties

- [Portal](https://developer.tdameritrade.com/)
- [Getting Started](https://developer.tdameritrade.com/content/getting-started)
- [Documentation](https://developer.tdameritrade.com/apis)
- [Authentication](https://developer.tdameritrade.com/authentication/apis)
- [Authentication F A Q](https://developer.tdameritrade.com/content/authentication-faq)
- [Plans](https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/plans/plans.yml)
- [Rate Limits](https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/rate-limits/rate-limits.yml)
- [Fin Ops](https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/finops/finops.yml)
- [Terms of Service](https://developer.tdameritrade.com/content/td-ameritrade-api-terms-use)
- [Status Page](https://developer.tdameritrade.com/content/getting-started)
- [Deprecation Notice](https://blog.pickmytrade.trade/td-ameritrade-have-api-2025/)
- [Migration Guide](https://developer.schwab.com/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
**URL:** https://www.apievangelist.com
