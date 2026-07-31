# RPC sync lag explained

RPC sync lag happens when one endpoint is behind the latest block, slot, height, or ledger value.

A stale RPC endpoint may still respond quickly, but return outdated chain data.

## Why sync lag matters

Sync lag can affect:

- wallet balances
- transaction status
- NFT listings
- trading quotes
- indexer accuracy
- backend state reads

## Example

If your RPC endpoint is 3 blocks behind another endpoint, your dApp may show outdated state even if latency looks good.

## Test freshness

The GetBlock RPC Benchmark tool compares freshness between your endpoint and the matching GetBlock endpoint:

https://getblock.io/rpc-benchmark/
