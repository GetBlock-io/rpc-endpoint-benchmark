# Indexer RPC benchmark

Data indexers and analytics platforms depend on reliable block, transaction, and log access.

Indexer workloads are often more demanding than simple wallet reads because they need consistent historical and event data.

## Important signals

For indexer workloads, check:

- `eth_getLogs` compatibility
- block-read latency
- p95 latency
- p99 latency
- timeout rate
- error rate
- rate-limit symptoms
- chain freshness

## Important methods

Common indexer-related EVM methods include:

- `eth_blockNumber`
- `eth_getBlockByNumber`
- `eth_getLogs`
- `eth_getTransactionReceipt`
- `eth_call`

## What can go wrong

Indexer RPC issues may cause:

- missing events
- delayed indexing jobs
- incomplete analytics data
- failed historical scans
- backend retry loops
- HTTP 429 rate limits

## Run this benchmark

Select the Data indexer / analytics profile in the live GetBlock RPC Benchmark:

https://getblock.io/rpc-benchmark/?utm_source=github&utm_medium=referral&utm_campaign=rpc_benchmark_repo&utm_content=indexer_example
