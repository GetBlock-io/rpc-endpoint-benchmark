# RPC rate limits and HTTP 429

HTTP 429 indicates that an endpoint is throttling requests.

Rate limiting can appear because of:

- public endpoint restrictions;
- provider plan limits;
- temporary overload;
- per-IP limits;
- burst traffic;
- method-specific restrictions.

The benchmark records HTTP errors and identifies rate-limit-like behavior in its findings.

Run a reliability benchmark:

https://getblock.io/rpc-benchmark/
