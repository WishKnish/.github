<div align="center">
  <img src="https://raw.githubusercontent.com/WishKnish/KnishIO-Technical-Whitepaper/master/KnishIO-Logo.png" alt="Knish.IO" width="320" />

  **Cryptographic-evidence infrastructure for regulated industries.**<br/>
  Tamper-evident, post-quantum-signed, append-only by construction.

  [Website](https://wishknish.com) · [Developers](https://wishknish.com/developers) · [Whitepaper](https://github.com/WishKnish/KnishIO-Technical-Whitepaper) · [Contact](https://wishknish.com/contact)
</div>

---

Every regulated industry has the same problem at the moment of handoff: a record moves between organizations, systems or people, and everyone downstream has to trust it. **Knish.IO** replaces that trust with evidence anyone can verify. It is a post-blockchain ledger: atomic transactions ("molecules") in a DAG, every one signed with post-quantum one-time signatures (WOTS+ over SHAKE256), with zero gas fees. It runs from a Raspberry Pi to the cloud and sits underneath existing systems instead of replacing them.

## Client SDKs

Eight implementations of the same signing, molecule-building and verification logic. Every SDK runs the same conformance suite, so a molecule signed in Rust verifies byte-for-byte against one signed in TypeScript. All GPL-3.0.

| Language | Repository | Install | Status |
| --- | --- | --- | --- |
| JavaScript / Node.js | [KnishIO-Client-JS](https://github.com/WishKnish/KnishIO-Client-JS) | `npm install @wishknish/knishio-client-js` | production |
| TypeScript | [KnishIO-Client-TS](https://github.com/WishKnish/KnishIO-Client-TS) | `npm install @wishknish/knishio-client-ts` | production |
| Rust | [KnishIO-Client-Rust](https://github.com/WishKnish/KnishIO-Client-Rust) | `cargo add knishio-client` | production |
| Python | [KnishIO-Client-Python](https://github.com/WishKnish/KnishIO-Client-Python) | `pip install knishioclient` | production |
| Kotlin / JVM | [KnishIO-Client-Kotlin](https://github.com/WishKnish/KnishIO-Client-Kotlin) | `io.knish:knishio-client-kotlin` (Maven Central) | production |
| PHP | [KnishIO-Client-PHP](https://github.com/WishKnish/KnishIO-Client-PHP) | `composer require wishknish/knishio-client-php` | production |
| C | [KnishIO-Client-C](https://github.com/WishKnish/KnishIO-Client-C) | build from source (CMake) | in active development |
| C++ | [KnishIO-Client-CPP](https://github.com/WishKnish/KnishIO-Client-CPP) | build from source (CMake) | in active development |

## Core and tooling

| Repository | What it is |
| --- | --- |
| [KnishIO-Crypto-Core](https://github.com/WishKnish/KnishIO-Crypto-Core) | One small C library for the hot cryptographic paths every SDK shares over FFI: SHAKE256, WOTS+ chains, ML-KEM-768/1024 (FIPS 203) |
| [KnishIO-Kcore-JS](https://github.com/WishKnish/KnishIO-Kcore-JS) | Node bindings for the Crypto Core, with a WebAssembly fallback |
| [KnishIO-CLI](https://github.com/WishKnish/KnishIO-CLI) | `cargo install knishio-cli`: runs, health-checks and benchmarks a validator stack locally |
| [KnishIO-Technical-Whitepaper](https://github.com/WishKnish/KnishIO-Technical-Whitepaper) | The formal foundations (v6.1): molecules, post-quantum signing, ContinuID identity continuity, validation |

## Working with us

- **Building on Knish.IO?** Start with an SDK README, then [wishknish.com/developers](https://wishknish.com/developers).
- **Found a security issue?** Please report it privately; see each repository's `SECURITY.md`. Don't open a public issue.
- **Want a pilot or an integration?** [wishknish.com/contact](https://wishknish.com/contact). Engineers and solutions architects answer, usually within one business day.

<sub>WishKnish Corp. · Washington, D.C.</sub>
