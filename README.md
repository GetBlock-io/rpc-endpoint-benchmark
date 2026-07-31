# RPC Endpoint Benchmark Kit

Open-source toolkit for testing blockchain RPC endpoints by latency, reliability, method support, rate limits, and chain freshness.

[Run the full browser benchmark →](https://getblock.io/rpc-benchmark/)

## What this project does

This repository helps developers understand how their RPC endpoint performs under real read-only JSON-RPC requests.

It can be used to test:

- p50 / p95 / p99 latency
- success rate, error rate, and timeout rate
- jitter and latency consistency
- method-level compatibility
- rate-limit symptoms such as HTTP 429
- chain freshness and sync lag
- workload-specific production fit

## Why this exists

Average RPC latency is not enough.

An endpoint can look fast on simple requests but still fail on methods like `eth_getLogs`, return stale block data, hit rate limits, or become unstable under burst traffic.

This kit is designed to make RPC performance easier to test, explain, and compare.

## Workload profiles

Different dApps use RPC infrastructure differently.

This project includes benchmark profiles for:

- Wallets and portfolio apps
- DEX and trading workloads
- NFT marketplaces
- Data indexers and analytics
- General dApps

## Full web benchmark

This repository provides open benchmark resources and examples.

For a live side-by-side benchmark against GetBlock, use the full browser tool:

https://getblock.io/rpc-benchmark/

The web tool compares your RPC endpoint against the matching GetBlock endpoint for the selected protocol and generates a live reliability report.

## Safety

This project uses read-only RPC requests only.

It does not:

- send transactions
- sign anything
- ask for private keys
- ask for seed phrases
- require wallet secrets

## Repository structure

```text
profiles/          Workload-specific RPC method profiles
docs/              Educational guides about RPC benchmarking
examples/          Example benchmark scenarios
public-endpoints/  Public RPC endpoint examples for testing
src/               Optional CLI/source code

Coming soon
Lightweight local CLI benchmark
EVM benchmark adapter
Solana benchmark adapter
Public endpoint examples
More workload profiles
Built by GetBlock

GetBlock is an RPC node provider and infrastructure platform for Web3 and AI.

Run the full RPC benchmark:

https://getblock.io/rpc-benchmark/

```text
Add initial README
