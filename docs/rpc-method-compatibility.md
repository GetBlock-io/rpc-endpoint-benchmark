# Method-level RPC compatibility

Method-level compatibility shows whether an RPC endpoint supports the methods your dApp actually needs.

An endpoint can respond successfully to simple methods but fail on heavier or restricted methods.

## Why method compatibility matters

Different applications depend on different RPC methods.

For example:

- wallets need balance and state reads
- indexers need block and log access
- DEX apps need fast `eth_call` responses
- NFT marketplaces may need logs, token data, and metadata-related reads
- backend services need predictable method behavior

## Common method issues

RPC method problems may include:

- method not found
- restricted method access
- timeout errors
- rate limits
- slow p95 or p99 latency
- inconsistent responses
- incomplete historical support

## EVM examples

Common EVM methods include:

- `eth_chainId`
- `eth_blockNumber`
- `eth_getBlockByNumber`
- `eth_getBalance`
- `eth_call`
- `eth_getLogs`

## Run a live benchmark

Check method-level performance with the GetBlock RPC Benchmark:

https://getblock.io/rpc-benchmark/?utm_source=github&utm_medium=referral&utm_campaign=rpc_benchmark_repo&utm_content=method_compatibility
