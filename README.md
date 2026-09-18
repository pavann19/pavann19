<h1 align="center">Pavan Kumar Gannoju</h1>

<p align="center">
  <b>Software Engineer</b> · Backend Systems · Distributed-Systems Correctness · Security
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/pavan-gannoju/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="https://pavann19.github.io/Pavan_kumar_gannoju_portfolio/"><img src="https://img.shields.io/badge/Portfolio-111827?style=for-the-badge&logo=vercel&logoColor=white"/></a>
  <a href="mailto:pavan9542644804@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>
</p>

I build backend and systems software and verify it with tests, fault injection, fuzzing and CI. Every project below says what is checked automatically and what is not.

|  |  |
|---|---|
| 🎓 **Education** | B.Tech, Computer Science & Engineering (AI/ML) · Minor in Artificial Intelligence, IIT Ropar |
| 💼 **Experience** | Two software engineering internships (AI / Gen AI), 2025 |
| 🎯 **Looking for** | Junior / graduate software engineering roles in Germany |
| 🧰 **Main stack** | Java · Go · Rust · Python · PostgreSQL · Kafka · Kubernetes |

---

## 🚀 Featured Projects

| Project | What it is | Evidence in the repo |
|---|---|---|
| **[Gatekeeper](https://github.com/pavann19/Gatekeeper-AI-Infrastructure-and-Governance-Gateway)**<br>![CI](https://github.com/pavann19/SentinAL-Desktop-AI-Orchestration/actions/workflows/ci.yml/badge.svg) | Fail-closed AI security gateway that screens prompts for injection and PII before they reach an LLM (multi-detector fusion, German-language calibration) | py-spy profiling and a benchmark methodology flaw I caught myself · before/after results in `docs/perf/` · Trivy + SBOM in CI |
| **[Agentic-OS](https://github.com/pavann19/Agentic-OS)**<br>![CI](https://github.com/pavann19/Agentic-OS/actions/workflows/ci.yml/badge.svg) | Capability-based x86_64 OS in Rust: every resource is reached through an explicit, revocable capability | CI builds, boots in QEMU and asserts capability revocation · ext2 parsers fuzzed · per-subsystem status in `docs/VERIFICATION.md` (QEMU only, no real hardware) |
| **[LedgerLine](https://github.com/pavann19/LedgerLine)**<br>![CI](https://github.com/pavann19/LedgerLine/actions/workflows/ci.yml/badge.svg) | Double-entry ledger (Spring Boot, PostgreSQL) with idempotent transfers, a transactional outbox and Kafka projection | Four locking strategies benchmarked with committed k6 output · real-Kafka failure tests · property tests · AWS deployment defined but **not yet run** |
| **[QuorumKV](https://github.com/pavann19/QuorumKV)**<br>![CI](https://github.com/pavann19/QuorumKV/actions/workflows/ci.yml/badge.svg) | Replicated key-value store in Go on `hashicorp/raft`, with my own write-ahead log and fault-injection harness | 100/100 crash-recovery trials · 5 fault scenarios checked with Porcupine · checker validated on known-bad histories |
| **[ModelGate](https://github.com/pavann19/ModelGate)**<br>![CI](https://github.com/pavann19/ModelGate/actions/workflows/ci.yml/badge.svg) | Kubernetes admission webhook allowing only cosign-signed images and hash-verified safetensors model artifacts | Found and fixed two real bypasses · fuzzing · real cosign test · kind-cluster smoke test in CI |
| **[SentinAL](https://github.com/pavann19/SentinAL-Desktop-AI-Orchestration)** | Desktop agent that treats the LLM as untrusted: allowlist, sandbox and confirmation gate sit outside the model | Fully offline mode (`SENTINAL_OFFLINE=1`) · task success scored from OS state, not the agent's own report |

---

## 💼 Experience

**Software Engineering Intern (AI Intern) — Prodigal AI Technologies Pvt. Ltd.** · *March 2025 – November 2025*
- Led intern teams building modular backend components and API workflows in Python, following Agile practice
- Built and optimized backend data-processing workflows and scalable REST APIs
- Worked on workflow validation, orchestration pipelines and secure-execution concepts
- Designed structured test scenarios from failure-log analysis and edge-case validation

**Software Engineering Intern (Gen AI / LLM Intern) — Digital Nexus AI** · *May 2025 – September 2025*
- Developed backend services in Python with RESTful APIs for enterprise applications
- Built reliable inter-module communication and scalable backend workflows
- Debugged backend defects through API request-flow analysis and server-log validation
- Wrote unit and functional tests to protect stability and data integrity

---

## 🛠️ Tech

| | |
|---|---|
| **Languages** | Java · Go · Rust · Python · SQL · TypeScript / JavaScript |
| **Backend & data** | Spring Boot · FastAPI · PostgreSQL · Kafka · Redis · SQLite |
| **Infrastructure & security** | Docker · Kubernetes (kind, controller-runtime) · GitHub Actions · Terraform · cosign · Trivy · SBOM |
| **Testing & verification** | Testcontainers · property-based testing · fuzzing · Porcupine · k6 · envtest |

---

## 🧭 How I Work

- **No number without a committed file.** A benchmark that can't be reproduced from the repo stays out of the README.
- **State what isn't verified.** Each repo lists its known gaps.
- **Record the dead ends.** `docs/DECISIONS.md` in each project keeps rejected options and fixes that didn't hold.
- I use AI coding tools in my workflow. I own the design decisions and can walk through every component.

---

## 🏆 Certifications & Learning

Google Cybersecurity Professional Certificate · Microsoft Cybersecurity & OS Fundamentals · SAP Code Unnati Advanced Training Program · Google Data Analytics · Python Data Structures · Networks & Cisco Devices · Smart India Hackathon participant
