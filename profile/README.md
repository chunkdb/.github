# chunkdb

`chunkdb` is a specialized chunk/grid storage engine for games and grid-based simulations, with bit-packed block storage and a chunk-native protocol.

## Why it exists

- Store world and grid state in configurable chunk hierarchies instead of forcing it into a row-oriented model.
- Expose a chunk-native protocol for point reads, point writes, and full-chunk transfer.
- Provide explicit WAL/checkpoint durability modes with documented guarantees and limitations.

## Current status

- Public release channel: [Release Preview `v0.1.1-preview`](https://github.com/chunkdb/chunkdb/releases/tag/v0.1.1-preview)
- Evaluation and integration testing: supported
- Stable release status: no stable release has been published yet
- Windows Native TLS: not yet guaranteed as fully supported

## Repositories

- [chunkdb](https://github.com/chunkdb/chunkdb): C++ storage engine, TCP server, durability docs, tests, and benchmarks.
- [chunk-cli](https://github.com/chunkdb/chunk-cli): Go CLI for `ping`, `info`, `auth`, `get`, `set`, `chunk`, `chunkbin`, and interactive shell use.
- [chunkdb-js](https://github.com/chunkdb/chunkdb-js): Official Node.js/TypeScript client (`@chunkdb/client`) with `chunk://`/`chunks://` (TLS), connection pooling, and pipelining.

## Quick entry points

- [Open the `chunkdb` repository](https://github.com/chunkdb/chunkdb)
- [Open the `chunk-cli` repository](https://github.com/chunkdb/chunk-cli)
- [Open the `chunkdb-js` repository](https://github.com/chunkdb/chunkdb-js)
- [Open the current preview release](https://github.com/chunkdb/chunkdb/releases/tag/v0.1.1-preview)
- [Read the main `chunkdb` README](https://github.com/chunkdb/chunkdb#readme)
- [Read the protocol documentation](https://github.com/chunkdb/chunkdb/blob/main/docs/PROTOCOL.md)
- [Read the release policy](https://github.com/chunkdb/chunkdb/blob/main/docs/RELEASE_POLICY.md)
- [Read the artifact verification guide](https://github.com/chunkdb/chunkdb/blob/main/docs/VERIFY_RELEASE.md)

## Start here

- Want to run the server: start with the [`chunkdb` README quick start](https://github.com/chunkdb/chunkdb#protocol-startup-and-connection-examples).
- Want CLI interaction: start with [`chunk-cli`](https://github.com/chunkdb/chunk-cli#quick-start) and then use [`chunk-cli shell`](https://github.com/chunkdb/chunk-cli#interactive-shell).
- Want to integrate from Node.js/TypeScript: use [`chunkdb-js`](https://github.com/chunkdb/chunkdb-js#readme) (`@chunkdb/client`).
- Want to inspect release artifacts: open the [preview release](https://github.com/chunkdb/chunkdb/releases/tag/v0.1.1-preview) and verify downloads with [VERIFY_RELEASE.md](https://github.com/chunkdb/chunkdb/blob/main/docs/VERIFY_RELEASE.md).

## Current limitations

- The public release channel is preview, not stable.
- Windows Native TLS is not yet guaranteed and is not part of stable support claims yet.
- `chunkdb` does not provide multi-chunk transactions and is not a full ACID DBMS.

## Roadmap direction

- The next focus is SDK/client adoption and real consumer validation.
- Ongoing work will keep prioritizing durability proof, platform validation, and benchmark transparency over scope expansion.

## Contribute or report issues

- [Open an issue in `chunkdb`](https://github.com/chunkdb/chunkdb/issues)
- [Open an issue in `chunk-cli`](https://github.com/chunkdb/chunk-cli/issues)
- [Open an issue in `chunkdb-js`](https://github.com/chunkdb/chunkdb-js/issues)
- [Read the `chunkdb` issue policy](https://github.com/chunkdb/chunkdb/blob/main/docs/ISSUE_POLICY.md)
