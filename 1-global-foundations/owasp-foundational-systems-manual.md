# The Core OWASP Foundational Systems Manual

An AI application sits on servers, connects to cloud pipelines, and interacts with traditional user portals. This companion manual breaks down the three foundational software security frameworks that secure the underlying enterprise infrastructure wrapping around AI models.

---

## 🌐 1. OWASP Top 10 Core (Web Application Security)
* **What it is:** The global standard list of the most critical security vulnerabilities for web software.
* **Why it matters for AI:** If a hacker can bypass your main login screen or inject code into your regular user web page, they can easily reach and compromise your underlying AI modules without needing to hack the AI itself.
* **Critical Control Points:**
  * **A01: Broken Access Control:** Users accessing data or paths they shouldn't. *(In AI: A customer exploiting a website bug to view another customer's private prompt history).*
  * **A05: Security Misconfiguration:** Leaving default setup passwords, unpatched systems, or open debug ports. *(In AI: Forgetting to put a password on your raw Vector Database server panel).*
  * **A06: Vulnerable and Outdated Components:** Building software using old code libraries. *(In AI: Using an outdated open-source machine learning library that has a known remote execution exploit).*

---

## 🔌 2. OWASP API Security Top 10
* **What it is:** A specialized list focusing on flaws in Application Programming Interfaces (APIs)—the digital bridges that software programs use to talk to each other.
* **Why it matters for AI:** Large Language Models and agents are completely dependent on APIs. Whether you pull data from a database into a RAG pipeline or connect an Agent to an external tool, you are using APIs. If the API is weak, the entire AI chain breaks.
* **Critical Control Points:**
  * **API1: Broken Object Level Authorization (BOLA):** An API endpoint leaks user data because it doesn't verify if the person requesting a specific ID owns it. *(In AI: An agent fetches data via `api/get_profile?id=999` without verifying if user 999 sent the request).*
  * **API4: Unrestricted Resource Consumption:** Allowing unlimited data requests to hit an API hook, leading to system crashes. *(In AI: A script spamming an LLM API endpoint, blowing past rate limits, and draining your cloud compute budget).*

---

## ☁️ 3. OWASP Cloud-Native Application Security Top 10
* **What it is:** A framework for evaluating security risks in cloud environments, microservices, container structures (like Docker), and serverless code.
* **Why it matters for AI:** Modern enterprise AI models and databases are built, fine-tuned, and scaled across cloud networks (like AWS). 
* **Critical Control Points:**
  * **CNAS1: Cloud Infrastructure Misconfiguration:** Weak settings in your cloud management panel. *(In AI: Leaving an AWS S3 bucket containing raw corporate training datasets wide open to the public internet).*
  * **CNAS3: Insecure Container Images:** Running microservices inside infected or unvetted system containers. *(In AI: Deploying an AI tool inside a Docker container image that has pre-installed malware hidden in its base operating layer).*
