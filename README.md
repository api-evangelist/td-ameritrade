# TD Ameritrade (td-ameritrade)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
