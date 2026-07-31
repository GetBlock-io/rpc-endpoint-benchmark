# Wallet RPC benchmark

Wallet and portfolio apps depend on fresh balances, reliable reads, and stable latency.

A wallet RPC endpoint should respond quickly and consistently to common account and state requests.

## Important signals

For wallet workloads, check:

- p50 latency
- p95 latency
- p99 latency
- success rate
- timeout rate
- latest block freshness
- method-level compatibility

## Important methods

Common wallet-related EVM methods include:

- `eth_chainId`
- `eth_blockNumber`
- `eth_getBalance`
- `eth_call`
- `eth_getTransactionReceipt`

## What can go wrong

Wallet users may experience:

- slow balance loading
- stale portfolio data
- delayed transaction status
- failed token reads
- inconsistent app state

## Run this benchmark

Select the Wallet profile in the live GetBlock RPC Benchmark:

https://getblock.io/rpc-benchmark/?utm_source=github&utm_medium=referral&utm_campaign=rpc_benchmark_repo&utm_content=wallet_example
