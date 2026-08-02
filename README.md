<h1 align="center">Hi, I'm Mohamed Arafa 👋</h1>
<h3 align="center">Backend Software Engineer | Event-Driven Systems, Financial Engines & Distributed Architecture</h3>

<p align="center">
  <a href="https://www.linkedin.com/in/mohamed-arafa-6628211b8/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:mohamed3rafa01@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>

<p align="center">
  <b>Building scalable, high-concurrency backend systems with Node.js, NestJS & TypeScript, complemented by modern interfaces in React & Next.js.</b><br>
  Specializing in event-driven microservices pipelines, deterministic matching engines, event sourcing, real-time telemetry, and cloud-native Kubernetes orchestration.
</p>

---

### ⚙️ Core Expertise & Tech Stack

| Category | Technologies |
| :--- | :--- |
| **Languages & Core** | ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white) ![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Express.js](https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white) |
| **Messaging & Real-Time** | ![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white) ![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white) ![Socket.io](https://img.shields.io/badge/Socket.io-010101?style=flat-square&logo=socket.io&logoColor=white) ![gRPC](https://img.shields.io/badge/gRPC-4285F4?style=flat-square&logo=googlecloud&logoColor=white) ![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white) |
| **Databases & Event Sourcing** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) ![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white) ![TypeORM](https://img.shields.io/badge/TypeORM-FE0902?style=flat-square&logo=typeorm&logoColor=white) |
| **Observability & DevOps** | ![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white) ![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white) ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white) ![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) |
| **Frontend & UI** | ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white) ![Redux](https://img.shields.io/badge/Redux-764ABC?style=flat-square&logo=redux&logoColor=white) ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white) |

---

### 🚀 Featured Projects

#### ⚡ [Matchbook](https://github.com/mo74x/matchbook) — Real-Time Event-Sourced Order Matching Engine
> High-throughput financial matching engine featuring Price-Time Priority (FIFO) execution, append-only event store crash recovery, full Prometheus/Grafana telemetry, and automated CI SLA performance gates.

*   **Deterministic Engine:** Implemented a synchronous Price-Time Priority (FIFO) matching algorithm supporting `LIMIT`, `MARKET`, `IOC`, and `FOK` order types with sub-millisecond execution times and L2 depth aggregation (**18,700+ ops/sec throughput**).
*   **Event Sourcing & Crash Recovery:** Designed an append-only event store (`OrderEvent`) backed by PostgreSQL 15, coupled with automated `OrderBookSnapshot` state checkpoints enabling zero-data-loss crash recovery.
*   **Multi-Market Isolation & Circuit Breakers:** Created per-instrument task queues (`MarketProcessor`) with automated circuit breakers that halt trading on persistence failures, preventing memory/database state divergence.
*   **Observability & Cloud-Native Deployment:** Built custom Prometheus OpenMetrics (`prom-client`), auto-provisioned Grafana dashboards, `AsyncLocalStorage` request correlation ID tracking, and production Kubernetes manifests & Helm v3 charts with Horizontal Pod Autoscaling (HPA).
*   **CI SLA Gate:** Configured GitHub Actions CI pipeline with automated SLA performance verification (`p95 <= 500ms`, `throughput >= 5,000 ops/sec`).

---

#### 🌐 [Nexora](https://github.com/mo74x/Nexora) — Multi-Tenant Event Ingestion & Analytics Platform
> A high-performance 3-service microservices platform built to ingest, throttle, and analyze per-tenant events in real-time.

*   **Distributed Architecture:** Integrated cross-service communication utilizing **gRPC** for synchronous request-response and **Apache Kafka** for decoupled event-driven streaming.
*   **Atomic Rate Limiting:** Enforced dynamic per-tenant throttling using an atomic **Redis Lua token-bucket** script to guarantee system fairness and prevent noisy-neighbor issues.
*   **Performance & Validation:** Rigorously load-tested with **k6**, validating sub-500ms p99 latency under high-concurrency scenarios (200+ concurrent users).
*   **Analytics Interface:** Built a flexible, low-latency **GraphQL** API layer for rapid querying of historical and real-time ingestion analytics.

---

#### 🚚 [FleetPulse](https://github.com/mo74x/Fleetpulse) — Production-Grade Last-Mile Delivery Engine
> A polyglot-persistent, event-driven logistics platform handling the full delivery lifecycle — from order ingestion and geo-spatial courier dispatch, through real-time GPS tracking, to double-entry financial settlement.

*   **Polyglot Persistence:** Architected a multi-database system using **MongoDB** (order documents), **PostgreSQL** (double-entry financial ledger), **Redis** (GeoSets, distributed locks, BullMQ queues), and **Elasticsearch** (fuzzy waybill search) — each selected for its optimal use case.
*   **Concurrency-Safe Dispatch:** Implemented a geo-spatial courier matching engine using **Redis GeoSets** (`GEOSEARCH`) with **Redlock** distributed locking to prevent race conditions during concurrent order assignment.
*   **Double-Entry Ledger:** Built an ACID-compliant COD (Cash-on-Delivery) settlement engine using **TypeORM** pessimistic write locks (`SELECT FOR UPDATE`) to guarantee financial consistency across courier, merchant, and platform accounts.
*   **Async Order Pipeline:** Designed a resilient order ingestion pipeline via **BullMQ** with exponential backoff retries, decoupled from **RabbitMQ** event-driven consumers (`order.delivered`) triggering downstream financial processing.
*   **Real-Time Telemetry:** Established **Socket.IO** WebSocket connections on a `/telemetry` namespace for continuous driver GPS coordinate ingestion, stored in Redis GeoSets for proximity queries.
*   **Observability & Hardening:** Integrated **@nestjs/terminus** health checks (Postgres, MongoDB, Redis, Elasticsearch), global **@nestjs/throttler** rate limiting (100 req/min), JWT + RBAC authentication, and a **GitHub Actions** CI pipeline with automated lint, build, and test gates.

---

#### 💼 Caliber Talent Network — Event-Driven Recruitment Platform
> An asynchronous recruitment pipeline designed to handle document processing and user management under strict tenant-isolation policies.

*   **Background Processing:** Designed a resilient resume and document parsing queue using **Redis** and **BullMQ** for delayed and background task execution.
*   **Secure Multi-Tenancy:** Implemented bulletproof data isolation between recruiters and candidates using **JWT-based RBAC (Role-Based Access Control)**.
*   **Payment Gateways:** Integrated **Stripe webhooks** to automatically handle subscription lifecycle events, processing invoices and access grants asynchronously.

---

#### 🏎️ PitWall — Real-Time F1 Telemetry System
> High-throughput IoT/telemetry processing system capturing live F1 race telemetry at sub-millisecond latencies.

*   **Telemetry Ingestion:** Developed concurrent consumer microservices built around **RabbitMQ** to ingest and route continuous streams of sensor data.
*   **Live Leaderboards:** Implemented memory-optimized caching patterns in **Redis** to store and serve live, real-time leaderboard statistics instantly.
*   **Infrastructure & Scaling:** Packaged applications using **Docker** and deployed to **AWS ECS Fargate**, designing auto-scaling policies triggered by telemetry ingestion spikes.

---

#### 📦 LogiTrack — Event-Driven Logistics Backend
> Geolocation tracking and dispatcher-matching engine processing rapid updates for fleet management.

*   **State Tracking:** Leveraged **Apache Kafka** to track driver statuses, trip states, and logistical checkpoints in an append-only event stream.
*   **Driver Matching:** Utilized **MongoDB Geospatial indexing** and queries to calculate real-time spatial proximity, automatically matching drivers to incoming orders.
*   **Real-Time Subscriptions:** Established full-duplex persistent connections using **Socket.io** to stream live driver coordinate changes directly to customer apps.

---

### 🛡️ Engineering Philosophy & System Design Values

*   **Deterministic & Event-Sourced Architecture:** Decoupling execution logic from I/O boundaries, using append-only event logs for auditability, replayability, and deterministic state recovery.
*   **Zero-Trust Multi-Tenancy:** Ensuring absolute tenant data isolation at the routing, service, and database levels (e.g. strict JWT claim parsing and schema boundaries).
*   **Observability & Metric-Driven Engineering:** Treating latency percentiles (p50, p95, p99), metric exposition (Prometheus/Grafana), and log correlation (`x-request-id`) as first-class citizens.
*   **Performance & SLA Enforcement:** Constantly benchmarking under load, identifying database bottlenecks, and enforcing SLA performance gates in CI/CD pipelines.

---

### 📊 GitHub Insights & Statistics

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=mo74x&show_icons=true&theme=tokyonight&hide_border=true" alt="GitHub Stats" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=mo74x&theme=tokyonight&hide_border=true" alt="GitHub Streak" />
</p>

---

<p align="center">
  <i>Let's build something remarkable. Open to senior and backend engineering opportunities. Feel free to reach out on <a href="https://www.linkedin.com/in/mohamed-arafa-6628211b8/">LinkedIn</a>.</i>
</p>
