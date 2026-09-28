<h1 align="center">Pavan Kumar Gannoju</h1>

<p align="center">
  <b>Software Engineer</b><br>
  Backend Systems · Distributed Systems · Infrastructure · Security
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/pavan-gannoju/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white">
  </a>
  <a href="https://pavann19.github.io/Pavan_kumar_gannoju_portfolio/">
    <img src="https://img.shields.io/badge/Portfolio-111827?style=for-the-badge&logo=githubpages&logoColor=white">
  </a>
  <a href="mailto:pavan9542644804@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white">
  </a>
</p>

---

## About

I build backend and systems software because I like understanding what happens underneath the application layer.

Most of my recent work has been around **backend services, databases, distributed systems, Kubernetes and security**. I also build lower-level projects when I want to explore storage, operating systems, concurrency and failure handling.

I prefer projects where I can explain the design, the trade-offs, the bugs I found and how I tested the result.

Build something, test it, find what breaks, then fix it.

| |  |
| ----------------- | ------------------------------------------------------------------------------------------- |
| **German** | A2 in progress                                                                            |
| **Relocating to** | Ilmenau, Germany                                                                            |
| **Looking for**   | Junior Software Engineer · Backend Engineer · Werkstudent · Software Engineering Internship |
| **Available**     | 1 April 2027                                                                                |

---

## Education

**M.Sc. Research in Computer and Systems Engineering (RCSE)**<br>
**Technische Universität Ilmenau, Germany**<br>
*Incoming Student · April 2027*

**B.Tech in Computer Science and Engineering**<br>
**Jawaharlal Nehru Technological University Hyderabad**<br>
*Graduated · April 2026*

---

## Technical Stack

| Area                    | Technologies                                                                              |
| ----------------------- | ----------------------------------------------------------------------------------------- |
| **Languages**           | Java · Go · Rust · Python · SQL                                                           |
| **Backend**             | Spring Boot · FastAPI · REST APIs · gRPC                                                  |
| **Data & Messaging**    | PostgreSQL · Redis · Kafka                                                                |
| **Distributed Systems** | Raft · WAL · Concurrency · Isolation · Idempotency                                        |
| **Infrastructure**      | Docker · Kubernetes · kind · Terraform · GitHub Actions · Azure                           |
| **Security & Testing**  | cosign · Trivy · SBOM · Fuzzing · Property Testing · Testcontainers · envtest · k6 · QEMU |

---

## Selected Projects

### [LedgerLine](https://github.com/pavann19/LedgerLine)

**Java 21 · Spring Boot · PostgreSQL · Kafka**

> Financial ledger built around double-entry accounting and database-enforced invariants.

* **258.9 req/s (pessimistic locking)** under high contention in the recorded local k6 run using Docker Compose on a Windows developer laptop with Docker Desktop; Postgres, Kafka and the services shared the host CPU and disk.
* Under the same hot-account workload, optimistic locking reached 60.4 req/s with 13.5% request failures, while serializable isolation reached 50.0 req/s with 13.4% request failures; these were final HTTP failures after retry/abort exhaustion.
* Built idempotent transfers, deterministic locking, PostgreSQL constraints, transactional outbox and Kafka projections.
* A short-lived Azure evidence run completed 7,508/7,508 transfers successfully before the environment was removed.

---

### [QuorumKV](https://github.com/pavann19/QuorumKV)

**Go · Raft · gRPC · WAL**

> Replicated key-value store built to explore storage, consensus and failure recovery.

* **100 crash-recovery trials** against a real subprocess, checking that committed writes survived abrupt termination.
* Built a CRC-checked, `fsync`-backed WAL and a real 3-process Raft cluster with leader election and recovery.
* Added custom network fault injection for partitions, delays and rolling failures; client histories from five scenarios passed Porcupine linearizability checks.

---

### [ModelGate](https://github.com/pavann19/ModelGate)

**Go · Kubernetes · cosign · safetensors**

> Kubernetes admission webhook for signed container images and verified model artifacts.

* **2 real admission bypasses fixed**: image swaps through `kubectl set image` and ephemeral-container injection.
* Fuzz-tested artifact validation and added real cosign integration testing.
* kind-cluster smoke tests run in CI, with fail-closed admission and Helm/Kustomize deployment paths.

---

### [Agentic-OS](https://github.com/pavann19/Agentic-OS)

**Rust · x86_64 · UEFI · QEMU**

> From-scratch operating-system project focused on capability-based resource access.

* **CI verifies** capability revocation, syscall/IPC boundaries, address-space isolation and UEFI boot.
* Implemented capability management, memory management, IPC and user-space services.
* Currently QEMU-only; physical hardware support remains future work.

---

### [Gatekeeper](https://github.com/pavann19/Gatekeeper-AI-Infrastructure-and-Governance-Gateway)

**Python · FastAPI · Redis · FAISS · SQLite**

> Backend gateway that evaluates requests before they reach a language model.

* **70.0% recall at a 5% false-positive-rate operating point** on a 6,933-prompt evaluation suite.
* Combines rule checks, PII detection, similarity search and multiple detectors, with Redis-backed rate limiting and circuit breaking.
* Repository includes calibration, profiling and evaluation results with documented limitations.

---

### [SentinAL](https://github.com/pavann19/SentinAL-Desktop-AI-Orchestration)

**Python · Windows · Desktop Automation**

> Desktop automation project where important actions are checked outside the model.

* **96.7% end-to-end task success** across 120 evaluated tasks with independent Windows OS-state verification.
* Separates permissions from execution and checks whether the expected system state actually changed.
* 66/66 adversarial cases were blocked in the recorded security fuzz suite.
* Windows-only; 6 of 19 intents still lack independent postcondition checks.

---

## Experience

### Prodigal AI Technologies Pvt. Ltd.

**AI Intern (with Research Team Lead responsibilities)**
*March 2025 – November 2025 · Remote*

* Led a team of **5 interns** in an R&D unit focused on generative-AI security and trustworthy AI systems.
* Led the architectural design of a **white-box input-control protocol** for expressive zero-shot voice cloning with Mixture-of-Experts models (*“Guided Multi-Modal Sampling…” — manuscript*).
* Built a **defence-in-depth framework** against prompt injection, data poisoning and adversarial manipulation in LLMs (*“AI Tamper-Proofing and Data Integrity…” — manuscript*).
* Defined research protocols, ran empirical benchmarking and managed the research-publication workflow.

### Digital Nexus AI

**Gen AI / LLM Intern**
*May 2025 – September 2025 · Remote*

* Built Python backend services and REST APIs.
* Worked on service-to-service communication and request flows.
* Debugged backend issues using logs and request analysis.
* Added unit and functional tests.

---

## Certifications

* Google Cybersecurity Professional Certificate
* Microsoft Cybersecurity & OS Fundamentals
* SAP Code Unnati Advanced Training Program
