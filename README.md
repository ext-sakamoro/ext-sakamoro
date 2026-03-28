## Don't send data. Send the law.

I'm Moroya Sakamoto — systems engineer based in Japan, building **Project A.L.I.C.E.**

ALICE is a modular ecosystem of **514 Rust crates** and **299 SaaS products** that encode computational laws — physics, geometry, cryptography, finance, AI/ML, robotics, healthcare, logistics, and every major industry vertical — into deterministic, hardware-native binaries. Instead of shipping raw data across networks, ALICE ships the rules that regenerate it.

### [alicelaw.net](https://alicelaw.net/) | [SDF Metaverse](https://alicelaw.net/sdf-metaverse)

### Numbers

| Metric | Value |
|--------|-------|
| Rust Crates | **211** core + **299** SaaS + **4** commercial = **514 total** |
| SaaS Products | **299** (all public, AGPL-3.0) |
| Eco-System Bridges | **1,301** across 237 bridge files |
| Project-ALICE (AGI) | **9 crates**, 98K LoC, **2,376 tests** |
| Top Crate | ALICE-SDF — **1,077 tests** |
| clippy (pedantic+nursery) | **0 warnings** across all crates |
| LLM | ALICE-Cognitive-9B-Ternary (Qwen3.5-9B, 1.58-bit QAT, ~3.6GB) |

### The Ecosystem

| Domain | Crates | What it encodes |
|--------|--------|-----------------|
| **Geometry & 3D** | SDF, LOL, View, Animation, Font, Print, PointCloud, Bamboo | SDF compiler, LOL DSL, mesh generation, 3D printing pipeline |
| **Physics & Simulation** | Physics, Kinematics, Motion, Climate, Fluid, Atoms, Robotics, Swarm | Fixed-point deterministic physics, Navier-Stokes, swarm intelligence |
| **AI/ML & LLM** | ML, NLP, Vision, Embedding, RL, Diffusion, RAG, Train, TRT, LLM, GAN, AutoML | 1.58-bit QAT, ternary inference, GGUF, speculative decoding |
| **AGI Core** | Project-ALICE (9 crates) | 106 tools, 7 reasoning strategies, BDI, IIT Phi, ethics, swarm, innovation |
| **Networking** | Streaming-Protocol, Edge, CDN, DNS, API, Cloud-Gateway, VNet, MQTT, gRPC, HTTP, WebSocket | Zero-copy transport, SDN overlay, service mesh |
| **Data & Storage** | DB, Cache, VectorDB, Lakehouse, Search, ETL, StreamProc, CDC, TimeSeries, Graph | Lock-free caching, columnar lakehouse, change data capture |
| **Security** | Auth, AuthZ, Crypto, PKI, SIEM, WAF, DLP, SecretVault, DataShield | Zero-knowledge auth, certificate lifecycle, policy-based authz |
| **Finance** | Ledger, Risk, FIX, Settlement, Quant, MarketData, FinCompliance, Billing, Payment | FIX protocol, stochastic pricing, deterministic matching |
| **Science** | Bio, Quantum, Genome, Astro, Energy, Chemistry, Optics, Climate | Quantum circuits, molecular dynamics, celestial mechanics |
| **Infrastructure** | Container, Queue, RTOS, Terraform, Monitor, Scheduler, Hypervisor, OTA | Container orchestration, IaC, OTA firmware, sensor fusion |
| **Media** | Video, Audio, Voice, TTS, ASR, OCR, Camera, Codec, Subtitle | Parametric voice codec, AV pipeline, speech recognition |
| **IoT/Edge** | Edge, BLE, NFC, LoRa, Sensor, Serial, IoT, Drone, RTOS | Edge inference, BLE/LoRa/NFC protocols, UAV control |
| **XR/Spatial** | AR, VR, SLAM, Digital-Twin, Haptic, GameEngine, Metaverse | Spatial composition, SLAM mapping, game ECS |
| **DevTools** | CI, Debug, Lint, Test, QA, Sandbox, PackageRegistry, LogMgmt | Build DAG, AST matching, test automation |
| **Compiler/Language** | Compiler, VM, Parser, LOL, WASM | DSL compiler, bytecode VM, law-oriented DSL |

### SaaS Coverage (299 Products)

Full industry vertical coverage — every SaaS follows **MIT Core + AGPL-3.0 Shell** pattern:

| Category | Products | Examples |
|----------|----------|---------|
| **AI/ML** | 18 | LLM, AutoML, RAG, Embedding, Vision, OCR, ASR, TTS |
| **Data & Infrastructure** | 36 | DB, VectorDB, Cache, CDN, DNS, Container, Terraform, Monitor |
| **Security & Compliance** | 20 | Auth, WAF, SIEM, DLP, PKI, GRC, ESG, DataShield |
| **Finance & Commerce** | 18 | Ledger, Payment, POS, Invoice, Ecommerce, InsurTech, IPO |
| **Healthcare** | 6 | EHR, Telemedicine, Pharmacy, Dental, CareTech, Wellness |
| **Business Operations** | 20 | CRM, ERP, HRM, ATS, Payroll, ProjectMgmt, RPA, BI, Support |
| **Real Estate & Construction** | 3 | PropTech, Construction, BIM |
| **Education** | 3 | EdTech, LMS, Exam |
| **Travel & Hospitality** | 5 | Travel, PMS, Booking, Revenue, FoodTech |
| **Transport & Mobility** | 4 | Mobility, Aviation, Maritime, Railway |
| **Smart Infrastructure** | 6 | SmartCity, PowerGrid, WaterMgmt, WasteMgmt, Disaster, Recycle |
| **Primary Industry** | 6 | Agri, AgriIoT, Fishery, Forestry, Mining, SpaceTech |
| **Media & Creative** | 10 | Music, Manga, Animation, DAM, CMS, NoCode, GameCloud, Metaverse |
| **Lifestyle** | 3 | PetTech, SportsTech, Wellness |
| **Text-to-CAD** | 1 | Text → LOL DSL → SDF → .3mf (Bambu Lab) |
| **+ 140 more** | ... | Networking, IoT, Codec, Streaming, etc. |

### Design Philosophy

- **Send the law, not the data** — encode rules as deterministic functions; reconstruct on the edge
- **Hardware-native performance** — SoA layout, SIMD 8-wide (AVX2/NEON), branchless logic, division exorcism
- **Zero-cost composition** — each crate is independent; combine only what you need
- **100/100 quality standard** — clippy pedantic+nursery 0 warnings, comprehensive tests, fmt clean
- **Full-stack SaaS** — every core crate has a corresponding AGPL-3.0 SaaS with Stripe billing

### Tech Stack

```
Rust · PyO3 · SIMD (AVX2/NEON) · Rayon · wgpu · Cranelift JIT
TypeScript · Next.js · Supabase · Stripe
Qwen3.5-9B · 1.58-bit QAT · DeltaNet
```

### Contact

sakamoro@alicelaw.net
