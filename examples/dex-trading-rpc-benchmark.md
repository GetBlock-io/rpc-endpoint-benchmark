# DEX and trading RPC benchmark

DEX apps and trading bots depend on low-latency reads, fresh state, and predictable RPC behavior.

For trading workloads, slow or stale RPC responses can affect quotes, routing, execution timing, and risk checks.

## Important signals

For DEX and trading workloads, check:

- p50 latency
- p95 latency
- p99 latency
- jitter
- latest block freshness
- timeout rate
- method-level latency
- small burst behavior

## Important methods

Common trading-related EVM methods include:

- `eth_blockNumber`
- `eth_call`
- `eth_getBalance`
- `eth_getBlockByNumber`
- `eth_getTransactionReceipt`

## What can go wrong

Trading RPC issues may cause:

- stale quotes
- slow route calculations
- delayed price reads
- missed block updates
- timeout spikes
- unreliable backend decisions

## Run this benchmark

Select the DEX / trading profile in the live GetBlock RPC Benchmark:

https://getblock.io/rpc-benchmark/?utm_source=github&utm_medium=referral&utm_campaign=rpc_benchmark_repo&utm_content=dex_trading_example
