# Understanding p50, p95, and p99 RPC latency

RPC latency shows how long it takes an endpoint to respond to a request.

Average latency is useful, but it does not show the full picture. For production dApps, percentile latency is usually more helpful.

## p50 latency

p50 is the median response time.

It shows what a normal request usually feels like.

## p95 latency

p95 means that 95% of successful requests were faster than this value.

High p95 latency can create visible delays in wallets, dashboards, trading interfaces, NFT pages, and backend data flows.

## p99 latency

p99 shows tail latency.

It helps reveal the slowest requests that may affect real users or production jobs.

For latency-sensitive workloads like DEX apps, trading bots, GameFi apps, and indexers, p99 can matter more than average latency.

## What to check

When comparing RPC endpoints, check:

- p50 for normal performance
- p95 for user-visible slowdowns
- p99 for worst-case behavior
- timeout rate for failed requests
- jitter for consistency

## Run a live benchmark

Compare p50, p95, and p99 latency against GetBlock:

https://getblock.io/rpc-benchmark/?utm_source=github&utm_medium=referral&utm_campaign=rpc_benchmark_repo&utm_content=latency_percentiles
