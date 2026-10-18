# Section 1 — Global AI Governance Foundations

> **🗂️ Document Control Reference**
> * **Framework Index:** REG-SEC-1.0
> * **Current Version:** v1.2
> * **Last Operational Review:** October 2026
> * *Note: All materials in this directory are strictly subject to the master legal disclaimer located in the repository root [README.md](../README.md).*

---

To build a secure and legally compliant Enterprise AI Management System, a governance leader must look at the landscape through three distinct lenses: **Process Management**, **Regulatory Compliance**, and **Technical Vulnerability Defense**. 

This master matrix connects these worlds, showing you exactly which framework to use depending on the problem you are trying to solve.

---

## 🗺️ The Global AI Governance Landscape

| Framework / Standard | Core Focus Domain | Best Used For... | Operational Detailed Deep Dive |
| :--- | :--- | :--- | :--- |
| **ISO/IEC 42001 (AIMS)** | **Process & Operations** | Designing internal corporate policies, logging system inventories, and enforcing company-wide AI risk lifecycles. | 📂 **[Read 1.2 - ISO 42001 Manual](./1.2-iso-42001-translation-manual.md)** |
| **OWASP Core & AI Suite** | **Technical & Cyber Security** | Auditing engineering teams to ensure applications are protected against web exploits, broken APIs, prompt injection, and rogue autonomous loops. | 📂 **[Read 1.3 - OWASP Foundational Hub](./1.3-owasp-foundational-systems-manual.md)** |
| **NIST AI RMF 1.0** | **Risk Assessment Culture** | Aligning corporate, engineering, and legal teams to measure model trustworthiness traits like bias, reliability, and explainability. | 📂 **[Read 1.4 - NIST AI RMF Manual](./1.4-nist-rmf-translation-manual.md)** |
| **Regional Regulatory Laws** | **Hard Legal Compliance** | Classifying models into legal risk tiers and avoiding multi-million dollar regulatory fines across international markets. | 🗂️ **[Go to Section 2: Regional Regulations](../2-regional-regulations/)** |

---

## 🧭 How to Choose Your Starting Framework

### 1. Are you setting up the corporate infrastructure?
* **Use:** **ISO/IEC 42001**
* **Why:** It provides the structural scaffolding. It tells you *how* to set up the committees, *how* to mandate logs, and *how* to force teams to report their models.

### 2. Are you evaluating a model's trustworthiness?
* **Use:** **NIST AI RMF (Govern, Map, Measure, Manage)**
* **Why:** It focuses heavily on the human and systemic elements of trust—ensuring a model is reliable, safe, explainable, and free from dangerous bias loops.

### 3. Are you checking code security across systems?
* **Use:** **The OWASP Ecosystem Hub**
* **Why:** Compliance laws don't stop hackers. You need the **[OWASP Central Hub](./1.3-owasp-foundational-systems-manual.md)** to route your development teams to specific checklists protecting your systems:
  * 🌐 **[1.3.1 - OWASP AI Security Manual](./1.3.1-owasp-ai-security-manual.md)**: Mitigating LLM-specific vulnerabilities, core prompt injection risks, and pipeline vulnerabilities.
  * ⚙️ **[1.3.2 - OWASP API Security Manual](./1.3.2-owasp-api-security-manual.md)**: Securing data transit endpoints and token hooks connecting to model services.
  * 💻 **[1.3.3 - OWASP Web Security Manual](./1.3.3-owasp-web-security-manual.md)**: Hardening legacy frontend user interfaces rendering AI outputs.
  * ☁️ **[1.3.4 - OWASP Cloud Security Manual](./1.3.4-owasp-cloud-security-manual.md)**: Safeguarding the underlying host infrastructure and virtual cloud environments.
  * 🤖 **[1.3.5 - OWASP Agentic Systems Manual](./1.3.5-owasp-agentic-systems.md)**: Managing vulnerabilities specific to autonomous agency, tool execution loops, and inter-agent synchronization.
  * 🔢 **[1.3.6 - OWASP ML Security Manual](./1.3.6-owasp-ml-security-manual.md)**: Defending core model weights, array math, data poisoning vectors, and registry storage layers.
  * 📦 **[1.5 - AI Software Supply Chain Provenance Manual](./1.5-ai-supply-chain-provenance-manual.md)**: Validating AI software bills of materials (AI-SBOM), model weight serialization security, and preventing model poisoning.
  * ⚖️ **[1.6 - AI Content Provenance & Automation Bias Manual](./1.6-ai-content-provenance-automation-bias-manual.md)**: Tracking RAG / training copyright transparency boundaries and auditing human-in-the-loop cognitive friction gates.

---

## 🔗 Jurisdictional Legal Routing

While global foundations provide the operational and technical scaffolding, your systems must ultimately satisfy the hard statutory boundaries of the specific markets where they deploy. 

All country-specific compliance playbooks, legal timelines, and enforcement matrices are fully consolidated within our secondary directory:

👉 **[Go to Section 2: Regional Regulations & Handbooks](../2-regional-regulations/README.md)**
