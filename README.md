## Don't send data. Send the law.

I'm Moroya Sakamoto — systems engineer based in Japan, building **Project A.L.I.C.E.**

ALICE is a modular ecosystem of **151 Rust crates** that encode computational laws — physics, geometry, cryptography, finance, AI/ML, robotics — into deterministic, hardware-native binaries. Instead of shipping raw data across networks, ALICE ships the rules that regenerate it.

### [alicelaw.net](https://alicelaw.net/) | [SDF Metaverse](https://alicelaw.net/sdf-metaverse)

### Quality

All 151 crates pass **ALICE-KARIKARI 100/100** quality standard:

| Metric | Result |
|--------|--------|
| Crates | **151 / 151** Tier A |
| clippy (pedantic + nursery) | **0 warnings** across all crates |
| Tests | **21,840+** (unit + doc-tests) |
| `cargo fmt` | **clean** across all crates |
| Top crate | ALICE-SDF — **1,077 tests** |

### The Ecosystem

| Domain | Crates | What it encodes |
|--------|--------|-----------------|
| **Geometry & Rendering** | SDF, View, Animation, Font, Print, PointCloud | Signed distance fields, CSG compiler, mesh generation |
| **Physics & Simulation** | Physics, Kinematics, Motion, Climate, Space, Atoms, Fluid, Robotics | Fixed-point deterministic physics, Navier-Stokes, planetary SDF |
| **AI/ML** | ML, NLP, Vision, Embedding, RL, Diffusion, RAG, Train, TRT | Ternary inference, diffusion models, retrieval-augmented generation |
| **Networking & Streaming** | Streaming-Protocol, Edge, CDN, DNS, API, Cloud-Gateway, VNet, MQTT, ServiceMesh | Zero-copy frame transport, SDN overlay, service mesh |
| **Data & Storage** | DB, Cache, Search, Text, Codec, Zip, History, VectorDB, Text-Compression, ETL, StreamProc, Lakehouse, CDC | Lock-free caching, change data capture, columnar lakehouse |
| **Security & Finance** | Crypto, Auth, AuthZ, PKI, SIEM, SecretVault, Ledger, Risk, FIX, Settlement, Quant, MarketData | Policy-based authz, certificate lifecycle, stochastic pricing |
| **Science** | Bio, Neural, Quantum, Genome, Astro, Energy | Quantum circuits, genome FM-Index, celestial mechanics |
| **Infrastructure** | Container, Queue, RTOS, VCS, Sync, Presence, Scheduler, Log, Config, Migrate, Backup, Circuit, Consensus, Hypervisor, Storage, OTA, Sensor | Hypervisor, OTA firmware, sensor fusion |
| **DevTools** | CI, Debug, Sandbox, Lint, PackageRegistry | Build DAG optimization, AST pattern matching, capability sandbox |
| **Application** | Browser, Form, Email, Payment, AR, Haptic, Subtitle, GameEngine, Map, Identity, Blockchain, Accessibility | ECS game loop, AR spatial composition, haptic feedback |
| **Communication** | Serial, RateLimit, Realtime, Collab, Workflow, Notify, TimeSeries | UART/SPI/I²C, CRDT collaboration, time-series DB |
| **Domain** | Billing, Legal, Legal-AI, Digital-Twin, Graph, Geo, Document, i18n, Compliance, FinCompliance, DataShield, Browser-Secure | Invoice engine, contract analysis, regulatory compliance |
| **Low-Level** | Image, WASM, FFI, SIMD, Metrics, Observability, Experiment, Test, Token | SIMD 8-wide, WASM VM, FFI, A/B testing |
| **Commercial** | Edge-Commercial, Streaming-Protocol-Commercial, Voice-Commercial | Enterprise-grade edge, streaming, voice |
| **Media** | Voice, Synth, Manga, ASR, TTS, OCR | Parametric voice codec, speech recognition, text-to-speech, OCR |
| **Spatial** | SLAM, Medical, Drone, Render | SLAM mapping, medical imaging, UAV control, ray tracing |
| **Optimization** | Recommend, Logistics, Matchmaking, Agri | Recommendation, supply chain, ELO/Glicko-2, crop modeling |
| **Real-time** | Chat, LoadBalancer, VideoAnalytics | Chat protocol, L4/L7 load balancing, video tracking |

All crates are connected through [ALICE-Eco-System](https://github.com/ext-sakamoro/ALICE-Eco-System) — 734 bridges across 22 pipeline paths.

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
