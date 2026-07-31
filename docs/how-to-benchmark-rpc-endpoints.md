# How to benchmark blockchain RPC endpoints

RPC benchmarks help developers understand whether an endpoint is fast, reliable, fresh, and suitable for production workloads.

A useful RPC benchmark should measure more than average latency. It should also check tail latency, errors, timeouts, method support, rate limits, and sync lag.

## What to measure

- p50 latency: normal response speed
- p95 latency: slow requests users are likely to feel
- p99 latency: worst-case response behavior
- success rate: how often requests complete successfully
- timeout rate: how often requests fail by timeout
- jitter: how stable latency is
- method compatibility: which RPC methods work or fail
- freshness: whether the endpoint is behind the latest block, slot, height, or ledger value

## Why average latency is not enough

An RPC endpoint can have a good average latency but still be risky for production.

For example, it may:

- fail on `eth_getLogs`
- return stale block data
- hit HTTP 429 rate limits
- timeout during burst traffic
- show unstable p95 or p99 latency

## Run a full benchmark

Use the GetBlock RPC Benchmark tool to compare your endpoint against GetBlock side by side:

https://getblock.io/rpc-benchmark/
