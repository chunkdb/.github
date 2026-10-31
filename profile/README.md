# chunkdb

chunkdb 2.0 stores grid data in tables of chunks of typed blocks.
CQL reads and writes blocks, transfers chunks and streams committed changes over TCP or TLS.
Users control access per table; transactions commit several chunks of one table together, and backup copies a running server for offline restore.

## Start

Follow the [quick start](https://github.com/chunkdb/chunkdb/blob/main/docs/QUICK_START.md) to run the server, write blocks and watch an update.

## Repositories

- [chunkdb](https://github.com/chunkdb/chunkdb): C++ storage engine, server, verifier and restore tools.
- [chunkdb-go](https://github.com/chunkdb/chunkdb-go): Go client for typed data, transactions and streams.
- [chunkdb-js](https://github.com/chunkdb/chunkdb-js): Node.js/TypeScript client published as `@chunkdb/client`.
- [chunk-cli](https://github.com/chunkdb/chunk-cli): Command-line and interactive CQL client.

## Documentation and issues

Read [CQL](https://github.com/chunkdb/chunkdb/blob/main/docs/CQL.md), [protocol](https://github.com/chunkdb/chunkdb/blob/main/docs/PROTOCOL.md), [durability](https://github.com/chunkdb/chunkdb/blob/main/docs/DURABILITY_CONTRACT.md), [compatibility](https://github.com/chunkdb/chunkdb/blob/main/docs/COMPATIBILITY.md) and [known limitations](https://github.com/chunkdb/chunkdb/blob/main/docs/KNOWN_LIMITATIONS.md).
Report reproducible server problems in [chunkdb issues](https://github.com/chunkdb/chunkdb/issues), and client problems in the corresponding repository's issue tracker.
