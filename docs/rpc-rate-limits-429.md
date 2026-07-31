# RPC rate limits and HTTP 429

HTTP 429 means an RPC endpoint is throttling requests.

This often happens with public RPC endpoints, free plans, or overloaded infrastructure.

## Why rate limits matter

Rate limits can cause:

- failed wallet requests
- delayed dApp updates
- broken indexer jobs
- failed backend workflows
- unstable user experience during traffic spikes

## What to check

A benchmark should detect:

- HTTP 429 responses
- timeout spikes
- method-specific failures
- burst traffic degradation

## Test rate-limit symptoms

Run a live RPC benchmark:

https://getblock.io/rpc-benchmark/
