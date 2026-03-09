## Don't send data. Send the law.

I'm Moroya Sakamoto — systems engineer based in Japan, building **Project A.L.I.C.E.**

ALICE is a modular ecosystem of **185 Rust crates** that encode computational laws — physics, geometry, cryptography, finance, AI/ML, robotics — into deterministic, hardware-native binaries. Instead of shipping raw data across networks, ALICE ships the rules that regenerate it.

### [alicelaw.net](https://alicelaw.net/) | [SDF Metaverse](https://alicelaw.net/sdf-metaverse)

### Quality

All 185 crates pass **ALICE-KARIKARI 100/100** quality standard:

| Metric | Result |
|--------|--------|
| Crates | **185 / 185** Tier A |
| clippy (pedantic + nursery) | **0 warnings** across all crates |
| Tests | **25,485+** (unit + doc-tests) |
| `cargo fmt` | **clean** across all crates |
| Top crate | ALICE-SDF — **1,077 tests** |

### The Ecosystem

| Domain | Crates | What it encodes |
|--------|--------|-----------------|
| **Geometry & Rendering** | SDF, View, Animation, Font, Print, PointCloud | Signed distance fields, CSG compiler, mesh generation |
| **Physics & Simulation** | Physics, Kinematics, Motion, Climate, Space, Atoms, Fluid, Robotics, Swarm | Fixed-point deterministic physics, Navier-Stokes, planetary SDF, swarm intelligence |
| **AI/ML** | ML, NLP, Vision, Embedding, RL, Diffusion, RAG, Train, TRT, LLM, GAN, AutoML | Ternary inference, diffusion models, retrieval-augmented generation, LLM serving |
| **Networking & Streaming** | Streaming-Protocol, Edge, CDN, DNS, API, Cloud-Gateway, VNet, MQTT, ServiceMesh, Proxy, WebSocket, gRPC, HTTP | Zero-copy frame transport, SDN overlay, service mesh, reverse proxy |
| **Data & Storage** | DB, Cache, Search, Text, Codec, Zip, History, VectorDB, Text-Compression, ETL, StreamProc, Lakehouse, CDC, FileSystem, ObjectStore | Lock-free caching, change data capture, columnar lakehouse, object storage |
| **Security & Finance** | Crypto, Auth, AuthZ, PKI, SIEM, SecretVault, Ledger, Risk, FIX, Settlement, Quant, MarketData, WAF, DLP, Audit | Policy-based authz, certificate lifecycle, stochastic pricing, WAF rules |
| **Science** | Bio, Neural, Quantum, Genome, Astro, Energy, Chemistry, Optics, Signal | Quantum circuits, genome FM-Index, celestial mechanics, molecular dynamics |
| **Infrastructure** | Container, Queue, RTOS, VCS, Sync, Presence, Scheduler, Log, Config, Migrate, Backup, Circuit, Consensus, Hypervisor, Storage, OTA, Sensor, IoT, Terraform, Monitor | Hypervisor, OTA firmware, sensor fusion, IoT device control, IaC provisioning |
| **DevTools** | CI, Debug, Sandbox, Lint, PackageRegistry | Build DAG optimization, AST pattern matching, capability sandbox |
| **XR/Application** | Browser, Form, Email, Payment, AR, VR, Haptic, Subtitle, GameEngine, Map, Identity, Blockchain, Accessibility | ECS game loop, AR/VR spatial composition, haptic feedback |
| **Communication** | Serial, RateLimit, Realtime, Collab, Workflow, Notify, TimeSeries, BLE, LoRa, NFC | UART/SPI/I²C, CRDT collaboration, time-series DB, BLE/LoRa/NFC |
| **Domain** | Billing, Legal, Legal-AI, Digital-Twin, Graph, Geo, Document, i18n, Compliance, FinCompliance, DataShield, Browser-Secure | Invoice engine, contract analysis, regulatory compliance |
| **Low-Level** | Image, WASM, FFI, SIMD, Metrics, Observability, Experiment, Test, Token | SIMD 8-wide, WASM VM, FFI, A/B testing |
| **Commercial** | Edge-Commercial, Streaming-Protocol-Commercial, Voice-Commercial | Enterprise-grade edge, streaming, voice |
| **Media** | Voice, Synth, Manga, ASR, TTS, OCR, Audio, Video, Camera | Parametric voice codec, speech recognition, text-to-speech, OCR, AV pipeline |
| **Spatial** | SLAM, Medical, Drone, Render, Navigation | SLAM mapping, medical imaging, UAV control, ray tracing, path planning |
| **Optimization** | Recommend, Logistics, Matchmaking, Agri | Recommendation, supply chain, ELO/Glicko-2, crop modeling |
| **Real-time** | Chat, LoadBalancer, VideoAnalytics | Chat protocol, L4/L7 load balancing, video tracking |
| **Compiler/Language** | Compiler, VM, Parser | DSL compiler, bytecode VM, parser combinators |
| **Business** | CRM, ERP, HRM, LMS | Customer management, inventory/MRP, payroll, learning |

All crates are connected through [ALICE-Eco-System](https://github.com/ext-sakamoro/ALICE-Eco-System) — 1,195 bridges across 22 pipeline paths.

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
