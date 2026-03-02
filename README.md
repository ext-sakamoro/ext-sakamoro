## Don't send data. Send the law.

I'm Moroya Sakamoto — systems engineer based in Japan, building **Project A.L.I.C.E.**

ALICE is a modular ecosystem of 52+ Rust crates that encode computational laws — physics, geometry, cryptography, finance — into deterministic, hardware-native binaries. Instead of shipping raw data across networks, ALICE ships the rules that regenerate it.

### [alicelaw.net](https://alicelaw.net/) | [SDF Metaverse](https://alicelaw.net/sdf-metaverse)

### The Ecosystem

| Domain | Crates | What it encodes |
|--------|--------|-----------------|
| **Geometry & Rendering** | SDF, View, Animation, Font, Print | Signed distance fields, CSG compiler, mesh generation |
| **Physics & Simulation** | Physics, Kinematics, Motion, Climate, Space | Fixed-point deterministic physics, planetary SDF fields |
| **Networking & Streaming** | Streaming-Protocol, Edge, CDN, DNS, API | Zero-copy frame transport, edge computing |
| **Data & Storage** | DB, Cache, Search, Text, Codec, Zip | Lock-free caching, full-text search, lossless compression |
| **Security & Finance** | Crypto, Auth, Ledger, Risk, FIX, Settlement | Post-quantum crypto, FIX protocol gateway |
| **Infrastructure** | Container, Queue, RTOS, VCS, Sync | Lightweight container runtime, real-time OS primitives |
| **AI & Sensing** | ML, Neural, Voice, Bio, Analytics | BCI signal compression, semantic telemetry |

All crates are connected through [ALICE-Eco-System](https://github.com/ext-sakamoro/ALICE-Eco-System) — 456 bridges across 21 pipeline paths.

### Design Philosophy

- **Send the law, not the data** — encode rules as deterministic functions; reconstruct on the edge
- **Hardware-native performance** — SoA layout, SIMD 8-wide (AVX2/NEON), branchless logic, division exorcism
- **Zero-cost composition** — each crate is independent; combine only what you need
- **100/100 quality standard** — clippy pedantic clean, full doc coverage, comprehensive tests

### Tech Stack

```
Rust · PyO3 · SIMD (AVX2/NEON) · Rayon · wgpu · Cranelift JIT
TypeScript · Next.js · Flutter · Unreal Engine 5
```
