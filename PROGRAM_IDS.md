# Program IDs

**Checked:** 2026-09-22  
**Source:** [pump-fun/pump-public-docs — PumpSwap README](https://github.com/pump-fun/pump-public-docs/blob/main/docs/PUMP_SWAP_README.md)

> Always re-verify on-chain / against official docs before production. IDs and IDL can change.

## Mainnet-beta & Devnet (same address per official docs)

| Item | Address |
|------|---------|
| **PumpSwap (Pump AMM) program** | `pAMMBay6oceH9fJKBRHGP5D4bD4sWpmSwMn52FMfXEA` |
| **GlobalConfig PDA** (`["global_config"]`) | `ADyA8hdefvWN2dbGGWFotbzWxrAvLW83WG6QCVXvJKqw` |

Explorer:
- Mainnet: https://solscan.io/account/pAMMBay6oceH9fJKBRHGP5D4bD4sWpmSwMn52FMfXEA
- Devnet: https://solscan.io/account/pAMMBay6oceH9fJKBRHGP5D4bD4sWpmSwMn52FMfXEA?cluster=devnet

## Pool PDA seeds (from docs)

Pools are PDA-derived from:

```text
["pool", index, creator, baseMint, quoteMint]
```

Canonical pools typically use `index = 0`. Non-canonical indexes have different creator-fee implications — read official docs before assuming fee routing.

## Fees (GlobalConfig snapshot from docs — re-check live)

- `lp_fee_basis_points`: 20 bps
- `protocol_fee_basis_points`: 5 bps
- Protocol fee recipients: 8 pubkeys in GlobalConfig; rotate randomly for throughput

## Related (not PumpSwap AMM)

Do **not** confuse with Pump.fun bonding-curve program IDs. Migration bots that hardcode the wrong program silently miss events.
