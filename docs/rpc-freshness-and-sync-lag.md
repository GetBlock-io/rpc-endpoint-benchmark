# RPC freshness and sync lag

RPC freshness shows whether an endpoint is up to date with the latest chain state.

An RPC endpoint can respond quickly but still return stale data.

## What is sync lag?

Sync lag happens when one endpoint is behind the latest block, slot, height, or ledger value.

For example, if one Ethereum RPC endpoint returns block `20500000` while another returns `20500003`, the first endpoint may be 3 blocks behind.

## Why freshness matters

Stale RPC data can affect:

- wallet balances
- transaction status
- DEX quotes
- NFT listings
- indexer accuracy
- backend state reads
- user-facing dashboards

## Latency is not enough

A fast stale endpoint is still risky.

For production dApps, freshness should be checked together with latency, errors, timeouts, and method compatibility.

## Run a live benchmark

Compare endpoint freshness against GetBlock:

https://getblock.io/rpc-benchmark/?utm_source=github&utm_medium=referral&utm_campaign=rpc_benchmark_repo&utm_content=freshness_sync_lag
