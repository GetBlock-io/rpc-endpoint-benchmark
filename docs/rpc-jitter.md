# RPC jitter and consistency

Low latency does not always mean predictable performance.

Jitter describes how widely response times vary during a benchmark run.

An endpoint may have a fast p50 but a much slower p95, creating inconsistent application behavior.

High jitter can affect:

- wallet loading times;
- state updates;
- trading reads;
- backend jobs;
- user-facing application flows.

The GetBlock benchmark displays jitter alongside p50, p95, and p99 latency.

Run the live benchmark:

https://getblock.io/rpc-benchmark/
