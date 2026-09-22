# Matching PumpSwap instruction discriminators

1. Load `idl/pumpswap.json` (snapshot dated in README).
2. For each instruction in the IDL, take the 8-byte Anchor discriminator.
3. When decoding a tx, assert the first 8 bytes of instruction data match before deserializing the rest.
4. For migration / pool events, reject payloads that fail the discriminator check (silent wrong decode is worse than a hard fail).

Never trust a random GitHub constant named `PUMPSWAP_PROGRAM_ID` without comparing to:

`pAMMBay6oceH9fJKBRHGP5D4bD4sWpmSwMn52FMfXEA`
