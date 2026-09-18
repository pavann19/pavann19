<h1 align="center">Hi 👋, I'm Pavan Kumar Gannoju</h1> <h3 align="center"> Software Engineer | Backend Systems · Distributed-Systems Correctness · Security </h3> <p align="center"> <a href="https://www.linkedin.com/in/pavan-gannoju/"> <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/> </a> <a href="https://pavann19.github.io/Pavan_kumar_gannoju_portfolio/"> <img src="https://img.shields.io/badge/Portfolio-111827?style=for-the-badge&logo=vercel&logoColor=white"/> </a> <a href="mailto:pavan9542644804@gmail.com"> <img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/> </a> </p>
💡 About Me
Computer Science Engineering graduate (AI/ML) who builds backend systems and checks them the hard way: with tests, fault injection, fuzzing, and CI. Open to junior / graduate software engineering roles in Germany.

Education: B.Tech in Computer Science & Engineering (AI/ML) · Minor Certification in Artificial Intelligence, IIT Ropar
Interests: backend engineering · distributed-systems correctness · systems and security engineering · AI infrastructure
🚀 Selected Projects
Each project states what CI checks and what it doesn't. Numbers link to files committed in the repo.

Gatekeeper — fail-closed AI security gateway
FastAPI gateway that screens prompts for injection and PII before they reach an LLM, using a learned fusion of several detectors with per-language calibration (including German).

Profiled the service with py-spy, found the detector ensemble oversubscribing CPU under concurrency, and caught a cache-warmth flaw in my own first benchmark before trusting it.
Shipped a torch-thread-pinning fix and re-ran the same workload; before/after numbers are in docs/perf/, including the p99 that did not improve.
CI: tests, dependency audit, and container build with Trivy + SBOM.
Python · FastAPI · PyTorch · Redis · Prometheus · Docker

Agentic-OS — capability-based x86_64 OS in Rust
UEFI-booting kernel where every resource is reached through an explicit, revocable capability, with no ambient authority.

GitHub Actions builds the kernel, runs host tests, boots it in QEMU, and asserts that capability revocation is enforced; ext2 parsers are fuzzed in CI.
Debugged a CI-only kernel crash down to a missing LAPIC end-of-interrupt in the timer handler.
docs/VERIFICATION.md marks each subsystem Verified in CI / Demonstrated / Partial / Experimental. Most are not CI-verified yet, and it says so. Everything runs under QEMU emulation, not on real hardware.
Rust (no_std) · UEFI · QEMU · GitHub Actions · cargo-fuzz

LedgerLine — double-entry ledger with proven concurrency behaviour
Spring Boot / PostgreSQL ledger with idempotent transfers, database-enforced zero-sum and non-negative-balance constraints, and a transactional outbox to Kafka with a deduplicating projection service.

Four transfer strategies (unprotected, pessimistic, optimistic, serializable) benchmarked with k6; raw results are committed, including the measured lost-update drift of the deliberately broken variant.
Failure tests use a real Kafka container, and property-based tests drive the real service.
The AWS deployment (Terraform) is defined but has not been run yet; docs/experiments/03-cloud-load.md says so.
Java 21 · Spring Boot · PostgreSQL · Kafka · Testcontainers · jqwik · k6 · Terraform

QuorumKV — replicated key-value store with a validated consistency checker
Go key-value store on a Raft cluster (hashicorp/raft), with a from-scratch write-ahead log and a fault-injection harness.

WAL survives 100/100 randomized kill trials with no lost or invented writes.
Five fault scenarios (leader partition, minority partition, rolling restarts, network delay, double-leader attempt) recorded and checked with Porcupine. The checker is validated against known-bad histories, and errored writes are modelled as "may have happened".
Histories are small and benchmarks run on localhost processes; both are stated in the docs.
Go · gRPC · Raft · Porcupine

ModelGate — Kubernetes admission control for ML workloads
Go admission webhook that admits only cosign-signed images and hash-verified safetensors model artifacts, and denies privileged and host-access pods.

Adversarial testing found two real bypasses (post-admission image swap, ephemeral containers) that the design had assumed away; both are fixed and tested.
Fuzzing the pickle detector broke my first two fixes; the third changed the detection strategy. The full sequence is in docs/DECISIONS.md.
CI runs unit tests, envtest, real cosign sign/verify, fuzzing, and a kind-cluster smoke test.
Go · Kubernetes · controller-runtime · cosign · envtest · kind

SentinAL — desktop agent with a deterministic safety layer
Voice/text agent that treats the LLM as untrusted: every action passes an allowlist, sandbox, and confirmation gate outside the model. Runs fully offline (SENTINAL_OFFLINE=1), and end-to-end task success is scored by checking OS state rather than the agent's own report.

Python · Windows automation · OpenTelemetry

💼 Professional Experience
Software Engineering Intern (AI Intern) — Prodigal AI Technologies Pvt. Ltd.
March 2025 – November 2025

Led intern teams in developing modular backend components and API workflows using Python and Agile methodologies
Built and optimized backend data-processing workflows and scalable REST APIs
Worked on workflow validation systems, orchestration pipelines, and secure execution concepts
Designed structured testing scenarios through failure-log analysis and edge-case validation
Software Engineering Intern (Gen AI / LLM Intern) — Digital Nexus AI
May 2025 – September 2025

Developed backend services using Python and RESTful APIs for enterprise applications
Built reliable inter-module communication systems and scalable backend workflows
Debugged and resolved backend defects using API request-flow analysis and server-log validation
Executed unit and functional testing to ensure software stability and data integrity
🛠️ Tech
Languages: Java · Go · Rust · Python · SQL · TypeScript / JavaScript Backend & data: Spring Boot · FastAPI · PostgreSQL · Kafka · Redis · SQLite Infrastructure & security: Docker · Kubernetes (kind, controller-runtime) · GitHub Actions · Terraform · cosign / Trivy / SBOM Testing: Testcontainers · property-based testing · fuzzing · Porcupine · k6

🧭 How I work
No number without a committed file. If a benchmark can't be reproduced from the repo, it isn't in the README.
Say what isn't verified. Each repo lists its known gaps.
Write down the dead ends. docs/DECISIONS.md in each project records rejected options and fixes that didn't hold.
I use AI coding tools as part of my workflow; I own the design decisions and can walk through every component.
🏆 Certifications & Learning
Google Cybersecurity Professional Certificate
Microsoft Cybersecurity & OS Fundamentals
SAP Code Unnati Advanced Training Program
Google Data Analytics
Python Data Structures
Networks & Cisco Devices
Smart India Hackathon participation
