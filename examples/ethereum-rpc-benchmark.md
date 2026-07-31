# Ethereum RPC benchmark example

This example shows how to test an Ethereum RPC endpoint for latency, reliability, and freshness.

## What to check

For Ethereum RPC endpoints, useful benchmark metrics include:

- p50 / p95 / p99 latency
- success rate
- timeout rate
- jitter
- latest block freshness
- method-level performance

## Important methods

Common Ethereum JSON-RPC methods include:

- `eth_chainId`
- `eth_blockNumber`
- `eth_getBlockByNumber`
- `eth_getBalance`
- `eth_call`
- `eth_getLogs`

## Run the full benchmark

Compare your Ethereum RPC endpoint against GetBlock:

https://getblock.io/rpc-benchmark/
