# Gabriel

**Software Engineer · TypeScript · Backend · AI Evaluation**

I build TypeScript backends, React Native / Expo apps, and AI features with
Supabase and Postgres. I use coding agents with automated tests, CI, and
explicit review gates.

Mato Grosso, Brazil · [LinkedIn](https://www.linkedin.com/in/liongabdev/)

## Featured engineering work

| Project | Problem and approach | Evidence to inspect |
| --- | --- | --- |
| [Agent Merge Guard](https://github.com/TheLionGab/agent-merge-guard) | Pure decision functions reject unreviewed PR changes, incomplete inspections, and unexpected identities. | 21 tests; commit race, rename allowlist, and hostile text cases. |
| [Deterministic Answer Grader](https://github.com/TheLionGab/deterministic-answer-grader) | Offline grading of collected LLM answers with explicit safety and quality rules. | 13 tests; a versioned 19-case fixture; reproducible 18/19 result with the false negative explained. |
| [WhatsApp Gateway — Express](https://github.com/TheLionGab/whatsapp-gateway-express) | A small HTTP service with signed webhooks, authenticated sending, and an injectable provider. | 14 tests; strict TypeScript; Vitest + Supertest; CI. |
| [WhatsApp Gateway — NestJS](https://github.com/TheLionGab/whatsapp-gateway-nestjs) | The same service expressed through modules, guards, pipes, filters, and dependency injection. | 23 tests, including raw-body signatures, guard ordering, and log redaction. |

The gateways are two implementations of one service. Compare them to see
architectural tradeoffs. Each project documents its design, test strategy,
setup, and limitations; none requires a paid API to run its test suite.

## Engineering focus

- Separate deterministic decisions from model output and external I/O.
- Write tests for incorrect implementations, including races and security boundaries.
- Make results reproducible and document where the evidence stops.

## Product work

My work also includes **Pulso do Campo**, an agricultural app, and private
client projects. The public repositories above provide inspectable examples
without exposing private source code. The grader includes a dated answer
fixture; reproducing it does not verify the current production system.

## Stack

TypeScript · Node.js · Express · NestJS · Zod · Vitest · React Native / Expo ·
Supabase / Postgres · GitHub Actions
