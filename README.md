# Mohamed Arafa

### Backend engineer. I care about what happens when things go wrong.

A webhook arrives twice. A worker dies halfway through. An AI agent wants to send something it shouldn't.

That's the kind of backend work I like: figuring out what can break, then making the failure boring.

I work mostly with **TypeScript, Node.js, and NestJS**, backed by PostgreSQL, Redis, and queues.

[LinkedIn](https://www.linkedin.com/in/mohamed-arafa-6628211b8/) · [Email](mailto:mohamed3rafa01@gmail.com)

## Things I've built

### [Vetoq](https://github.com/mo74x/Vetoq)
**An AI agent can ask. A human gets the final say.**

An approval layer between agents and actions like refunds, emails, and database writes. Policies decide what needs review. People can edit or reject the action before it runs.

The interesting part: an email scanner opening an approval link must never approve anything. Vetoq separates viewing from deciding, checks for replay, and sends signed callbacks.

`NestJS` · `Next.js` · `PostgreSQL` · `Redis` · `BullMQ`

### [Matchbook](https://github.com/mo74x/matchbook)
**Same orders. Same sequence. Same result.**

An order matching engine with price-time priority and an append-only event history. If the process stops, it can rebuild its state by replaying events.

I keep storage and network calls outside the matching loop. The matching logic has one job: decide what trades.

`TypeScript` · `NestJS` · `PostgreSQL` · `WebSockets`

### [Invoice Chaser](https://github.com/mo74x/invoice-chaser)
**Check that the invoice is still unpaid before chasing it.**

A Stripe-connected reminder system with scheduled jobs and AI-assisted drafts. Before dispatch, it checks payment status, duplicates, send windows, and the generated text.

Writing the email is only one step. Knowing when not to send it is the part I care about.

`NestJS` · `Prisma` · `PostgreSQL` · `BullMQ` · `Stripe` · `Claude`

### [FleetPulse](https://github.com/mo74x/Fleetpulse)
**From assigning a courier to accounting for the cash.**

A delivery backend covering orders, dispatch, live tracking, and cash-on-delivery settlement.

Two dispatchers shouldn't get the same courier. A settlement shouldn't leave half the accounts updated. Redis locks and PostgreSQL transactions handle those boundaries.

`NestJS` · `PostgreSQL` · `Redis` · `RabbitMQ` · `MongoDB`

## Beyond my own repos

I contribute to **[NestJS](https://github.com/nestjs/nest)** and **[Nest CLI](https://github.com/nestjs/nest-cli)**, including microservice shutdown handling and compiler behavior. I like digging into the tools I use.

I also build **[agentic-json-repair](https://github.com/mo74x/agentic-json-repair)** for malformed JSON from LLMs and webhook streams. Sometimes the missing bracket really is the problem.

---

**My default:** assume retries will happen, keep money changes transactional, and leave enough evidence to debug the failure.
