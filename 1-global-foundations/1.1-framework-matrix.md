# The Master AI Governance Framework Matrix

To build a secure and legally compliant Enterprise AI Management System, a governance leader must look at the landscape through three distinct lenses: **Process Management**, **Regulatory Compliance**, and **Technical Vulnerability Defense**. 

This master matrix connects these worlds, showing you exactly which framework to use depending on the problem you are trying to solve.

---

## 🗺️ The Global AI Governance Landscape

| Framework / Standard | Core Focus Domain | Best Used For... | Detailed Deep Dive |
| :--- | :--- | :--- | :--- |
| **ISO/IEC 42001 (AIMS)** | **Process & Operations** | Designing the internal policies, tracking system inventories, and building company-wide AI risk lifecycles. | 🔹 **[ISO 42001 Translation Manual](./iso-42001-translation-manual.md)** |
| **NIST AI RMF 1.0** | **Risk Assessment Culture** | Getting corporate, engineering, and legal teams to speak the same language when measuring model trustworthiness. | 🟡 *Handbook Under Construction* |
| **EU AI Act & GDPR** | **Hard Legal Compliance** | Classifying models into strict risk tiers and avoiding multi-million dollar regulatory fines in the European market. | 🗂️ **[Go to Regional Handbooks](../3-regional-handbooks/)** |
| **OWASP Top 10 for LLMs** | **Technical & Cyber Security** | Auditing engineering teams to ensure applications are protected against code-level exploits like prompt injection and data leaks. | 🟡 *Handbook Under Construction* |

---

## 🧭 How to Choose Your Starting Framework

### 1. Are you setting up the corporate infrastructure?
* **Use:** **ISO/IEC 42001**
* **Why:** It provides the structural scaffolding. It tells you *how* to set up the committees, *how* to mandate logs, and *how* to force teams to report their models.

### 2. Are you evaluating a model's trustworthiness?
* **Use:** **NIST AI RMF (Govern, Map, Measure, Manage)**
* **Why:** It focuses heavily on the human and systemic elements of trust—ensuring a model is reliable, safe, explainable, and free from dangerous bias loops.

### 3. Are you building applications like LLMs, RAG, or AI Agents?
* **Use:** **OWASP Top 10 for LLMs / GenAI**
* **Why:** Compliance laws don't stop hackers. You need OWASP to audit technical flaws like **Prompt Injection**, **Insecure Output Handling**, and **System Overreliance** across the different layers of your deployment (the model layer, the agentic orchestration layer, and the data pipeline layer).
