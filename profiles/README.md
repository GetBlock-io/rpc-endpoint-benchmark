# RPC workload profiles

Workload profiles change the method mix used by the benchmark.

The same generated profile is always sent to both endpoints.

## Available profiles

### General dApp

Balanced read-only traffic for common frontend and backend applications.

### Wallet / portfolio app

Prioritizes balances, latest state, and lightweight account or contract reads.

### Data indexer / analytics

Emphasizes block-heavy, log-heavy, and method-compatibility checks.

### DEX / trading bot

Prioritizes fresh state and tail-latency-sensitive reads.

### NFT marketplace

Focuses on contract reads, logs, collection state, and consistency.

## Live benchmark

Select a profile and run the comparison:

https://getblock.io/rpc-benchmark/
