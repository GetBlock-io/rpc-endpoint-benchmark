# NFT marketplace RPC benchmark

NFT marketplaces depend on reliable reads, event data, ownership checks, metadata-related flows, and fresh marketplace state.

RPC performance affects how quickly users see listings, ownership updates, collection pages, and transaction status.

## Important signals

For NFT marketplace workloads, check:

- p50 latency
- p95 latency
- p99 latency
- success rate
- timeout rate
- method compatibility
- rate-limit symptoms
- chain freshness

## Important methods

Common NFT-related EVM methods include:

- `eth_blockNumber`
- `eth_call`
- `eth_getLogs`
- `eth_getTransactionReceipt`
- `eth_getBlockByNumber`

## What can go wrong

NFT RPC issues may cause:

- stale ownership data
- delayed listing updates
- slow collection pages
- failed event reads
- missing marketplace activity
- timeout errors during traffic spikes

## Run this benchmark

Select the NFT marketplace profile in the live GetBlock RPC Benchmark:

https://getblock.io/rpc-benchmark/?utm_source=github&utm_medium=referral&utm_campaign=rpc_benchmark_repo&utm_content=nft_marketplace_example
