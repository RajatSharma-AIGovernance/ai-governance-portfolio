# The Ultimate OWASP Foundational Systems Manual

Welcome to the central knowledge hub for software and systems security. This master document outlines the entire ecosystem of the **Open Worldwide Application Security Project (OWASP)**. It explains what OWASP is, how it helps corporate governance, maps all major security dimensions in a master table, and routes you to technical sub-pages for deep-dive execution.

---

## 🏛️ Module 1: What is OWASP and Why Does Governance Need It?

### What is OWASP?
The **Open Worldwide Application Security Project (OWASP)** is a global, community-driven non-profit foundation that acts as the world’s leading authority on software security. OWASP produces free, open-source documentation, tools, and frameworks designed to help organizations build, buy, and maintain secure software systems.

### How It Helps Corporate Governance & Compliance
Process standards (like ISO/IEC 42001) establish management frameworks, policies, and committees. However, auditors and regulators cannot use an abstract policy to stop an active hacker. 
* **The Bridge to Execution:** OWASP translates high-level corporate policies into concrete engineering check-points.
* **Audit and Assurance:** Implementing OWASP standards allows an organization to formally prove to financial regulators (like the HKMA or global banks) that their infrastructure is physically defended against data breaches and code exploits.

---

## 🗺️ Module 2: The Core OWASP Ecosystem Matrix

OWASP structures its security frameworks into distinct tracking matrices based on the architectural layer being built or audited. Below is the master matrix mapping all core OWASP focus areas, their tracking codes, and their sub-page documentation paths.

| Security Layer | Framework / Standard | Alphanumeric Codes | Target Environment (What it protects) | Operational Sub-Page Link |
| :--- | :--- | :--- | :--- | :--- |
| **1. The Intelligence Layer** | **OWASP Top 10 for LLM Applications** | `LLM01` to `LLM10` | Input windows, model prompts, and retrieval-augmented generation pipelines (RAG). | 📂 **[View AI Deep Dive](./owasp-ai-security-manual.md)** |
| **2. The Autonomous Layer** | **OWASP Top 10 for GenAI & AI Agents** | `AGE01` to `AGE10` | Multi-step agentic execution loops, automated tools, and agent communication. | 📂 **[View AI Deep Dive](./owasp-ai-security-manual.md)** |
| **3. The Interconnection Layer** | **OWASP API Security Top 10** | `API1` to `API10` | Application Programming Interfaces—the digital bridges connecting models to backend data. | 📌 *See Module 4 Below* |
| **4. The Front-End Layer** | **OWASP Top 10 Core (Web Apps)** | `A01` to `A10` | Main user portals, dashboards, web authentication systems, and database inputs. | 📌 *See Module 3 Below* |
| **5. The Infrastructure Layer** | **OWASP Cloud-Native Security Top 10**| `CNAS1` to `CNAS10`| Cloud environments (AWS/Azure), container engines (Docker), and serverless environments. | 📌 *See Module 5 Below* |

---

## 🌐 Module 3: OWASP Top 10 Core (Web Application Security Overview)

The foundational standard for general web systems. If your web dashboard is vulnerable, attackers can bypass your entire AI governance pipeline.

* **A01: Broken Access Control:** Users accessing data or server paths outside their privilege tier. *(Example: A regular user viewing someone else's private prompt history).*
* **A02: Cryptographic Failures:** Data in transit or at rest being stored unencrypted. *(Example: Transmitting API keys over insecure plain text channels).*
* **A03: Injection:** Passing unvalidated user strings into text interpreters. *(Example: SQL injection attacks that leak an entire backend user database).*
* **A04: Insecure Design:** Architecture flaws created due to a lack of threat-modeling before writing code.
* **A05: Security Misconfiguration:** Leaving default setup credentials, unpatched software, or open server debug ports.
* **A06: Vulnerable and Outdated Components:** Building applications using old open-source code libraries that have public exploits.
* **A07: Identification and Authentication Failures:** Weak password rules or broken session-token handling.
* **A08: Software and Data Integrity Failures:** Utilizing plugins or code updates without running cryptographic signature verifications.
* **A09: Security Logging and Monitoring Failures:** Failing to log critical user actions, making it impossible to detect or investigate a live breach.
* **A10: Server-Side Request Forgery (SSRF):** Forcing a web application to fetch data from an unauthorized internal backend source.

---

## 🔌 Module 4: OWASP API Security Top 10 Overview

Modern technology stacks interact almost exclusively via APIs. If your digital bridges are weak, your data supply chain collapses.

* **API1: Broken Object Level Authorization (BOLA):** API endpoints exposing records without validating if the requester owns them.
* **API2: Broken Authentication:** Attackers exploiting weak API tokens to masquerade as legitimate internal services.
* **API3: Broken Object Property Level Authorization:** Exposing sensitive internal model variables through default endpoint return values.
* **API4: Unrestricted Resource Consumption:** Lacking rate limits, letting automated scripts flood endpoints and spike cloud compute bills.
* **API5: Broken Function Level Authorization:** Regular users invoking administrative API paths to change configuration maps.
* **API6: Unrestricted Access to Sensitive Business Flows:** Automated bots exploiting APIs to execute mass processes (like bulk scraping data).
* **API7: Server-Side Request Forgery (SSRF) in APIs:** Tricking internal API loops into reaching untrusted public networks.
* **API8: Security Misconfiguration in APIs:** Exposing detailed code-level error traces to public users during a system crash.
* **API9: Improper Inventory Management:** Leaving forgotten, unpatched beta or legacy versions of APIs exposed to the internet.
* **API10: Unsafe Consumption of APIs:** Trusting data received from third-party vendor APIs without running strict input sanitization.

---

## ☁️ Module 5: OWASP Cloud-Native Application Security Top 10 Overview

Securing applications deployed in highly elastic cloud infrastructure, microservice environments, and system container fabrics.

* **CNAS1: Cloud Infrastructure Misconfiguration:** Weak access settings inside your cloud control panel. *(Example: Leaving an AWS S3 bucket containing raw model training data open to the public).*
* **CNAS2: Insecure Container Images:** Deploying applications using pre-packaged runtime environments that contain pre-installed vulnerabilities.
* **CNAS3: Lack of Structured Cloud-Native Logging:** Missing infrastructure traces, leaving cloud administrators blind during an operational incident.
* **CNAS4: Over-Privileged Microservice Access Profiles:** Granting wide system permissions to small system sub-modules that only require local execution parameters.
* **CNAS5: Insecure Secret Management:** Hardcoding system encryption keys or API tokens directly inside the application source code files.
* **CNAS6: Weak Container Isolation Boundaries:** Flaws in runtime separation that allow an attacker to escape an isolated application container and touch the host OS.
* **CNAS7: Insecure Cloud Networking Topologies:** Permitting wide microservice communication routes without internal firewalls or mutual authentication tokens.
* **CNAS8: Insecure Serverless Function Architectures:** Deploying serverless hooks without setting input boundaries or maximum timeout limits.
* **CNAS9: Outdated Infrastructure-as-Code (IaC) Templates:** Utilizing outdated server setup scripts that configure vulnerable infrastructure networks by default.
* **CNAS10: Supply Chain Risks in Cloud Orchestration:** Integrating unverified third-party cloud orchestration plugins into core management panels.
