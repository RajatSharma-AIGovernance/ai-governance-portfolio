# Module 1: Mainframe AI System Profile & Boundaries Questionnaire
*Document Reference: AI-GRC-TPL-001 | Version: 2026.1*
*Target Output Format: Microsoft Word (.docx) / Corporate PDF Intake Form*

**Instructions for Completion:** This comprehensive intake questionnaire is a mandatory filing under **ISO 42001 Clause 8.2**. It must be completed jointly by the Project Lead Engineer and the Infrastructure Director before any computing resources are provisioned.

---

## 1. PROJECT & BUSINESS CONTEXT METADATA
* **1.1 Project Reference Identifier:** ______________________________________
* **1.2 Core Department/Business Unit:** ______________________________________
* **1.3 Primary Business Sponsor Name & Email:** ______________________________________
* **1.4 Technical Project Lead Name & Title:** ______________________________________

---

## 2. DETAILED AI ENGINE & ARCHITECTURAL TOPOLOGY
* **2.1 Underlying AI/ML Model Classification:**
  * [ ] Foundation Model / Large Language Model (e.g., Code Customizer, Code Assistant)
  * [ ] Predictive Analytics / Machine Learning Model (e.g., Deep Learning Fraud Scoring)
* **2.2 Runtime Execution Infrastructure:**
  * [ ] Native On-Chip Acceleration (e.g., IBM z16 Telum on-chip AI subsystem)
  * [ ] Dedicated Mainframe Linux Partition (zCX / Linux on Z Container Environment)
  * [ ] External Hybrid Cloud Environment (Connected via secure network endpoints)

---

## 3. LEGACY INTEGRATION MATRIX & SUB-SYSTEM CONNECTIVITY
Identify every legacy transactional ecosystem and database layer that will ingest data from, or feed raw parameters to, the proposed AI system:

| Legacy Sub-System | Data Flow Direction | Connection Method (API / Batch / MQ) | Maximum Expected Latency Tolerance |
| :--- | :--- | :--- | :--- |
| **CICS** (Customer Information Control System) | [ ] Inbound  [ ] Outbound | | |
| **DB2** (Relational Mainframe Database) | [ ] Inbound  [ ] Outbound | | |

---

## 4. REGULATORY DATA FOOTPRINT & RESIDENCY AUDIT
* **4.1 Regulated Data Categories Processed:** *(Check all that apply)*
  * [ ] PCI-DSS Bound Credit Cardholder Data (PAN, CVV)
  * [ ] GDPR / CCPA Personal Data Strings (Names, Government IDs, Account Numbers)
* **4.2 Data Residency Declarations:** 
  * State the exact geographic country/region where the AI model weights are hosted: ___________________

---

## 🔒 Access the Enterprise Toolkit Document
The functional, styled **Microsoft Word (.docx)** version of this template—fully configured with corporate branding, extended infrastructure fields, and a comprehensive pre-filled mock example—is restricted to the private enterprise repository.

To obtain access or request a customized implementation framework for your organization, please contact **Rajat Sharma** via **sharma.rajat.work@gmail.com** or connect on **[LinkedIn]([https://linkedin.com](https://www.linkedin.com/in/rajat-sharma-pm/))**.
