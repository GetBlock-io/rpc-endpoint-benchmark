# How RPC endpoint benchmarking works

The GetBlock RPC Benchmark uses paired side-by-side testing.

For every benchmark run, the user endpoint and the matching GetBlock endpoint receive:

- the same read-only RPC methods;
- the same generated request sequence;
- the same parameters;
- the same timeout;
- the same benchmark duration;
- requests from the same benchmark server.

This prevents different method mixes or measurement locations from skewing the comparison.

## Server-side measurement

Latency is measured by the backend server running the benchmark, not by the visitor's browser.

The result represents endpoint behavior from that benchmark location during that specific run.

## Point-in-time result

A short benchmark is not an SLA or a full production load test.

Results can change because of:

- provider routing;
- benchmark region;
- cache state;
- provider plan;
- current infrastructure load;
- rate limits;
- node health.

## Safety

The benchmark uses read-only requests only.

It never sends transactions, signs data, or requires wallet secrets.

## Complete methodology

Read the full methodology:

https://getblock.io/rpc-benchmark/methodology/
