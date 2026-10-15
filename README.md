# Gabriel

Software engineer from Mato Grosso, Brazil. I build TypeScript/Node
backends, React Native (Expo) apps, and AI features with Supabase/Postgres,
and I use coding agents (Claude Code, Codex) daily, with tests, CI, and
review gates around them.

## Public work

- [whatsapp-cloud-api-node](https://github.com/TheLionGab/whatsapp-cloud-api-node):
  Node 22 + TypeScript strict service for the WhatsApp Business Cloud API.
  Zod contracts, injectable `fetch`, dry-run mode, Vitest + Supertest, CI.

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

## Coming next to this profile

- RAG evaluation harness, without the proprietary corpus
- The agent workflow gates, with tests
- The WhatsApp service ported to NestJS

## Stack

TypeScript, Node.js, Express, Zod, Vitest, React Native/Expo,
Supabase/Postgres (RLS, pgvector), GitHub Actions.
