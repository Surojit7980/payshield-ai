\# 🛡️ PayShield AI — Autonomous PayPal Dispute \& Chargeback Defense Engine



\*\*PayShield AI\*\* is an autonomous merchant revenue-defense engine built for the \*\*PayPal AI Hackathon 2026\*\*. It connects directly to the \*\*PayPal Sandbox REST APIs\*\* (`Orders v2` \& `Customer Disputes v1`), validates agentic API payloads via \*\*APIMatic MCP (OpenAPI 3.0 Context)\*\*, and provides real-time financial triage inside an \*\*AG Grid + AG Studio AI\*\* command center.



\## 🚀 Key Capabilities

1\. \*\*Live PayPal Sandbox Integration:\*\* Authenticates via PayPal OAuth 2.0 (`/v1/oauth2/token`), creates and inspects live orders (`/v2/checkout/orders`), and monitors merchant disputes (`/v1/customer/disputes`).

2\. \*\*Fee-Waiver Micro-Dispute Triage (<$25 Policy):\*\* Automatically detects when fighting a low-value dispute costs more in PayPal dispute fees ($15.00) than the transaction itself, routing to `POST /v1/customer/disputes/{id}/accept-claim` to waive the $15 fee.

3\. \*\*Cryptographic PDF Evidence Dossier Generator:\*\* For high-value claims (>$25), cross-verifies carrier delivery signatures and IP/session telemetry, compiles a downloadable PDF-1.4 legal evidence packet, and prepares `POST /v1/customer/disputes/{id}/provide-evidence`.

4\. \*\*AG Grid + AG Studio AI Lenses:\*\* Interactive dark-mode financial matrix with instant AI triage filters, live KPI reconciliation, and 1-click autonomous execution.



\## 🛠️ Tech Stack \& Sponsor Integrations

\- \*\*PayPal Developer Platform:\*\* Sandbox OAuth 2.0, Orders v2 API, Customer Disputes v1 API

\- \*\*AG Grid \& AG Studio:\*\* Custom Quartz Dark financial telemetry grid \& AI view lenses

\- \*\*APIMatic MCP:\*\* Strict OpenAPI 3.0 schema \& scope registry for agentic PayPal calls

\- \*\*Backend \& Runtime:\*\* Node.js Zero-Dependency HTTP Engine + Native PDF-1.4 Generator

\- \*\*Cloud Hosting:\*\* Render Web Service



\## ⚡ Quick Start (Local Setup)

1\. Clone this repository and navigate into the project directory:

&#x20;  ```bash

&#x20;  git clone \[https://github.com/Surojit7980/payshield-ai.git](https://github.com/Surojit7980/payshield-ai.git)

&#x20;  cd payshield-ai

