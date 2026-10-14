<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/banner-light.svg">
  <img alt="Mohamed Arafa, backend and systems integration engineer" src="./assets/banner-light.svg" width="100%">
</picture>

<br/>

[LinkedIn](https://www.linkedin.com/in/mohamed-arafa-6628211b8/) | [Email](mailto:mohamed3rafa01@gmail.com) | [npm](https://www.npmjs.com/package/agentic-json-repair)

## About

I build backend systems where money and data have to stay correct: ledgers, payment and ERP integrations, and the event-driven plumbing between them.

My work is mostly Node.js, NestJS and TypeScript, and it keeps returning to the same hard problems: double-entry ledger integrity, effectively exactly-once webhook processing, deterministic execution, and fair multi-tenant rate limiting.

## Selected work

### [FleetPulse](https://github.com/mo74x/Fleetpulse)
Last-mile logistics with a double-entry settlement engine.

- ACID-compliant ledger in PostgreSQL, using pessimistic write locks (`SELECT FOR UPDATE`) across courier, merchant, and platform accounts.
- Geo-spatial dispatch on Redis GeoSets with Redlock, so one order is never assigned twice.
- Ingestion and settlement split into BullMQ and RabbitMQ workers with exponential backoff.

`NestJS` `PostgreSQL` `MongoDB` `Redis` `RabbitMQ` `Elasticsearch`

### Hawala
Remittance and ledger backend built around idempotent settlement.

- Idempotency keys and atomic state transitions prevent double-spending across settlement nodes.
- Background reconciliation on Redis and BullMQ, with a dead-letter queue isolating failed transfers.

`NestJS` `TypeScript` `PostgreSQL` `Redis` `BullMQ`

### [Matchbook](https://github.com/mo74x/matchbook)
Event-sourced order matching engine, 18,700+ ops/sec.

- Deterministic price-time priority matching for `LIMIT`, `MARKET`, `IOC`, and `FOK` orders, with sub-millisecond execution and L2 depth aggregation.
- Append-only PostgreSQL event log with automated snapshots, so state recovers after a crash without losing an event.
- Per-instrument queues, circuit breakers, and Prometheus and Grafana for SLA metrics.

`TypeScript` `Node.js` `PostgreSQL` `Prometheus` `Grafana`

### [Nexora](https://github.com/mo74x/Nexora)
Multi-tenant event ingestion and throttling platform.

- gRPC for low-latency service calls, Apache Kafka for high-throughput event streaming.
- Atomic per-tenant token-bucket rate limiter in a Redis Lua script, so one noisy tenant cannot starve the rest.

`Node.js` `TypeScript` `gRPC` `Kafka` `Redis` `Docker`

## Open source

[**agentic-json-repair**](https://www.npmjs.com/package/agentic-json-repair): a zero-dependency TypeScript utility that repairs malformed, truncated, or unescaped JSON from LLMs and external webhooks.

## Stack

| Area | Tools |
| :--- | :--- |
| Runtime and APIs | Node.js, NestJS, TypeScript, Express, Python, gRPC, GraphQL |
| Data | PostgreSQL, MongoDB, Redis (Lua, Redlock, GeoSets), Elasticsearch, Prisma, TypeORM |
| Messaging | Kafka, RabbitMQ, BullMQ, transactional outbox, dead-letter queues |
| Infrastructure | AWS, Docker, Kubernetes, GitHub Actions, Prometheus, Grafana |

## How I work

- Record events first. Append-only logs keep state auditable and replayable.
- Isolate tenants at every layer: routing, rate limits, and data.
- Measure latency in percentiles (p50, p95, p99) and trace requests with correlation IDs.

## Get in touch

Open to backend and integration roles. The best way to reach me is [LinkedIn](https://www.linkedin.com/in/mohamed-arafa-6628211b8/) or [email](mailto:mohamed3rafa01@gmail.com).
