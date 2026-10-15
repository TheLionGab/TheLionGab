# Gabriel

Software engineer from Mato Grosso, Brazil. I build TypeScript/Node
backends, React Native (Expo) apps, and AI features with Supabase/Postgres,
and I use coding agents (Claude Code, Codex) daily, with tests, CI, and
review gates around them.

## Public work

- [agent-workflow-gates](https://github.com/TheLionGab/agent-workflow-gates):
  pure decision gates for multi-agent workflows. The agent only reads; a
  deterministic function decides the merge (path allowlist, single SHA,
  CI), and untrusted text is marked as data. 18 tests, checked by mutation.
- [llm-answer-eval](https://github.com/TheLionGab/llm-answer-eval):
  offline, deterministic grader for LLM chat answers (Deno/TypeScript).
  Fixed questions, hard safety failures, reproducible score: 18 of 19
  (0.947) from a production run, with the failing case explained.
- [whatsapp-cloud-api-node](https://github.com/TheLionGab/whatsapp-cloud-api-node):
  Node 22 + TypeScript strict service for the WhatsApp Business Cloud API.
  Zod contracts, signature-checked webhook, authenticated send, dry-run
  mode, Vitest + Supertest, CI.

- [whatsapp-cloud-api-nestjs](https://github.com/TheLionGab/whatsapp-cloud-api-nestjs):
  the same service ported to NestJS: module, controllers, provider with an
  injectable `fetch`, guards, Zod pipe, exception filter. 23 tests, 0
  audit findings. A port of the Express project above, not a new product.

## What I work on (private repositories)

Most of my code lives in private repositories for clients and my own
products, so it is not listed here. I am happy to walk through it.

- Pulso do Campo, a farming app with production RAG over an agronomic
  corpus. Retrieval uses curated metadata plus reranking, and the final
  answers are scored by a fixed 19-question evaluation: 18 of 19 passed
  (0.947), with zero dose, product or brand violations, on the first
  production run (15 Oct 2026).
- A multi-agent workflow that finds problems, has a skeptic try to refute
  each finding, ranks them, and opens PRs for human review. Agents never
  merge or write to production on their own. Security review rounds on it
  found and closed real issues (for example a race between reading CI
  status and the commit SHA).

## Stack

TypeScript, Node.js, Express, Zod, Vitest, React Native/Expo,
Supabase/Postgres (RLS, pgvector), GitHub Actions.
