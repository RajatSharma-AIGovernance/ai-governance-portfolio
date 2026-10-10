# Project 3: Third-Party AI Vendor Risk Assessment Questionnaire

## 1. Executive Summary & Objective
Organizations rarely build foundational AI models from scratch; instead, they integrate third-party APIs and SaaS platforms. This introduces critical third-party dependencies. This questionnaire provides a standardized vetting protocol for procurement and risk teams to evaluate an AI vendor's security, data retention policies, and alignment with **ISO/IEC 42001 (Annex A - Relationship with Stakeholders)**.

---

## 2. Vendor Information & Model Profile
* **Vendor Name:** 
* **AI Product/Service Name:** 
* **Underlying Model Architecture:** *(e.g., GPT-4o, Claude 3.5 Sonnet, Custom Fine-Tuned Llama)*

---

## 3. Core Risk Evaluation Questionnaire

### Section A: Data Governance & Privacy
* **A.1 Data Training Opt-Out:** Does your organization use our submitted text, prompts, data, or files to retrain your base models or fine-tune models for other customers?
  * *Expected Answer:* No. Confirm if data logging must be explicitly disabled via an enterprise setting or API flag.
* **A.2 Data Retention & Logging:** How long are customer prompts and generated outputs cached or stored on your servers for abuse monitoring?
  * *Expected Answer:* Maximum 30 days, or immediate deletion upon processing if zero-retention data pathways are contracted.
* **A.3 Regional Data Sovereignty:** In which geographical regions/data centers is consumer data stored and processed? 
  * *Expected Answer:* Explicit country listing to verify alignment with regional privacy laws (e.g., GDPR, CCPA).

### Section B: Model Reliability, Safety & Ethics
* **B.1 Bias and Fairness Testing:** What methodology do you use to test and mitigate demographic or systemic bias within your model's outputs?
  * *Expected Answer:* Evidence of red-teaming exercises, benchmark evaluations, or fairness audits.
* **B.2 Hallucination & Accuracy Grounding:** Does your application utilize Retrieval-Augmented Generation (RAG) or similar grounding architectures to limit factual hallucinations?
  * *Expected Answer:* Technical confirmation of context windows and source attribution features.

### Section C: Technical Security & System Vulnerabilities
* **C.1 Prompt Injection Defenses:** What internal guardrails or system prompts are implemented to prevent prompt injection and jailbreaking attempts by malicious users?
  * *Expected Answer:* Input validation layers, input filtering, and active firewalling of LLM requests.
* **C.2 Model Poisoning & Supply Chain Security:** How do you secure your training pipeline and weights against unauthorized manipulation or model poisoning?
  * *Expected Answer:* Strict cryptographic access to model checkpoints and rigorous dataset supply chain validation.

---

## 4. Vendor Compliance Evaluation Matrix
Risk officers use this scoring rubric to determine if a supplier can be safely onboarded based on questionnaire responses:

```text
[ High Risk ] ─────> Uses corporate data for training ──────> REJECT VENDOR
[ Medium Risk ] ───> Stores data > 30 days or lack RAG ─────> REQUIRES COMPLIANCE MITIGATION
[ Low Risk ] ──────> Zero data retention + active guardrails ─> APPROVE VENDOR
```

| Evaluation Domain | Risk Tier Criteria | Compliance Verdict |
| :--- | :--- | :--- |
| Data Training | Vendor uses inputs for model tuning | **Critical Block** (Unacceptable Risk) |
| System Auditing | Vendor lacks independent SOC 2 Type II or ISO 42001 | **High Risk** (Requires executive exception) |
| Safety Filtering | Vendor enforces strict automated input/output filtering | **Low Risk** (Approved for deployment) |
