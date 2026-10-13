---
name: claude-ccdv-f
description: Companion for Anthropic's Claude Certified Developer - Foundations (CCDV-F) cert and for doing the Developer's actual job: building production-grade Claude apps, agents, and workflows (API mechanics, prompt/tool engineering, model selection, cost management, MCP servers, evals, security). Use when preparing for CCDV-F or shipping Claude-powered software. Not for no-code work (CCAO-F) or system-level architecture (CCAR-F/P).
metadata:
  short-description: CCDV-F certification + production Claude-app engineering skill
---

# Claude CCDV-F (Developer - Foundations)

Two uses, one skill: (a) get an agent skillful at the Developer job - standing up a
well-engineered application against the Claude API, wiring agents with the Agent SDK,
defining tools and MCP servers, managing model/cost decisions, and proving reliability -
and (b) prepare for the CCDV-F exam (53 items, 8 domains, 120 min, pass 720/1000,
$125 USD, the hands-on builder credential; counts toward the Claude Partner Network tier).

Read [references/ccdv-f-blueprint.md](references/ccdv-f-blueprint.md) for the 8-domain,
25-sub-skill blueprint with official weights and the "what good looks like" per domain.
Read [references/ccdv-f-logistics.md](references/ccdv-f-logistics.md) for access, fees,
retake/renewal, and free prep. Read
[../references/claude-cert-family.md](../references/claude-cert-family.md) for the
four-cert family and role routing.

## The builder's discipline (task guidance)

The exam rewards people who can stand up a well-engineered application against the Claude
API, not people who can describe one. One third of the exam is Applications and
Integration.

- **Understand the substrate at the level that drives decisions**: tokens; the context
  window as a fixed budget; sampling and non-determinism; model tiers; SDK vs REST access
  patterns. These drive prompt, tool, and agent design choices.
- **Prompt like production code**: system prompts, XML structure, few-shot examples,
  explicit constraints. Diagnose underperformance: which component failed (system
  prompt, context, tool definitions, example set) and fix that one.
- **Tools = schemas, not vibes**: every tool is a narrow purpose, a usable description,
  an input schema, an auth boundary, and a structured failure result. Build the
  tool-use loop (model -> tool call -> result -> model) with controlled retries that
  only fire when they can change the outcome.
- **Extended thinking for multi-turn work**: manage it explicitly across turns; do not
  assume a fixed behaviour.
- **Agents: smallest architecture that meets the need**: direct call / fixed workflow /
  agentic loop. Name the owner, the state carried forward, and the human-decision moment
  per step. A coordinator needs a bounded task, a clear hand-off, and a consumable result
  format. Human-in-the-loop checkpoints on irreversible actions. Design for partial
  failure before adding agents.
- **Claude Code**: operate under a permission model; give it durable project context;
  package workflows as Skills and plugins.
- **Model selection and cost**: match tier to the task; manage tokens and context; the
  Batches API is a cost tool, not a speed tool - never for user-facing real-time paths.
- **Security is designed in, not bolted on**: guardrails and safe deployment; hooks;
  identity, secrets, and key management.
- **Prove it before shipping**: build evals that resemble real tasks (labelled set,
  success criteria, review process). Debugging and error handling are lightweight on the
  exam (2.6%) - they are on it, not where it is decided.

## How to answer exam-style questions

- Lead with the decision and its trade-off; cite the weight when prioritising. The
  top-to-bottom order of the blueprint shapes study time: D2 Applications & Integration
  33.1% > D5 Model Selection 16.8% > D1 Agents & Workflows 14.7% > D6 Prompt/Context 11.0%
  > D8 Tools & MCPs 10.6% > D7 Security 8.1% > D3 Claude Code 3.1% > D4 Evals/Debug 2.6%.
- API-mechanics questions: state the exact call shape and the failure behaviour.
- Agent questions: name the orchestration pattern and why a simpler one does not suffice.
- Cost questions: model tier + context strategy + batch-where-appropriate, with the
  latency/quality trade-off stated.
- Never claim exam content verbatim; use the blueprint and discipline above as the spine.
  Facts are time-sensitive (exam guide v1.0, effective July 2026; logistics re-verified
  2026-10-13); re-verify fees, access, and prep availability against
  [sources/claude-cert/README.md](../../../sources/claude-cert/README.md) before advising.

## What "good" looks like

- [ ] The user can stand up a working end-to-end integration: prompt + tool + agent loop +
      structured output + a human-approval gate, with cost and latency stated.
- [ ] The user can produce the architecture decision record: users, data read, step order,
      what each tool may do, what happens on step failure, how it is tested.
- [ ] The user can write an eval that catches a real failure mode, and state the model
      tier and context strategy chosen for a given cost/quality constraint.
