# X2Y2 API FinOps

## Cost Structure

X2Y2 did not publish a paid API pricing model. The API was available free of charge to approved developers during its beta period.

## Platform Fees (Marketplace)

While the API itself was free, transactions executed through the X2Y2 marketplace incurred platform fees:

- **Marketplace fee**: 0.5% per sale (one of the lowest in the NFT industry)
- **Royalty fees**: Variable, configurable per collection; obtainable via `GET /v1/contracts/{contract}`

## FinOps Considerations

| Item | Detail |
|------|--------|
| API Access Cost | Free (key required via Discord) |
| Transaction Gas | Ethereum mainnet gas fees apply to on-chain operations |
| Smart Contract Interactions | Gas costs for buy, sell, cancel, offer accept operations |
| SDK | Open source, no licensing fee (`@x2y2-io/sdk` on npm) |

## Shutdown Notice

X2Y2 ceased marketplace operations on April 30, 2025. Any ongoing cost considerations are limited to direct smart contract interactions on Ethereum, which carry standard gas fees. No API billing is expected post-shutdown.
