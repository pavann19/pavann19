<h1 align="center">Pavan Kumar Gannoju</h1>

<p align="center">
  <b>Backend / Platform Engineer</b><br>
  Java · Go · Kubernetes · Azure · AI Security
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

I build backend and platform systems and verify them with **CI, fault injection, fuzzing, cloud evidence, and reproducible tests**.

Most of my recent work has been around backend services, databases, distributed systems, Kubernetes and security. I also build lower-level projects when I want to explore storage, operating systems, concurrency and failure handling.

I prefer projects where I can explain the design, the trade-offs, the bugs I found and how I tested the result.

Build something, test it, find what breaks, then fix it.

|                   |                                                                                             |
| ----------------- | ------------------------------------------------------------------------------------------- |
| **German**        | A2 in progress                                                                              |
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
* Idempotent, principal-scoped transfers, deterministic locking, PostgreSQL constraints, a transactional outbox and Kafka projections.
* Recorded Azure runs on 2026-10-26 reached 322.83 and 329.80 transfers/s with p95 362.01 and 341.11 ms and zero failures, on Premium SSD v2 storage; the repository states this is not a code-only improvement over earlier runs.
* A disposable Azure acceptance run passed smoke checks, a k6 correctness profile, SQL invariant checks and cleanup. Production operation is not claimed.

### [ModelGate](https://github.com/pavann19/ModelGate)
**Go · Kubernetes · cosign**
> Kubernetes validating admission webhook for signed image digests and bounded local model-artifact checks.
* Regression tests cover image updates and ephemeral-container admission; real registry/signature acceptance and mocked-verifier bypass tests are documented separately.
* Fuzzing, cosign integration, envtest and kind smoke tests run in CI; admission fails closed.

### [SentinAL](https://github.com/pavann19/SentinAL-Desktop-AI-Orchestration)
**Python · Windows · Desktop Automation**
> Supervised desktop voice/text agent with deterministic action controls and OS-state postcondition checks.
* A historical local benchmark recorded 116/120 successful executions (40 tasks, three repeats each; 96.7%); failures were in multi-step tasks.
* A finite authored adversarial suite reported 66/66 cases blocked. This is not a universal security guarantee.
* Windows-only; some actions lack independent postcondition checks.

### [QuorumKV](https://github.com/pavann19/QuorumKV)
**Go · Raft · gRPC · WAL**
> Replicated key-value store built to explore storage, consensus and failure recovery.
* 100 crash-recovery trials with a real subprocess, checking that acknowledged writes survived abrupt termination (process kill, not power loss).
* CRC-checked, fsync-backed WAL, a real 3-process Raft cluster, custom network fault injection, and client histories from five scenarios checked with Porcupine.
* No successful 24-hour or multi-host run is claimed.

### [Gatekeeper](https://github.com/pavann19/Gatekeeper-AI-Infrastructure-and-Governance-Gateway)
**Python · FastAPI · Redis · FAISS**
> Governance gateway that assesses prompts and outputs before they reach a language model.
* Privacy processing, input and output assessment, tenant policy, human review and audited tool execution; Redis shares configured rate limits (circuit breakers are process local).
* Evaluation notes distinguish frozen-oracle replay, model accuracy and deployment evidence; no current independent accuracy headline is published.

### [Agentic-OS](https://github.com/pavann19/Agentic-OS)
**Rust · x86_64 · UEFI · QEMU**
> Experimental capability-based OS project.
* CI covers the documented boot and capability-revocation boundary; other features have separate local or partial status.
* QEMU-only; physical hardware support remains future work.

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
