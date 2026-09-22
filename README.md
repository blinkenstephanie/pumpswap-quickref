# PumpSwap program-id + IDL quickref

Minimal, **dated** reference for Solana builders working with **PumpSwap** (Pump AMM) post-migration flows.

> Always re-verify program IDs and IDL against [official pump-public-docs](https://github.com/pump-fun/pump-public-docs) / on-chain before production use.

**IDL snapshot checked:** 2026-09-22  
**Program (mainnet + devnet per docs):** `pAMMBay6oceH9fJKBRHGP5D4bD4sWpmSwMn52FMfXEA`

## What’s here

- [`PROGRAM_IDS.md`](./PROGRAM_IDS.md) — cluster → program id / GlobalConfig / pool seeds
- [`idl/pumpswap.json`](./idl/pumpswap.json) — IDL snapshot (+ source URL in this README)
- [`examples/decode-ix.md`](./examples/decode-ix.md) — discriminator hygiene notes

## Source

- Docs: https://github.com/pump-fun/pump-public-docs/blob/main/docs/PUMP_SWAP_README.md
- IDL file pulled from pump-public-docs `idl/pump_amm.json` (verify hash against upstream if shipping prod)

## Soft CTA

If you need a **public, self-hosted PumpSwap / Pump.fun launch & trade terminal** (not another opaque hosted stack):

**APEX** — first non-private toolkit offering the public the same class of tools top PumpSwap coin gainers use to launch (now public).  
Free to use; ~3 SOL to download & run locally, or tiny fees to test.

- https://apexlauncher.fun  
- https://github.com/blinkenstephanie/apex-solana-pumpswap-launcher  
- @suntzuson  

## License

MIT
