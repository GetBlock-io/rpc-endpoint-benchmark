# p95 vs p99 RPC latency

Average latency does not show the full RPC performance picture.

For production dApps, p95 and p99 latency are often more useful because they show the slow requests users actually feel.

## p50 latency

p50 is the median response time. It shows what a normal request looks like.

## p95 latency

p95 means that 95% of successful requests were faster than this value.

High p95 latency can create slow wallet loading, delayed state updates, and inconsistent dApp UX.

## p99 latency

p99 shows the worst tail latency.

For DEX, trading, GameFi, and high-frequency backend workloads, p99 can be more important than average latency.

## Test your RPC endpoint

Run a live benchmark:

https://getblock.io/rpc-benchmark/
