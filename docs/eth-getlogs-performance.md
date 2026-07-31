# eth_getLogs performance

`eth_getLogs` is one of the most important and demanding Ethereum JSON-RPC methods.

It is commonly used by:

- data indexers
- analytics tools
- NFT marketplaces
- DeFi dashboards
- event-driven backend services

## Why eth_getLogs can fail

Some RPC endpoints limit or block `eth_getLogs` because log queries can be expensive.

Common issues include:

- timeout errors
- HTTP 429 rate limits
- method restrictions
- slow p95 or p99 latency
- incomplete log support

## How to test it

A safe benchmark should use a small bounded block range and avoid heavy historical scans.

For a live side-by-side benchmark, use:

https://getblock.io/rpc-benchmark/
