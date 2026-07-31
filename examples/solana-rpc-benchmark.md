# Solana RPC benchmark example

This example shows how to test a Solana RPC endpoint for latency, reliability, and slot freshness.

## What to check

For Solana RPC endpoints, useful benchmark metrics include:

- p50 / p95 / p99 latency
- success rate
- timeout rate
- jitter
- latest slot freshness
- method-level performance

## Important methods

Common Solana RPC methods include:

- `getHealth`
- `getSlot`
- `getLatestBlockhash`
- `getBalance`

## Run the full benchmark

Compare your Solana RPC endpoint against GetBlock:

https://getblock.io/rpc-benchmark/
