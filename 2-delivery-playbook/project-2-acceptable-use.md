# Project 2: Enterprise Generative AI Acceptable Use Policy

## 1. Executive Summary & Objective
With the rapid emergence of consumer-facing Large Language Models (LLMs), organizations face significant legal, privacy, and intellectual property exposure. Employees frequently input proprietary source code or confidential client data into public models. This policy establishes the boundaries for acceptable use of Generative Artificial Intelligence (GenAI) across the enterprise workforce.

---

## 2. Policy Scope
This policy applies to all full-time employees, part-time employees, contractors, and third-party vendors operating on behalf of the company. It governs the use of all text, image, code, and audio generation tools.

---

## 3. Permitted vs. Prohibited Activities

### 🟢 Permitted Workflows (Low-Risk Data)
* **Drafting Assistance:** Using enterprise-approved tools to draft emails, generate standard marketing copy, or summarize open-source industry articles.
* **Brainstorming:** Generating structural outlines for internal presentations or testing conversational ideas using public data.
* **Refactoring Code:** Using local or corporate-licensed IDE autocomplete plugins on open-source or non-proprietary code segments.

### 🔴 Strictly Prohibited Workflows (High-Risk/Severe Risk)
* **PII Exfiltration:** Pasting customer or employee Personally Identifiable Information (PII) into unvetted, consumer-grade public tools (e.g., free tiers of ChatGPT/Claude).
* **Intellectual Property Input:** Uploading proprietary software code, trade secrets, unreleased financial reports, or pending legal strategy documents into external training datasets.
* **Automated Decision-Making:** Using AI output to directly execute hiring decisions, performance evaluations, or customer contract terminations without mandatory human review.

---

## 4. The Data Handling Matrix
To ensure compliance with corporate data protection policies, all employees must reference the following guidelines prior to inputting information into any GenAI tool:

| Corporate Data Classification | Consumer GenAI Tools (Free Tier) | Enterprise GenAI Tools (Corporate Account) | Approved Action Required |
| :--- | :--- | :--- | :--- |
| **Public Data** (Press releases, etc.) | Allowed | Allowed | None |
| **Internal Only** (Meeting notes, etc.) | **Prohibited** | Allowed | Ensure data retention is disabled |
| **Restricted PII** (Health/Financials) | **Prohibited** | **Prohibited** | Requires AI Governance Board Waiver |
| **Source Code** (Core business IP) | **Prohibited** | Allowed | Use authorized corporate code assistants |

---

## 5. Human-in-the-Loop (HITL) Requirement
All AI-generated content intended for external distribution or client delivery must undergo strict manual verification. 

```text
[ AI Generated Draft ] ──> [ Mandatory Human Review ] ──> [ Sign-Off & Distribution ]
                                     │
                                     └── Verification Checklist:
                                         • Check for factual hallucinations
                                         • Validate source data authenticity
                                         • Inspect for algorithmic bias
```

* **Hallucination Checking:** Requestors are individually liable for verifying the factual accuracy of any technical or regulatory data produced by an LLM.
* **Plagiarism and Bias Scans:** Content must be audited to ensure it does not explicitly recreate copyrighted material or output discriminatory language.

---

## 6. Enforcement & Compliance Audits
Compliance with this policy is continuously audited using network data-loss prevention (DLP) filters. Violations may result in formal disciplinary action up to and including termination of contract or employment.
