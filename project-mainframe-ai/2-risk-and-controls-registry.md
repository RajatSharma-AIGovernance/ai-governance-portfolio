# Module 2: Mainframe AI Risk & Controls Registry
*Document Reference: AI-GRC-XLS-002 | Version: 2026.1*
*Target Output Format: Microsoft Excel (.xlsx) Pivot Matrix*

**Operational Purpose:** This structural registry functions as the core control verification log required to satisfy **ISO 42001 Annex A Risk Treatment Assessments**. It highlights unique mainframe vulnerabilities that general IT risk registers miss.

---

### Master Risk Ledger (Public Preview)

| Risk ID | System Component | Hazard Scenario / Threat Analysis | Initial Risk Score | Mandatory Technical Mitigation Control | Residual Risk Score |
| :--- | :--- | :--- | :---: | :--- | :---: |
| **MF-R-001** | **Network Perimeter** | **Off-Platform Data Leakage:** Subsystems pass plaintext transaction fields to public cloud LLM instances for automated processing, creating a direct regulatory breach. | 🔴 Critical | **AT-TLS & Field-Level Tokenization:** Configure Application Transparent Transport Layer Security (AT-TLS) on all outbound connections. Mandate format-preserving tokenization on all core alphanumeric blocks before network transmission. | 🟢 Low |
| **MF-R-002** | **DevOps Pipeline** | **Legacy Code Hallucination:** Code assistants output syntactically functional but structurally flawed legacy language code (COBOL copybooks) that creates infinite loops or memory allocation leaks in high-volume transaction monitors. | 🔴 High | **Dual-Gate SAST & Expert Architectural Vetting:** Implement automated static application security testing (SAST) customized for mainframe structures. Enforce a mandatory double-blind human review process and compiler sanity testing by a designated Systems Expert. | 🟡 Medium |
| **MF-R-003** | **Operating System** | **Transaction Queue Deprivation:** Computationally heavy deep learning neural network inference models executing natively on system consume excessive clock cycles, starving core real-time transactional queues (CICS / IMS). | 🟡 Medium | **Workload Manager (WLM) Enclave Isolation:** Restrict all AI execution runtimes to lower-tier, discretionary service classes via z/OS Workload Manager (WLM) profiles, ensuring real-time operational capacity is preserved. | 🟢 Low |

---

## 🔒 Access the Full Interactive Excel Matrix
The complete, production-grade **Microsoft Excel (.xlsx)** version of this control framework is hosted inside the secure private repository. The premium file features:
* **Dynamic Risk Calculators:** Automated formulas that instantly compute residual risk levels based on impact and likelihood metrics.
* **Complete Audit Trail Fields:** Columns pre-configured for control ownership mapping, testing frequencies, and evidence collection mapping.
* **GRC System Readiness:** Clean layouts optimized for immediate CSV import into enterprise tools (ServiceNow, Archer).

To request private access or schedule a walkthrough of the functional risk model, message **Rajat Sharma** directly via **sharma.rajat.work@gmail.com** or follow on **[LinkedIn](https://linkedin.com/in/rajat-sharma-pm/)**.
