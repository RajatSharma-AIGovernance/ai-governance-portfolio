# Project 4: Algorithmic Impact Assessment (AIA) – Automated Hiring System

## 1. Executive Summary & System Profile
* **System Under Assessment:** TalentScout AI (Automated Resume Screening Engine)
* **Objective:** Automatically sort, rank, and filter inbound job applicant resumes to recommend top-tier candidates to hiring managers.
* **Core Technology:** Natural Language Processing (NLP) embedding models trained on historical company hiring data.
* **Framework Alignment:** IAPP AIGP Ethical Principles and ISO/IEC 42001 Clause 6.1.2 (AI Risk Assessment Process).

---

## 2. Stakeholder & Impact Mapping
Before assessing risks, the impacted parties must be mapped to ensure fairness across all touchpoints:

```text
┌────────────────────────┐      ┌────────────────────────┐      ┌────────────────────────┐
│    Job Applicants      │ ───> │    Hiring Managers     │ ───> │  Legal & Compliance    │
├────────────────────────┤      ├────────────────────────┤      ├────────────────────────┤
│ High Risk: Systemic    │      │ Med Risk: Over-reliance│      │ High Risk: Regulatory  │
│ bias or false rejection│      │ on tool (automation)   │      │ penalties & lawsuits   │
└────────────────────────┘      └────────────────────────┘      └────────────────────────┘
```

---

## 3. Risk Identification & Mitigation Register

### Risk 1: Algorithmic Bias & Discriminatory Filtering
* **Description:** The system learns from historical company hiring data. If past hiring trends favored a specific demographic, the model will unintentionally penalize resumes containing words associated with minority groups or female applicants (e.g., "women's college").
* **Initial Risk Level:** 🔴 High
* **Mitigation Strategy:** 
  1. **Data Pre-processing:** Strip names, gender markers, zip codes, and graduation years before text embeddings are processed.
  2. **Synthetic Data Balancing:** Train the model using a demographic-parity balanced dataset.
* **Residual Risk Level:** 🟡 Medium

### Risk 2: Automation Bias & Lack of Human Oversight
* **Description:** Recruiter teams stop reading resumes entirely, blindly trusting the AI's top 10 rankings without questioning errors or hallucinations.
* **Initial Risk Level:** 🔴 High
* **Mitigation Strategy:**
  1. **Mandatory Audit Sample:** Require recruiters to manually review a random 10% sample of "rejected" resumes weekly to test system accuracy.
  2. **Score Transparency:** Display an explanation alongside the rank (e.g., "Matched 4/5 required skills listed in job post").
* **Residual Risk Level:** 🟢 Low

### Risk 3: Lack of Transparency & Explanability
* **Description:** Job applicants are rejected by an automated system without receiving a rationale, violating core principles of algorithmic transparency.
* **Initial Risk Level:** 🟡 Medium
* **Mitigation Strategy:**
  1. **Automated Notification:** Configure system to send a high-level automated reason upon rejection (e.g., "Candidate lacked mandatory certification requirement").
  2. **Opt-Out Path:** Provide a mechanism for applicants to request a manual human review if they contest the AI's baseline decision.
* **Residual Risk Level:** 🟢 Low

---

## 4. Continuous Monitoring Plan (ISO 42001 Alignment)
To maintain alignment with ISO 42001 performance evaluation criteria, the system must undergo quarterly testing:

| Assessment Interval | Metric Tested | Testing Methodology | Threshold for Action |
| :--- | :--- | :--- | :--- |
| **Quarterly** | Demographic Parity | Apply the Four-Fifths Rule across protected demographic classes | Selection rate falls below 80% for any group |
| **Bi-Annually** | Drift Analysis | Evaluate if new job description styles degrade the model's accuracy | True-positive ranking drops by >5% |
| **Annually** | External Audit | Third-party independent model evaluation and bias review | Mandatory before enterprise license renewal |

---

## 5. Governance Sign-Off & Verdict
* **Final Compliance Recommendation:** Approved for conditional deployment with automated stripping of PII and mandatory quarterly bias audits.
* **Assessor:** AI Governance & Compliance Team
