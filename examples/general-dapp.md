# General dApp RPC benchmark

General dApps need a balanced RPC endpoint that is fast, reliable, fresh, and compatible with common read methods.

This profile is useful when a project does not fit one specific workload category such as wallet, indexer, DEX, or NFT marketplace.

## Important signals

For general dApp workloads, check:

- p50 latency
- p95 latency
- p99 latency
- success rate
- error rate
- timeout rate
- jitter
- method compatibility
- chain freshness

## Important methods

Common general dApp EVM methods include:

- `eth_chainId`
- `eth_blockNumber`
- `eth_getBlockByNumber`
- `eth_getBalance`
- `eth_call`

## What can go wrong

General RPC issues may cause:

- slow page loading
- failed state reads
- stale UI data
- inconsistent user experience
- timeout errors
- backend retries

## Run this benchmark

Select the General dApp profile in the live GetBlock RPC Benchmark:

https://getblock.io/rpc-benchmark/?utm_source=github&utm_medium=referral&utm_campaign=rpc_benchmark_repo&utm_content=general_dapp_example
