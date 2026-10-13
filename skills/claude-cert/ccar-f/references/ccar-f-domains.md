# CCAR-F Domains & Sub-topics

Official weights (exam guide v1.0):

| # | Domain | Weight |
|---|---|---|
| 1 | Agentic Architecture & Orchestration | 27% |
| 2 | Tool Design & MCP Integration | 18% |
| 3 | Claude Code Configuration & Workflows | 20% |
| 4 | Prompt Engineering & Structured Output | 20% |
| 5 | Context Management & Reliability | 15% |

**Domains 1 + 5 = 42%** - if you only study two areas deeply, these are them.

## 30 sub-topics (1.1-5.6)

**D1 Agentic Architecture & Orchestration (27%)**
1.1 agentic loops - 1.2 coordinator & subagent patterns - 1.3 subagent invocation & context passing - 1.4 workflow enforcement & handoff - 1.5 Agent SDK hooks - 1.6 task decomposition - 1.7 session state, resumption & forking

**D2 Tool Design & MCP Integration (18%)**
2.1 tool interface design - 2.2 structured errors for MCP tools - 2.3 tool distribution & tool choice - 2.4 MCP server integration - 2.5 built-in tools

**D3 Claude Code Configuration & Workflows (20%)**
3.1 CLAUDE.md hierarchy - 3.2 slash commands & skills - 3.3 path-specific rules - 3.4 plan mode vs direct execution - 3.5 iterative refinement - 3.6 Claude Code in CI/CD

**D4 Prompt Engineering & Structured Output (20%)**
4.1 prompts with explicit criteria - 4.2 few-shot prompting - 4.3 structured output with JSON schemas - 4.4 validation & retry loops - 4.5 Message Batches API - 4.6 multi-pass review

**D5 Context Management & Reliability (15%)**
5.1 context across long conversations - 5.2 escalation & ambiguity - 5.3 error propagation - 5.4 large codebase context - 5.5 human review & confidence - 5.6 information provenance

## What to study per domain (the decision, not the fact)

- **Orchestration**: start from the smallest architecture that meets the requirement (direct call / fixed workflow / agentic loop). Name the owner, state carried forward, and the human-decision moment per step. A coordinator needs a bounded task + clear hand-off + consumable result format. Design for partial failure before adding agents.
- **Claude Code**: CLAUDE.md is the persistent architectural rulebook (conventions, test commands, rules, approval-gated actions). Owning architecture = deciding how generated changes are checked (review stages, branch controls, pre-release evidence).
- **Tools & MCP**: each tool = narrow purpose + usable description + input schema + auth boundary + structured failure result. MCP: map client<->server<->credentials<->allowed operations; the trust boundary matters as much as the interface.
- **Structured output & errors**: define fields/types/required evidence/validation. Record unknown/incomplete data so a consumer never treats it as a confident answer. Failed lookup / malformed response / timeout needs a controlled path; retry only when it can change the outcome.
- **Context & reliability**: retrieve/summarise/cache with a stated purpose; keep sensitive data in the smallest boundary. Reliability = evaluations that resemble real tasks: labelled set, success criteria, review process. Measure quality beside latency, token use, tool availability.

## Recurring exam themes

- Evidence/provenance preservation: preserve source references as docs are processed; a fluent paragraph without source references is not a usable result.
- Retry only when it can change the outcome (tools AND model calls).
- An architecture decision record beats a diagram without rationale: name users, data, step order, tool actions, failure behaviour, test plan.
- Schema-compliant != semantically correct: structured output via tool_use + JSON schemas kills syntax errors only; add programmatic validation for meaning.
- The Batches API is a cost tool, not a speed tool: no SLA, never for user-facing real-time paths.

## 4-week study plan shape

- **Week 1**: Domains 1 + 5 (42%): agentic-loop mental model, coordinator/subagent, handoffs, session state/forking, context preservation & provenance.
- **Week 2**: Domains 3 + 4 (40%): CLAUDE.md hierarchy, rules globs, slash commands/skills, plan vs direct, few-shot, tool_use + JSON schemas, validation-retry loops, Batches API, multi-pass review.
- **Week 3**: Domain 2 + integration + hands-on: MCP primitives, tool schemas + auth boundaries, structured errors, .mcp.json; build one small end-to-end system (tool + agent + structured output + human-approval gate).
- **Week 4**: timed mocks (target 900+), review every wrong-answer rationale; exam Day 28.

Daily loop: ~10 practice questions, read explanations, 1 anti-pattern. The scenario exam rewards hands-on judgment, not recall.
