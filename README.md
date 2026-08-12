<h1 align="center">Hi, I'm Mohamed Arafa 👋</h1>

<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=20&pause=1000&color=38B2AC&center=true&vCenter=true&width=800&lines=Backend+Software+Engineer;Event-Driven+Systems+%26+Microservices;Financial+Engines+%26+Distributed+Architecture;AWS+%26+Cloud-Native+Orchestration" alt="Typing SVG" />
  </a>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/mohamed-arafa-6628211b8/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:mohamed3rafa01@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
  <img src="https://komarev.com/ghpvc/?username=mo74x&label=Profile%20Views&color=0A66C2&style=for-the-badge" alt="Profile Views" />
</p>

<p align="center">
  <b>Building scalable, high-concurrency backend systems with Node.js, NestJS & TypeScript, deployed on AWS.</b><br>
  Specializing in event-driven microservices pipelines, deterministic matching engines, event sourcing, real-time telemetry, and cloud-native Kubernetes orchestration.
</p>

---

### ⚙️ Core Expertise & Tech Stack

<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=nodejs,nestjs,ts,express,py,django&perline=10" alt="Languages & Frameworks" /><br><br>
    <img src="https://skillicons.dev/icons?i=postgres,mongodb,redis,prisma,kafka,rabbitmq,graphql&perline=10" alt="Databases & Messaging" /><br><br>
    <img src="https://skillicons.dev/icons?i=aws,kubernetes,docker,prometheus,grafana,githubactions,react,nextjs&perline=10" alt="DevOps, Observability & UI" />
  </a>
</p>

---

### 🚀 Featured Projects

#### ⚡ [Matchbook](https://github.com/mo74x/matchbook) — Real-Time Event-Sourced Order Matching Engine
> High-throughput financial matching engine featuring Price-Time Priority (FIFO) execution, append-only event store crash recovery, full Prometheus/Grafana telemetry, and automated CI SLA performance gates.
*   **Deterministic Engine:** Implemented a synchronous Price-Time Priority (FIFO) matching algorithm supporting `LIMIT`, `MARKET`, `IOC`, and `FOK` order types with sub-millisecond execution times and L2 depth aggregation (**18,700+ ops/sec throughput**).
*   **Event Sourcing & Crash Recovery:** Designed an append-only event store (`OrderEvent`) backed by PostgreSQL 15, coupled with automated `OrderBookSnapshot` state checkpoints enabling zero-data-loss crash recovery.
*   **Multi-Market Isolation & Circuit Breakers:** Created per-instrument task queues (`MarketProcessor`) with automated circuit breakers that halt trading on persistence failures.

#### 💸 Hawala — Fintech Remittance Backend
> A trust-network settlement system designed for secure, distributed financial remittances.
*   **Core Architecture:** Built utilizing **NestJS**, **PostgreSQL**, **Redis**, and **BullMQ**.
*   **System Integrity:** Established strict domain rules and idempotency requirements to simulate secure financial settlements, preventing double-spending and ensuring transaction integrity across distributed nodes.

#### 🚚 [FleetPulse](https://github.com/mo74x/Fleetpulse) — Production-Grade Last-Mile Delivery Engine
> A polyglot-persistent, event-driven logistics platform handling the full delivery lifecycle — from order ingestion and geo-spatial courier dispatch, to double-entry financial settlement.
*   **Polyglot Persistence:** Architected a multi-database system using **MongoDB** (order documents), **PostgreSQL** (double-entry financial ledger), **Redis** (GeoSets, distributed locks), and **Elasticsearch** (fuzzy waybill search).
*   **Concurrency-Safe Dispatch:** Implemented a geo-spatial courier matching engine using **Redis GeoSets** (`GEOSEARCH`) with **Redlock** distributed locking to prevent race conditions during concurrent order assignment.
*   **Async Order Pipeline:** Designed a resilient order ingestion pipeline via **BullMQ** with exponential backoff retries, decoupled from **RabbitMQ** event-driven consumers.

#### 🌐 [Nexora](https://github.com/mo74x/Nexora) — Multi-Tenant Event Ingestion & Analytics Platform
> A high-performance 3-service microservices platform built to ingest, throttle, and analyze per-tenant events in real-time.
*   **Distributed Architecture:** Integrated cross-service communication utilizing **gRPC** for synchronous request-response and **Apache Kafka** for decoupled event-driven streaming.
*   **Atomic Rate Limiting:** Enforced dynamic per-tenant throttling using an atomic **Redis Lua token-bucket** script to guarantee system fairness.

#### 📦 agentic-json-repair (npm package)
> Open-source utility library published to the npm registry.
*   Provides robust, automated repair of malformed JSON strings, specifically optimized for handling unpredictable structural outputs from LLMs and agentic systems.

---

### 🛡️ Engineering Philosophy & System Design Values

*   **Deterministic & Event-Sourced Architecture:** Decoupling execution logic from I/O boundaries, using append-only event logs for auditability, replayability, and deterministic state recovery.
*   **Zero-Trust Multi-Tenancy:** Ensuring absolute tenant data isolation at the routing, service, and database levels.
*   **Observability & Metric-Driven Engineering:** Treating latency percentiles (p50, p95, p99), metric exposition (Prometheus/Grafana), and log correlation (`x-request-id`) as first-class citizens.

---

### 📊 GitHub Insights & Statistics

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=mo74x&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true" alt="GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=mo74x&layout=compact&theme=tokyonight&hide_border=true" alt="Top Languages" />
</p>
<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=mo74x&theme=tokyonight&hide_border=true" alt="GitHub Streak" />
</p>

---

<p align="center">
  <i>Let's build something remarkable. Open to senior and backend engineering opportunities. Feel free to reach out on <a href="https://www.linkedin.com/in/mohamed-arafa-6628211b8/">LinkedIn</a>.</i>
</p>
