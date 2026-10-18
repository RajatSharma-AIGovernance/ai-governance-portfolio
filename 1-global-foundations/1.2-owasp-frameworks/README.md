# OWASP Frameworks Master Landing Page Index

> **🗂️ Document Control Reference**
> * **Framework Index:** REG-SEC-1.2.0
> * **Current Version:** v2.0 (Subdirectory README Integration)
> * **Last Operational Review:** October 2026
> * *Note: Subject to the master legal disclaimer located in the repository root [README.md](../../README.md).*

---

## 🏛️ Module 1: What is OWASP and Why Does AI Governance Need It?

### What is OWASP?
The **Open Worldwide Application Security Project (OWASP)** is a global, community-driven non-profit foundation that acts as the world’s leading authority on software security. OWASP produces open-source documentation, threat matrices, and defensive baselines designed to help organizations secure their software systems.

### The Role in AI Governance
Process standards (like ISO/IEC 42001) establish policies, committees, and compliance records, but they cannot stop a technical attack at runtime. This manual bridges the gap between high-level process compliance and engineering security execution. It organizes the entire ecosystem of specialized OWASP vulnerability frameworks into a unified, layer-by-layer technical audit blueprint.

---

## 🛡️ Module 2: The Enterprise AI Vulnerability Domain Matrix

To audit or secure an AI system, AppSec teams must evaluate six distinct layers of the application footprint. Below is the centralized index mapping every focus domain, its official tracking codes, and its dedicated deep-dive implementation manual within this sub-directory.

| Operational Layer | Framework / Standard | Control Codes | Target Environment (What it protects) | Dedicated Deep-Dive Manual |
| :--- | :--- | :--- | :--- | :--- |
| **1. Core Language Layer** | **OWASP Top 10 for LLM Applications** | `LLM01` to `LLM10` | Core prompt windows, input text blocks, and retrieval-augmented generation (RAG) pipelines. | 📂 **[Read 1.2.1 - LLM Security Manual](./1.2.1-owasp-LLM-security-manual.md)** |
| **2. Autonomous Layer** | **OWASP Top 10 for AI Agents** | `AGE01` to `AGE10` | Multi-step agentic execution loops, automated background tools, and inter-agent coordination tokens. | 📂 **[Read 1.2.2 - Agentic Systems Manual](./1.2.2-owasp-agentic-systems.md)** |
| **3. Core Mathematical Layer**| **OWASP Machine Learning Security** | `ML01` to `ML10` | Mathematical array models, data science classifiers, training weights, and tensor registries. | 📂 **[Read 1.2.3 - ML Security Manual](./1.2.3-owasp-ml-security-manual.md)** |
| **4. Integration Layer** | **OWASP API Security Top 10** | `API1` to `API10` | Application Programming Interfaces—the data transit bridges connecting models to backend databases. | 📂 **[Read 1.2.4 - API Security Manual](./1.2.4-owasp-api-security-manual.md)** |
| **5. User Interface Layer** | **OWASP Top 10 Core (Web Apps)** | `A01` to `A10` | Main consumer portal frontends, browser authentication interfaces, and client screens. | 📂 **[Read 1.2.5 - Web Security Manual](./1.2.5-owasp-web-security-manual.md)** |
| **6. Infrastructure Layer** | **OWASP Cloud-Native Security** | `CNAS1` to `CNAS10`| Distributed cloud instances (AWS/Azure), container ecosystems (Docker), and serverless execution frames. | 📂 **[Read 1.2.6 - Cloud-Native Manual](./1.2.6-owasp-cloud-security-manual.md)** |

---

## 🧭 Module 3: Technical Ingestion Scoping Guidelines

When executing downstream stage-gate checklists inside the **Enterprise AI Operating Model**, delivery leads use this index to target their engineering scans:
1. **For Technical Prompt & Agentic Audits:** Cross-reference system prompts and fine-tuning pools against **[Document 1.2.1](./1.2.1-owasp-LLM-security-manual.md)** and investigate autonomous tool execution loops via **[Document 1.2.2](./1.2.2-owasp-agentic-systems.md)**.
2. **For Core Deep Learning Math Reviews:** Audit tensor assets and dataset pipeline integrity parameters using **[Document 1.2.3](./1.2.3-owasp-ml-security-manual.md)**.
3. **For Pipeline and Access Token Validation:** Audit data hooks and connection variables traversing backend integration pipelines using **[Document 1.2.4](./1.2.4-owasp-api-security-manual.md)**.
4. **For Container Hosting & Portal Hardening:** Enforce strict zero-trust parameters over frontend applications and container infrastructure deploying workloads by auditing against **[Document 1.2.5](./1.2.5-owasp-web-security-manual.md)** and **[Document 1.2.6](./1.2.6-owasp-cloud-security-manual.md)**.
