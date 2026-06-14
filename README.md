# X2Y2

X2Y2 was an NFT marketplace and trading platform on Ethereum offering one of the lowest marketplace fees (0.5%) in the industry. It provided REST APIs and a JavaScript SDK enabling developers to build analytics tools, trading bots, and web3 applications on top of its marketplace infrastructure.

## API

The X2Y2 API is organized into two suites:

**X2Y2 OpenAPI** — marketplace data and order management:
- `GET /v1/orders` — fetch open listings/orders
- `POST /v1/orders` — create a new order/listing
- `GET /v1/events` — fetch marketplace events (sales, transfers)
- `GET /v1/offers` — fetch open offers
- `GET /v1/contracts/{contract}` — fetch collection/contract info
- `GET /v1/contracts/{contract}/stats` — fetch collection statistics

**X2Y2 Fi API** — NFT-backed lending and finance:
- `GET /system/option` — get system parameters
- Loan creation, repayment, and refinancing endpoints
- Offer creation and management endpoints

## Authentication

All endpoints require an API key. Keys are requested through the X2Y2 Developer Hub (Discord). The API was in beta with no published rate limit thresholds; error code `1002` indicates rate limit exceeded.

## Base URLs

- Mainnet: `https://api.x2y2.org/`
- Goerli Testnet: `https://goerli-api.x2y2.org/` (deprecated)

## SDK

- npm: `@x2y2-io/sdk`
- GitHub: [X2Y2-io/x2y2-sdk](https://github.com/X2Y2-io/x2y2-sdk)

## Status

X2Y2 shut down its NFT marketplace on April 30, 2025. Ethereum smart contracts remain deployed and operational.

## Links

- Developer Docs: https://docs.x2y2.io/developers/api
- API Reference: https://x2y2.readme.io/reference/introduction
- GitHub: https://github.com/X2Y2-io
