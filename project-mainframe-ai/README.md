# Project Overview: Mainframe AI Adoption & Modernization Governance

## 1. Executive Summary
Legacy mainframe environments (such as IBM z/OS platforms) handle an organization's most critical financial transactions, customer accounts, and core operations. Incorporating AI into these high-stakes ecosystems—whether through Generative AI for COBOL-to-Java translation, or native on-chip predictive machine learning for real-time fraud detection—presents severe systemic, operational, and regulatory risks.

This project delivers a production-grade governance blueprint that operationalizes **ISO/IEC 42001** and **IAPP AIGP** guardrails specifically for mainframe computing.

---

## 2. Directory Structure & Documentation Map
This directory contains the complete lifecycle documentation set required to pass stringent enterprise risk, privacy, and regulatory audits:

* 📄 **[README.md](README.md):** Executive summary, deployment context, and directory map *(This File)*.
* 📋 **[1-system-profile-template.md](1-system-profile-template.md):** Structural Word/PDF questionnaire template defining system architectural boundaries.
* 📊 **[2-risk-and-controls-registry.md](2-risk-and-controls-registry.md):** An Excel-aligned spreadsheet template detailing mainframe-specific AI failure modes and mitigations.
* 🗺️ **[3-step-by-step-implementation-guide.md](3-step-by-step-implementation-guide.md):** An operational, 5-phase playbook for governance implementation.
* 🛡️ **[4-supplementary-iam-and-rollback-plans.md](4-supplementary-iam-and-rollback-plans.md):** Crucial contingency plans covering access controls and emergency system rollbacks.

---

## 3. High-Level AI Deployment Topologies Covered
This framework provides risk controls across three distinct mainframe-AI architectures:
1. **On-Chip Inference:** AI models running natively on mainframe hardware (e.g., IBM Telum processor) for low-latency transaction processing.
2. **Hybrid Cloud Interconnection:** Mainframe core databases (DB2, IMS) exposing transactional data to off-platform cloud-hosted LLMs via private APIs.
3. **Development Tooling / Assistants:** Code-generation assistants (e.g., watsonx Code Assistant for Z) utilized by engineers to refactor legacy codebases.
