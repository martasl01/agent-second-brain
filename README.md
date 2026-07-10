# Content Second Brain

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)
[![claude-code](https://img.shields.io/badge/claude--code-black?style=flat-square)](https://claude.ai/code)
![ai-agents](https://img.shields.io/badge/ai--agents-5C6BC0?style=flat-square)
![knowledge-management](https://img.shields.io/badge/knowledge--management-2E7D32?style=flat-square)
![second-brain](https://img.shields.io/badge/second--brain-6D4C41?style=flat-square)

A living knowledge system for a Claude Code agent that helps create **short-form content for X (Twitter) and LinkedIn**. It's an instantiation of the architecture in Pawel Huryn's case study — *"From 4 hours to 30 minutes a day. 5M+ X impressions in 3 months"* — built on his [`agent-second-brain`](https://github.com/phuryn/agent-second-brain) starter kit.

The point isn't a config file that tells Claude what tone to take. It's a **memory architecture that compounds**: rules graduate from hypotheses, failed beliefs get logged so they're never re-tested, and the agent loads only what each task needs.

---

## What's in here (already set up)

This repo is **not** an empty starter — the identity and content knowledge base are filled in:

- **`CLAUDE.md`** — the brain. Identity (content creator / builder-teacher), output standards, routing table, the ingest + hypothesis procedures, and the hard constraints that keep the system honest.
- **`knowledge/INDEX.md`** — the router. Loaded first; tells the agent which `craft/` files a given task needs (progressive disclosure — never load everything).
- **`knowledge/craft/`** — the content domain, mirroring the case-study tree:
  - `writing-techniques.md` — the craft rules (one idea per post, the data-experiment format, the 10+ iteration editing loop).
  - `voice/archetypes.md` — 9 voice archetypes; **Builder-Teacher** is the default and the high performer.
  - `platforms/x-twitter.md` + `platforms/linkedin.md` — per-platform hooks, templates, rules (e.g. **negation hooks beat positive hooks on LinkedIn**).
  - `posts/performance-log.md` — the feedback layer; analyzed posts and the metrics that confirm or challenge rules.
  - `topic-lanes.md` — 7 topic lanes with energy tracking.
  - `hypotheses/` — the learning loop: `index.md` (active + graduated), `rejected.md` (immune memory), `EXAMPLE.md` (schema).

---

## Four cognitive components

| Component | What it does | Key file |
|-----------|-------------|----------|
| **Perception** | Loads only what the task needs (3–4 files standard) | `knowledge/INDEX.md` |
| **Reasoning** | Routes task types to the right knowledge files | `CLAUDE.md` routing table |
| **Learning** | Tests hypotheses, graduates them to rules with 3+ data points | `craft/hypotheses/index.md` |
| **Immunity** | Logs rejected beliefs so the agent never re-tests them | `craft/hypotheses/rejected.md` |

New evidence becomes a **hypothesis** first. Hypotheses graduate through evidence, not conviction. The false belief you've already tested is the most expensive one to re-test.

---

## How the patterns got here (honesty note)

Three rules are seeded from findings the **case study reports with data**, and tagged `[from case study]` in the files:

1. Data-experiment posts earn ~**3× the bookmarks** of opinion posts.
2. **Negation hooks** outperform positive hooks on LinkedIn.
3. **Builder-teacher** posts outperform analyst takes.

The article is partly paywalled and does **not** publish the underlying 26 templates, 13 hypotheses, or 50+ false beliefs. So everything else here is a **starter** — sensible defaults seeded at setup, clearly marked, meant to be confirmed or killed by your own data. Nothing fabricated is presented as Pawel's private content.

---

## How to use it

1. Open Claude Code in this directory. The agent loads `knowledge/INDEX.md` at the start of every conversation.
2. **Draft:** "draft a LinkedIn post about X" → it loads the craft + platform rules, proposes hooks, and iterates with you.
3. **Learn:** after a post runs, log its metrics in `craft/posts/performance-log.md`. When a pattern hits 3+ data points, the agent surfaces it for graduation to a rule.
4. **Stay honest:** when something contradicts a rule, the agent opens a hypothesis instead of silently editing the rule. Disproven beliefs go to `rejected.md`.

To extend: add a knowledge file, then add its routing row to `knowledge/INDEX.md` **and** the `CLAUDE.md` table. See `knowledge/system-maintenance.md` for split/merge/archive rules.

---

## Credit

Architecture by **Pawel Huryn** (The Product Compass). Based on his production system and case study:

- Starter kit: https://github.com/phuryn/agent-second-brain
- Case study: *Karpathy Built a Second Brain for Humans. Here's One for Your AI Agent.* — https://www.productcompass.pm/p/self-improving-claude-system

The role examples under `examples/` (software-engineer, researcher, ops-engineer) are from the original starter kit and kept as reference.
