# Project 1: AI Use-Case Intake Workflow & Inventory

## 1. Executive Summary & Objective
Organizations frequently suffer from "Shadow AI"—where employees deploy external AI tools without IT or Legal oversight. This project establishes a formalized entry gate. It forces business teams to document the *intent, data footprint,* and *risks* of an AI system before line-of-business approval.

---

## 2. The Step-by-Step Intake Lifecycle

```text
[ Business Requestor ] ──> Fills Intake Form ──> [ Preliminary Risk Tiering ]
                                                            │
  ┌─────────────────────────────────────────────────────────┴────────────────────────┐
  ▼                                                         ▼                        ▼
[ Low Risk ]                                          [ Medium Risk ]          [ High Risk ]
Auto-approved with standard guardrails                Requires Security        Requires Full Algorithmic
                                                       & Privacy Review        Impact Assessment (AIA)
```

1. **Identification:** The business unit submits the AI Intake Questionnaire.
2. **Triage:** The AI Governance Officer evaluates data types, user populations, and autonomy levels.
3. **Classification:** The system is assigned a Risk Tier (Low, Medium, High, Unacceptable).
4. **Action Registry:** The system is logged into the corporate AI Inventory for ongoing monitoring.

---

## 3. Template: AI System Procurement & Intake Form
*Deploy this form internally via Microsoft Forms, Jira Service Desk, or ServiceNow.*

### Section A: Business Owner Context
* **Project Name:** 
* **Business Sponsor & Department:** 
* **Primary Objective:** *What business problem does this AI solve?*

### Section B: Technical Architecture & Data Footprint
* **Model Deployment Type:** 
  * [ ] Third-Party SaaS (e.g., ChatGPT Enterprise, Claude Team)
  * [ ] API Integration (e.g., OpenAI API hosted on corporate Azure)
  * [ ] Proprietary / In-house trained model
* **Data Classification:** *Will this system ingest or process:*
  * [ ] Customer Personally Identifiable Information (PII)
  * [ ] Corporate Protected Intellectual Property (IP)
  * [ ] Biometric or Health Data
  * [ ] Publicly available data only

### Section C: Human-in-the-Loop (HITL) Controls
* **Autonomy Level:**
  * [ ] Fully Autonomous (AI takes action/makes decision without review)
  * [ ] Human-Assisted (AI recommends, human approves/executes)
  * [ ] Informational Only (Internal brainstorming, draft generation)

---

## 4. Internal AI Inventory Logging Matrix
Once approved, the system must be logged into a central registry with the following fields:

| System ID | Department | Model Source | Data Risk Tier | EU AI Act Classification | Next Review Date |
| :--- | :--- | :--- | :--- | :--- | :--- |
| AI-2026-001 | HR / Talent | Vendor SaaS | High (PII) | High-Risk (Employment) | 2027-01-27 |
| AI-2026-002 | Marketing | Public LLM API | Low (Public) | Minimal Risk | 2027-07-27 |
