# OWASP Top 10 Core: Web Application Security Manual

This manual serves as a definitive security architecture reference for client-facing software portals. It covers the complete, official list for the **OWASP Top 10 Core Web Application Vulnerabilities**, providing technical terms, tracking codes, and plain-English translation matrices.

---

## 🏛️ Module 1: What is Web Application Security and Why Does AI Governance Need It?

### What is Web Application Security?
Web application security focuses on protecting websites, browser portals, and online services from cyber exploits that seek to steal confidential data, alter code, or disrupt business continuity.

### The Role in AI Governance
The primary interface for any enterprise AI application is almost always a web portal—such as an internal corporate chat dashboard, an automated credit-scoring user pipeline, or an HR resume submission screen. If your web frontend has weak access boundaries or input logic, an attacker can bypass all AI guardrails and compromise corporate assets directly through the browser portal.

---

## 🛡️ Module 2: The Complete OWASP Top 10 Core Reference Matrix

| Official Code | Legal / Technical Security Term | Plain-English Meaning (What it is) | The Enterprise Risk (What breaks) | The Practical Defense (How to solve) |
| :--- | :--- | :--- | :--- | :--- |
| **A01:2021** | **Broken Access Control** | Users can bypass access boundaries and act outside their intended permission tiers. | A customer exploits a website navigation bug to view another customer's private account transaction logs. | Enforce strict, server-side authorization checks for every single page request. |
| **A02:2021** | **Cryptographic Failures** | Failing to protect sensitive corporate data in transit or at rest via encryption. | Transmitting user passwords or financial details over unencrypted plain text channels, exposing them to interception. | Mandate TLS 1.3 for data in transit; use strong AES-256 encryption algorithms for stored databases. |
| **A03:2021** | **Injection** | Passing raw, unchecked user text inputs straight into background code interpreters. | SQL Injection attacks where a malicious text string forces your web server to print your entire database to the screen. | Utilize parameterized queries and prepared statements; never concatenate raw inputs into database queries. |
| **A04:2021** | **Insecure Design** | Flaws created due to a lack of threat-modeling and secure architecture planning before code was written. | A application design forgets to limit retry loops, letting hackers guess passwords millions of times with zero lockouts. | Integrate security engineers into the planning phase; implement secure design patterns. |
| **A05:2021** | **Security Misconfiguration** | Leaving system defaults, unnecessary features, or default admin accounts active on production servers. | Forgetting to change the default software password (`admin`/`admin`) on an internal corporate monitoring dashboard. | Automate infrastructure setup using secure hardening scripts; remove unused software features. |
| **A06:2021** | **Vulnerable & Outdated Components** | Building applications using open-source libraries or plugins that have known security flaws. | A developer utilizes an old web framework package that has a public exploit, allowing hackers to execute code remotely. | Run automated dependencies checks (SCA); patch software versions regularly. |
| **A07:2021** | **Identification & Authentication Failures** | Weak identity defenses that let attackers brute-force accounts or hijack user sessions. | Attackers use credential-stuffing automated scripts to guess passwords and take over client profiles. | Enforce strong password complexity rules; implement rate limiting on logins and mandate MFA. |
| **A08:2021** | **Software & Data Integrity Failures** | Relying on code libraries, plugins, or software updates without verifying their source or signature. | A third-party software update server gets hacked, sending a corrupted, malicious plugin update directly onto your machine. | Verify digital signatures (hashes) for all imported plugins and software updates. |
| **A09:2021** | **Security Logging & Monitoring Failures** | Failing to record or analyze critical application events, keeping security teams blind to attacks. | A hacker spends weeks quietly stealing files from your network because no alerts were generated to warn administrators. | Implement unified log streaming; configure automated real-time alerts for high-risk system events. |
| **A10:2021** | **Server-Side Request Forgery (SSRF)** | A web application is tricked into sending an unauthorized request to internal cloud networks. | An attacker inputs a local server address into a public file-uploader feature, forcing the server to leak internal configuration data. | Strict validation on user-supplied URLs; implement network segmentation to isolate backend servers. |
