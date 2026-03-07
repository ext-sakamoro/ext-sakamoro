## Don't send data. Send the law.

I'm Moroya Sakamoto — systems engineer based in Japan, building **Project A.L.I.C.E.**

ALICE is a modular ecosystem of **86 Rust crates** that encode computational laws — physics, geometry, cryptography, finance — into deterministic, hardware-native binaries. Instead of shipping raw data across networks, ALICE ships the rules that regenerate it.

### [alicelaw.net](https://alicelaw.net/) | [SDF Metaverse](https://alicelaw.net/sdf-metaverse)

### Quality

All 86 crates pass **ALICE-KARIKARI 100/100** quality standard:

| Metric | Result |
|--------|--------|
| Crates | **86 / 86** Tier A |
| clippy (pedantic + nursery) | **0 warnings** across all crates |
| Tests | **10,889** (unit + doc-tests) |
| `cargo fmt` | **clean** across all crates |
| Top crate | ALICE-SDF — **1,077 tests** |

### The Ecosystem

| Domain | Crates | What it encodes |
|--------|--------|-----------------|
| **Geometry & Rendering** | SDF, View, Animation, Font, Print | Signed distance fields, CSG compiler, mesh generation |
| **Physics & Simulation** | Physics, Kinematics, Motion, Climate, Space, Atoms | Fixed-point deterministic physics, planetary SDF fields |
| **Networking & Streaming** | Streaming-Protocol, Edge, CDN, DNS, API, Cloud-Gateway | Zero-copy frame transport, edge computing |
| **Data & Storage** | DB, Cache, Search, Text, Codec, Zip, History, VectorDB, Text-Compression | Lock-free caching, full-text search, HNSW vector similarity |
| **Security & Finance** | Crypto, Auth, Ledger, Risk, FIX, Settlement, Legal, Compliance, FinCompliance, DataShield, Browser-Secure | Post-quantum crypto, FIX gateway, regulatory compliance |
| **Infrastructure** | Container, Queue, RTOS, VCS, Sync, Registry, Presence, Scheduler, Log, Config, Migrate, Backup, Circuit, Consensus | Container runtime, RTOS, circuit breaker, Raft consensus |
| **Communication** | Serial, RateLimit, Realtime, Collab, Workflow, Notify | UART/SPI/I²C, rate limiting, CRDT collaboration |
| **AI & Sensing** | ML, Neural, Train, Voice, Bio, Analytics, Semantic-Telemetry, Token, Experiment, Test | BCI compression, semantic telemetry, A/B testing |
| **Domain** | Billing, Legal-AI, Digital-Twin, Graph, Geo, Document, i18n | Invoice engine, contract analysis, property graph |
| **Low-Level** | Image, WASM, FFI, Metrics, Observability | Image processing, WASM VM, FFI bindings, OpenTelemetry |
| **Performance** | SIMD, TRT, Energy, Edge-Firewall | AVX2/NEON SIMD, tensor runtime, power-aware compute |
| **Commercial** | Edge-Commercial, Streaming-Protocol-Commercial, Voice-Commercial | Enterprise-grade edge, streaming, voice |

All crates are connected through [ALICE-Eco-System](https://github.com/ext-sakamoro/ALICE-Eco-System) — 719 bridges across 22 pipeline paths.

### Design Philosophy

- **Send the law, not the data** — encode rules as deterministic functions; reconstruct on the edge
- **Hardware-native performance** — SoA layout, SIMD 8-wide (AVX2/NEON), branchless logic, division exorcism
- **Zero-cost composition** — each crate is independent; combine only what you need
- **100/100 quality standard** — clippy pedantic+nursery 0 warnings, 100+ tests per crate, fmt clean

### Tech Stack

```
Rust · PyO3 · SIMD (AVX2/NEON) · Rayon · wgpu · Cranelift JIT
TypeScript · Next.js · Flutter · Unreal Engine 5
```
