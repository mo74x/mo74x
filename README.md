<div align="center">

# Mohamed Arafa
### Backend & Systems Integration Engineer

<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&pause=1200&color=10B981&center=true&vCenter=true&width=750&lines=High-Concurrency+Backend+Architecture+%7C+Node.js+%26+NestJS;Financial+Ledgers%2C+Idempotency+%26+Enterprise+Integrations;Event-Driven+Microservices+%7C+Kafka%2C+RabbitMQ+%26+BullMQ;Deterministic+Matching+Engines+%26+AI-Driven+FinTech+Workflows" alt="Typing SVG" />
</a>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Mohamed_Arafa-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mohamed-arafa-6628211b8/)
[![Email](https://img.shields.io/badge/Email-mohamed3rafa01%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:mohamed3rafa01@gmail.com)
[![npm](https://img.shields.io/badge/npm-agentic--json--repair-CB3837?style=flat-square&logo=npm&logoColor=white)](https://www.npmjs.com/package/agentic-json-repair)
![Profile Views](https://komarev.com/ghpvc/?username=mo74x&label=Views&color=10B981&style=flat-square)

</div>

---

### ⚡ About Me

I design and build **fault-tolerant, high-throughput backend systems and financial integrations** using **Node.js, NestJS, and TypeScript**. My work focuses on the hardest boundaries of distributed systems: **double-entry ledger integrity, effective exactly-once webhook processing, deterministic execution, multi-tenant isolation, and resilient AI-driven financial workflows**.

<pre align="center">
Inbound Webhooks ──► [ Fast-Ack / HMAC / Dedup ] ──► [ BullMQ / Kafka ] ──► [ ACID Ledger / 6-Gate Worker ] ──► [ Outbox / Audit Trail ]
</pre>

---

### 🏗️ Featured Systems & Architecture

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>⚡ <a href="https://github.com/mo74x/matchbook">Matchbook</a></h3>
      <p><b>Real-Time Event-Sourced Order Matching Engine</b></p>
      <p>
        <img src="https://img.shields.io/badge/Throughput-18,700%2B_ops%2Fsec-10B981?style=flat-square" alt="Throughput" />
        <img src="https://img.shields.io/badge/Pattern-Event_Sourcing-3B82F6?style=flat-square" alt="Event Sourcing" />
      </p>
      <ul>
        <li><b>Deterministic FIFO Engine:</b> Synchronous Price-Time Priority matching supporting <code>LIMIT</code>, <code>MARKET</code>, <code>IOC</code>, and <code>FOK</code> orders with sub-millisecond execution and L2 depth aggregation.</li>
        <li><b>Zero-Loss Crash Recovery:</b> Append-only PostgreSQL 15 event log (<code>OrderEvent</code>) paired with automated <code>OrderBookSnapshot</code> state checkpoints.</li>
        <li><b>Fault Isolation:</b> Per-instrument queues with automated circuit breakers and Prometheus/Grafana SLA telemetry.</li>
      </ul>
      <p><code>TypeScript</code> <code>Node.js</code> <code>PostgreSQL</code> <code>Prometheus</code> <code>Grafana</code></p>
    </td>
    <td width="50%" valign="top">
      <h3>🧾 <a href="https://github.com/mo74x/invoice-chaser">Invoice Chaser</a></h3>
      <p><b>Autonomous AI Invoice Recovery & Dunning Engine</b></p>
      <p>
        <img src="https://img.shields.io/badge/Ingestion-10k_Webhook_Storm-10B981?style=flat-square" alt="Webhook Storm" />
        <img src="https://img.shields.io/badge/Security-AES--256--GCM_%2B_Multi--Tenant-8B5CF6?style=flat-square" alt="Security" />
      </p>
      <ul>
        <li><b>Six-Gate BullMQ Pipeline:</b> Orchestrates multi-stage Stripe dunning with idempotent webhook deduplication, live pre-send Stripe status verification, timezone send windows, and DLQ replay.</li>
        <li><b>Hallucination-Guarded AI Voice Cloning:</b> Extracts founder writing traits via Claude and enforces strict output validation (exact currency match, zero fabricated payment links) with deterministic fallback.</li>
        <li><b>Zero-Trust Multi-Tenancy:</b> AES-256-GCM encrypted Stripe OAuth tokens at rest, Svix-verified Resend delivery/inbound reply auto-pause, and RFC 8058 one-click unsubscribe cascades.</li>
      </ul>
      <p><code>NestJS 11</code> <code>Prisma 7</code> <code>PostgreSQL</code> <code>Redis</code> <code>BullMQ</code> <code>Stripe</code> <code>Claude AI</code> <code>k6</code></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>🚚 <a href="https://github.com/mo74x/Fleetpulse">FleetPulse</a></h3>
      <p><b>Last-Mile Logistics & Double-Entry Settlement Engine</b></p>
      <p>
        <img src="https://img.shields.io/badge/Ledger-ACID_Double--Entry-10B981?style=flat-square" alt="Ledger" />
        <img src="https://img.shields.io/badge/Locking-Redlock_%2B_Pessimistic-F59E0B?style=flat-square" alt="Locking" />
      </p>
      <ul>
        <li><b>Financial Settlement Engine:</b> ACID-compliant double-entry ledger in PostgreSQL using pessimistic write locks (<code>SELECT FOR UPDATE</code>) across courier, merchant, and platform accounts.</li>
        <li><b>Concurrency-Safe Dispatch:</b> Geo-spatial matching via <b>Redis GeoSets</b> (<code>GEOSEARCH</code>) and distributed <b>Redlock</b> to eliminate double-assignment race conditions.</li>
        <li><b>Resilient Pipelines:</b> Decoupled ingestion and settlement workers via <b>BullMQ</b> and <b>RabbitMQ</b> with exponential backoff.</li>
      </ul>
      <p><code>NestJS</code> <code>PostgreSQL</code> <code>MongoDB</code> <code>Redis</code> <code>RabbitMQ</code> <code>Elasticsearch</code></p>
    </td>
    <td width="50%" valign="top">
      <h3>🌐 <a href="https://github.com/mo74x/Nexora">Nexora</a></h3>
      <p><b>Multi-Tenant Event Ingestion & Throttling Platform</b></p>
      <p>
        <img src="https://img.shields.io/badge/RPC-gRPC_%2B_Kafka-3B82F6?style=flat-square" alt="gRPC Kafka" />
        <img src="https://img.shields.io/badge/Rate_Limit-Redis_Lua_Script-10B981?style=flat-square" alt="Rate Limit" />
      </p>
      <ul>
        <li><b>Hybrid Transport:</b> Low-latency internal service communication via <b>gRPC</b> combined with high-throughput <b>Apache Kafka</b> event streaming.</li>
        <li><b>Noisy-Neighbor Protection:</b> Atomic per-tenant <b>Redis Lua token-bucket</b> rate limiter ensuring strict fairness under burst traffic.</li>
        <li><b>Distributed Backpressure:</b> Isolates high-volume tenant spikes without degrading shared downstream consumers.</li>
      </ul>
      <p><code>Node.js</code> <code>TypeScript</code> <code>gRPC</code> <code>Kafka</code> <code>Redis</code> <code>Docker</code></p>
    </td>
  </tr>
  <tr>
    <td colspan="2" valign="top">
      <h3>💸 Hawala</h3>
      <p><b>Distributed FinTech Remittance & Ledger Backend</b></p>
      <p>
        <img src="https://img.shields.io/badge/Architecture-Idempotent_Settlement-8B5CF6?style=flat-square" alt="Idempotent" />
        <img src="https://img.shields.io/badge/Queue-BullMQ_Workers-EF4444?style=flat-square" alt="BullMQ" />
      </p>
      <ul>
        <li><b>Transaction Integrity:</b> Enforces strict idempotency keys and atomic state transitions to prevent double-spending across distributed settlement nodes.</li>
        <li><b>Async Reconciliation:</b> Background settlement pipelines backed by <b>Redis</b> and <b>BullMQ</b> with Dead-Letter Queue (DLQ) isolation for failed transfers.</li>
      </ul>
      <p><code>NestJS</code> <code>TypeScript</code> <code>PostgreSQL</code> <code>Redis</code> <code>BullMQ</code></p>
    </td>
  </tr>
</table>

---

### 📦 Open-Source & Published Packages

| Package | Description | Registry |
| :--- | :--- | :--- |
| **[agentic-json-repair](https://www.npmjs.com/package/agentic-json-repair)** | Zero-dependency TypeScript utility for deterministic repair of malformed, truncated, or unescaped JSON payloads emitted by LLMs and external webhooks. | [![npm](https://img.shields.io/npm/v/agentic-json-repair?style=flat-square&color=CB3837)](https://www.npmjs.com/package/agentic-json-repair) |

---

### 🛠️ Technology & Architecture Stack

| Layer | Technologies |
| :--- | :--- |
| **Runtime & Frameworks** | `Node.js` · `NestJS` · `TypeScript` · `Express.js` · `Python` · `gRPC` · `GraphQL` |
| **Databases & Ledgers** | `PostgreSQL` · `MongoDB` · `Redis (Lua / Redlock / Geo)` · `Elasticsearch` · `Prisma 7` · `TypeORM` |
| **Messaging & Webhooks** | `Apache Kafka` · `RabbitMQ` · `BullMQ` · `Stripe OAuth & Webhooks` · `Svix / Resend` · `Transactional Outbox` · `DLQ` |
| **Cloud, Security & QA** | `AWS` · `Docker` · `Kubernetes` · `AES-256-GCM` · `GitHub Actions CI/CD` · `Prometheus` · `Grafana` · `k6` |

<br/>

<p align="center">
  <img src="https://skillicons.dev/icons?i=nodejs,nestjs,ts,postgres,prisma,mongodb,redis,kafka,rabbitmq,graphql,aws,docker,kubernetes,prometheus,grafana,githubactions&perline=16" alt="Tech Stack Icons" />
</p>

---

### 🛡️ Engineering Philosophy & System Design Values

* **Deterministic & Event-Sourced Architecture:** Decoupling execution logic from I/O boundaries, using append-only event logs and immutable audit trails (`OrderEvent`, `ReminderAudit`) for replayability and state recovery.
* **Zero-Trust Multi-Tenancy:** Enforcing tenant isolation at the JWT authentication, rate-limiting, encryption-at-rest (AES-256-GCM), and database query levels.
* **Observability & Load-Verified Engineering:** Treating latency percentiles (p50, p95, p99), Prometheus/Grafana telemetry, k6 stress testing, and Dead-Letter Queue (DLQ) replayability as first-class citizens.

---

### 📈 GitHub Telemetry

<div align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=mo74x&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=10B981&icon_color=10B981&include_all_commits=true&count_private=true" alt="GitHub Stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=mo74x&layout=compact&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=10B981" alt="Top Languages" />
</div>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=mo74x&theme=tokyonight&hide_border=true&background=0D1117&ring=10B981&fire=10B981&currStreakLabel=10B981" alt="GitHub Streak" />
</p>

---

<div align="center">
  <sub>Built with architectural rigor · Always open to discussing distributed systems, fintech infrastructure, and backend engineering on <a href="https://www.linkedin.com/in/mohamed-arafa-6628211b8/"><b>LinkedIn</b></a>.</sub>
</div>
