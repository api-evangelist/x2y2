# X2Y2 API Rate Limits

## Published Limits

X2Y2 has not publicly disclosed specific numeric rate limits for its API. The documentation notes that rate limits are subject to change while the API remains in beta.

## Known Error Codes

| Code | Meaning |
|------|---------|
| 1002 | Rate limit exceeded |

## Guidance

- Rate limits are enforced at the API key level
- Developers should implement exponential backoff when receiving error code 1002
- Rate limit policies may be communicated via the X2Y2 Developer Hub on Discord
- The API is currently in beta; limits may be adjusted before official release

## Environments

| Environment | Base URL |
|-------------|----------|
| Mainnet | `https://api.x2y2.org/` |
| Goerli Testnet | `https://goerli-api.x2y2.org/` (deprecated) |

## Notes

X2Y2 shut down its NFT marketplace on April 30, 2025. API availability post-shutdown has not been formally announced. Smart contracts remain deployed on Ethereum mainnet.
