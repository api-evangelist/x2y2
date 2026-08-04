# X2Y2

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
