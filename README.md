# PayShield AI — Autonomous PayPal Dispute & Chargeback Defense Engine

PayShield AI is an autonomous merchant revenue-defense platform engineered for the PayPal AI Hackathon 2026. The system interfaces directly with the PayPal Sandbox REST APIs (Orders v2 and Customer Disputes v1), validates agentic API payloads through the APIMatic MCP OpenAPI 3.0 specification, and delivers real-time financial triage via an AG Grid and AG Studio AI command center.

## Key Capabilities

- Live PayPal Sandbox Integration: Authenticates via PayPal OAuth 2.0, creates and inspects live orders, and monitors merchant disputes in real time.
- Fee-Waiver Micro-Dispute Triage: Automatically detects when contesting a low-value dispute incurs higher PayPal dispute fees than the transaction value itself, routing qualifying claims to accept-claim endpoints to waive associated fees.
- Cryptographic PDF Evidence Dossier Generator: For high-value claims, cross-verifies carrier delivery signatures and telemetry, compiles a downloadable PDF-1.4 legal evidence packet, and prepares dispute defense submissions.
- AG Grid and AG Studio Lenses: Interactive dark-mode financial matrix featuring instant AI triage filters, live KPI reconciliation, and one-click autonomous execution.

## Tech Stack & Sponsor Integrations

- PayPal Developer Platform: Sandbox OAuth 2.0, Orders v2 API, Customer Disputes v1 API
- AG Grid & AG Studio: Custom quartz dark financial telemetry grid and AI view lenses
- APIMatic MCP: Strict OpenAPI 3.0 schema and scope registry for agentic PayPal operations
- Backend & Runtime: Node.js zero-dependency HTTP engine and native PDF-1.4 generator
- Cloud Hosting: Render Web Service

## Quick Start (Local Setup)

1. Clone this repository and navigate into the project directory:
   git clone https://github.com/Surojit7980/payshield-ai.git
   cd payshield-ai

2. Create a .env file with your PayPal Sandbox credentials:
   PAYPAL_CLIENT_ID=your_sandbox_client_id
   PAYPAL_CLIENT_SECRET=your_sandbox_client_secret
   PAYPAL_API_BASE=https://api-m.sandbox.paypal.com

3. Start the server:
   node server.js

4. Open http://localhost:8000 in your browser.

## License

MIT License — see the LICENSE file for full text.
