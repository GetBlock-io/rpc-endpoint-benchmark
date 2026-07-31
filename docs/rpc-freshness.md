# RPC freshness and sync lag

A fast endpoint can still return stale blockchain data.

The benchmark compares the latest available chain value near the end of the run.

Depending on the protocol, this may be:

- block number;
- slot;
- block height;
- ledger value;
- checkpoint or another protocol-specific status value.

Freshness matters for:

- balances;
- transaction status;
- market data;
- NFT state;
- indexer accuracy;
- application state reads.

Run a live freshness comparison:

https://getblock.io/rpc-benchmark/
