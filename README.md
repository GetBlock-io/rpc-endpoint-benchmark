# RPC Endpoint Benchmark

Developer resources and benchmark profiles for testing blockchain RPC endpoint speed, reliability, method compatibility, rate limits, and chain freshness.

[**Run the live RPC benchmark →**](https://getblock.io/rpc-benchmark/?utm_source=github&utm_medium=referral&utm_campaign=rpc_benchmark_repo&utm_content=readme_hero)

![GetBlock RPC Benchmark preview](assets/rpc-benchmark-preview.png)

## What is the RPC Benchmark?

The GetBlock RPC Benchmark runs a live, side-by-side comparison between your current RPC endpoint and the matching GetBlock endpoint for the selected protocol.

Both endpoints receive the same bounded sequence of read-only RPC requests from the same benchmark server.

The tool helps developers understand not only which endpoint is faster, but which one looks more reliable and production-ready for their workload.

## What it measures

* p50, p95, and p99 latency
* Success, error, and timeout rates
* Latency jitter and consistency
* Method-level compatibility
* HTTP 429 and rate-limit symptoms
* Latest block, slot, height, or ledger freshness
* Sync lag and stale-node risk
* Workload-specific production fit

## Workload profiles

The benchmark adapts its RPC method mix to the type of application being tested:

* General dApp
* Wallet or portfolio app
* Data indexer or analytics platform
* DEX or trading bot
* NFT marketplace

## Supported protocols

The live benchmark supports 100+ blockchain protocol and network options, including:

* Ethereum
* BNB Smart Chain
* Polygon
* Solana
* Bitcoin
* Arbitrum
* Base
* Tron
* Avalanche
* Optimism
* Starknet
* Sui
* TON
* Polkadot
* Cosmos
* and many more

[**View and run the supported protocols →**](https://getblock.io/rpc-benchmark/?utm_source=github&utm_medium=referral&utm_campaign=rpc_benchmark_repo&utm_content=supported_protocols)

## Fair comparison methodology

The benchmark uses paired side-by-side testing:

* Same protocol and network
* Same workload profile
* Same read-only RPC methods
* Same request sequence
* Same timeout
* Same benchmark duration
* Same benchmark server
* Same measurement window

The benchmark never sends transactions, signs messages, or asks for private keys, seed phrases, or wallet secrets.

[Read the full benchmark methodology](https://getblock.io/rpc-benchmark/methodology/?utm_source=github&utm_medium=referral&utm_campaign=rpc_benchmark_repo&utm_content=methodology)

## Start here

* [How to benchmark RPC endpoints](docs/how-to-benchmark-rpc-endpoints.md)
* [Understanding p50, p95, and p99 latency](docs/p50-p95-p99-rpc-latency.md)
* [RPC jitter and latency consistency](docs/rpc-jitter-and-consistency.md)
* [RPC rate limits and HTTP 429](docs/rpc-rate-limits-and-429.md)
* [RPC freshness and sync lag](docs/rpc-freshness-and-sync-lag.md)
* [Method-level RPC compatibility](docs/rpc-method-compatibility.md)

## Workload examples

* [Wallet RPC benchmark](examples/wallet-rpc-benchmark.md)
* [Indexer RPC benchmark](examples/indexer-rpc-benchmark.md)
* [DEX and trading RPC benchmark](examples/dex-trading-rpc-benchmark.md)
* [NFT marketplace RPC benchmark](examples/nft-marketplace-rpc-benchmark.md)
* [General dApp RPC benchmark](examples/general-dapp-rpc-benchmark.md)

## Run the live benchmark

Use the browser tool to compare your RPC endpoint against GetBlock with live performance cards, latency charts, method-level results, freshness checks, actionable findings, and a downloadable report.

[**Run the free RPC benchmark →**](https://getblock.io/rpc-benchmark/?utm_source=github&utm_medium=referral&utm_campaign=rpc_benchmark_repo&utm_content=readme_bottom)

No signup is required to run the benchmark.

## Important limitations

The benchmark is a short, point-in-time comparison, not an SLA or a full production load test.

Results may vary depending on:

* Benchmark server region
* Provider routing
* RPC plan
* Rate limits
* Cache state
* Current node load
* Blockchain network conditions
* Selected workload profile

## Built by GetBlock

GetBlock provides RPC infrastructure and blockchain APIs across 100+ networks.

[Get started with GetBlock](https://getblock.io/?utm_source=github&utm_medium=referral&utm_campaign=rpc_benchmark_repo)
