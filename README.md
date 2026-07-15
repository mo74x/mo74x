
<h1 align="center">Hi, I'm Mohamed Arafa 👋</h1>
<h3 align="center">Backend Software Engineer | Event-Driven Systems & Distributed Architecture</h3>
<p align="center">
  <a href="https://www.linkedin.com/in/mohamed-arafa-6628211b8/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:mohamed3rafa01@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>
<p align="center">
  <b>Building scalable, high-concurrency backend systems with Node.js, NestJS & TypeScript, complemented by modern interfaces in React & Next.js.</b><br>
  Specializing in event-driven microservices pipelines, multi-tenant isolation, real-time telemetry, and high-performance caching strategies.
</p>
---
### ⚙️ Core Expertise & Tech Stack
| Category | Technologies |
| :--- | :--- |
| **Languages & Core** | ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white) ![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Express.js](https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white) |
| **Frontend & UI** | ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white) ![Redux](https://img.shields.io/badge/Redux-764ABC?style=flat-square&logo=redux&logoColor=white) ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white) |
| **Messaging & Real-Time** | ![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white) ![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white) ![gRPC](https://img.shields.io/badge/gRPC-4285F4?style=flat-square&logo=googlecloud&logoColor=white) ![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white) ![Socket.io](https://img.shields.io/badge/Socket.io-010101?style=flat-square&logo=socket.io&logoColor=white) |
| **Databases & Caching** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) ![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white) ![TypeORM](https://img.shields.io/badge/TypeORM-FE0902?style=flat-square&logo=typeorm&logoColor=white) |
| **DevOps & Infrastructure** | ![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![k6](https://img.shields.io/badge/k6-7D64FF?style=flat-square&logo=k6&logoColor=white) |
---
### 🚀 Featured Projects
#### 🌐 [Nexora](https://github.com/mo74x/Nexora) — Multi-Tenant Event Ingestion & Analytics Platform
> A high-performance 3-service microservices platform built to ingest, throttle, and analyze per-tenant events in real-time.
*   **Distributed Architecture:** Integrated cross-service communication utilizing **gRPC** for synchronous request-response and **Apache Kafka** for decoupled event-driven streaming.
*   **Atomic Rate Limiting:** Enforced dynamic per-tenant throttling using an atomic **Redis Lua token-bucket** script to guarantee system fairness and prevent noisy-neighbor issues.
*   **Performance & Validation:** Rigorously load-tested with **k6**, validating sub-500ms p99 latency under high-concurrency scenarios (200+ concurrent users).
*   **Analytics Interface:** Built a flexible, low-latency **GraphQL** API layer for rapid querying of historical and real-time ingestion analytics.
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
*   **Zero-Trust Multi-Tenancy:** Ensuring absolute tenant data isolation at the routing, service, and database levels (e.g. strict JWT claim parsing and schema boundaries).
*   **ACID & Transactional Integrity:** Designing strict ledger schemas (e.g. append-only ledgers) and protecting resources using Redis-based distributed locks.
*   **Performance as a First-Class Citizen:** Constantly benchmarking services with k6, identifying database bottlenecks, and tuning indexing/caching patterns.
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
