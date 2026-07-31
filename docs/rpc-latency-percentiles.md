# RPC latency percentiles

RPC latency should be evaluated as a distribution, not as one average value.

## p50

p50 is the median successful response time. It describes a typical request.

## p95

p95 shows the response time below which 95% of successful requests completed.

It highlights tail latency that users may experience regularly.

## p99

p99 represents slower edge cases and is particularly important for latency-sensitive applications.

Examples include:

- trading bots;
- DEX interfaces;
- real-time wallet updates;
- interactive GameFi applications.

## Compare your endpoint

Run a paired p50, p95, and p99 comparison:

https://getblock.io/rpc-benchmark/
