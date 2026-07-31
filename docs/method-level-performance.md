# Method-level RPC performance

An RPC endpoint can perform well on lightweight methods and poorly on heavier methods.

Method-level benchmarking helps identify the exact bottleneck.

Examples include:

- `eth_blockNumber`;
- `eth_getBalance`;
- `eth_call`;
- `eth_getBlockByNumber`;
- `eth_getLogs`;
- `getSlot`;
- `getLatestBlockhash`.

The live report compares latency, errors, and compatibility for each tested method.

Run a method-level comparison:

https://getblock.io/rpc-benchmark/
