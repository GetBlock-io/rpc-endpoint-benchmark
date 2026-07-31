# RPC jitter and latency consistency

RPC jitter shows how much latency varies between requests.

A low-latency endpoint is not always stable. Two endpoints may have similar average latency, but one may respond consistently while another has frequent spikes.

## Why jitter matters

High jitter can cause:

- inconsistent wallet loading
- delayed UI updates
- unstable trading workflows
- backend retry spikes
- poor user experience during traffic bursts

## Example

An RPC endpoint with 80 ms average latency but frequent 800 ms spikes may feel worse than an endpoint with 120 ms average latency and stable responses.

Consistency matters because users and backend systems feel the slow requests, not just the average.

## What to check

When testing RPC jitter, look at:

- latency spread
- p95 latency
- p99 latency
- timeout rate
- method-level latency spikes
- behavior under small bursts

## Run a live benchmark

Compare RPC latency consistency against GetBlock:

https://getblock.io/rpc-benchmark/?utm_source=github&utm_medium=referral&utm_campaign=rpc_benchmark_repo&utm_content=jitter_consistency
