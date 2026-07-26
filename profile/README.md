# ⚙️ Dehurdle Engineering

> Real-time voice AI simulation and practice platform for enterprise teams.

Dehurdle builds high-performance, sub-300ms voice AI simulations that allow sales executives, support agents, and leaders to practice critical conversations against dynamic AI avatars.

---

### 📐 Core Engineering & Architecture

1. **Sub-300ms Conversational Latency**
   Full-duplex WebSocket architecture (`@fastify/websocket`) streaming raw PCM audio between browser microphones and Gemini Live AI for instantaneous vocal responses.

2. **Enterprise Privacy & CISO Guardrails**
   Built from the ground up for strict infosec compliance (SOC2 / GDPR / DPDP). Zero customer voice data or transcripts are ever used for model training or shared with third parties.

3. **Hybrid Event-Driven Stack**
   Decoupled architecture isolating dashboard REST APIs, high-throughput voice WebSockets, and webhook automation pipelines (Razorpay, WorkOS, Slack Bot).

---

### 📦 Platform Monorepo Architecture

Our core monorepo is structured into specialized, domain-driven services:

| Service | Stack | Purpose |
| :--- | :--- | :--- |
| **`main-backend`** | Fastify 5, Node.js, Prisma, PostgreSQL | Core API backend, Gemini Live WebSockets, AWS SES email pipeline, and payment webhooks. |
| **`main-webapp`** | Next.js 16, React 19, Zustand, Tailwind | Main customer web app, audio streaming engine, and interactive debrief scorecards. |
| **`main-internal-admin`** | React 19, TypeScript | Multi-tenant admin console for telemetry, seat management, and credit overrides. |

*(Note: Core engine repositories and infrastructure configurations are kept private for enterprise infosec compliance.)*

---

### 🚀 We Are Hiring Systems & AI Engineers

We build real-time voice infrastructure, scalable WebSocket pipelines, and zero-leak privacy engines. If you obsess over low-latency Web Audio, Fastify performance, and clean TypeScript architecture, we want to talk to you.

🌐 **Website:** [dehurdle.com](https://dehurdle.com)  
📧 **Engineering Careers:** [reach@dehurdle.com](mailto:reach@dehurdle.com)
