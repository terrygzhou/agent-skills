# CCDV-F Blueprint (exam guide v1.0, effective July 2026)

- **Exam code**: CCDV-F (Claude Certified Developer - Foundations)
- **Audience**: AI/ML engineers, technical leads, senior software engineers who build,
  integrate, and ship Claude-powered applications, agents, and workflows. Recommended:
  1-5 years software engineering, 6+ months hands-on with Claude or comparable LLM
  systems, Python and/or TypeScript proficiency, REST + CLI fluency, working LLM /
  agent / MCP fundamentals. Recommended, not required.
- **Format**: 53 items (fewest of the four), standalone MC + multiple-response, 120 min,
  pass 720/1000, fee $125 USD, 12-month validity. Counts toward the Claude Partner
  Network tier.
- **Two-level blueprint**: 8 domains broken into 25 individually weighted sub-skills.
  The weights are unusually skewed - a third of the exam sits in one domain.

## Eight domains (official weights, heaviest first)

| # | Domain | Weight |
|---|---|---|
| 2 | Applications and Integration | 33.1% |
| 5 | Model Selection and Optimisation | 16.8% |
| 1 | Agents and Workflows | 14.7% |
| 6 | Prompt and Context Engineering | 11.0% |
| 8 | Tools and MCPs | 10.6% |
| 7 | Security and Safety | 8.1% |
| 3 | Claude Code | 3.1% |
| 4 | Eval, Testing, and Debugging | 2.6% |

The top-to-bottom ratio (33.1% vs 2.6%) should shape study time directly.

## The 25 sub-skills (official weights)

**D2 Applications and Integration (33.1%)**
Claude Application Design 8.6% - Software Engineering Foundations 7.4% - Claude API
Mechanics 6.8% - Configuration Management 4.1% - Understanding Requirements 3.4% -
Systems Life Cycle 2.8%

**D5 Model Selection and Optimisation (16.8%)**
Technical Fundamentals 6.1% - LLM Fundamentals 5.2% - Cost and Token Management 2.8% -
Model Selection and Trade-offs 2.7%

**D1 Agents and Workflows (14.7%)**
Agent Construction with Claude 5.3% - Agent Patterns and Frameworks 4.9% - Agent
Architecture 4.5%

**D6 Prompt and Context Engineering (11.0%)**
Prompt Engineering 4.6% - Context Engineering 3.8% - Output Handling 2.6%

**D8 Tools and MCPs (10.6%)**
Tool Implementation 4.4% - Agentic Customisation 4.1% - MCP Server Development 2.1%

**D7 Security and Safety (8.1%)**
AI Application Security 3.2% - Guardrails and Safe Deployment 2.3% - Identity, Secrets,
and Key Management 1.6% - Claude Hooks 1.0%

**D3 Claude Code (3.1%)**
Claude Code Operation 3.1%

**D4 Eval, Testing, and Debugging (2.6%)**
Debugging and Error Handling 2.6%

## The decision, not the fact (per domain)

- **D2 Applications & Integration (the spine)**: understanding requirements -> systems
  life cycle -> API mechanics -> software engineering foundations -> application design
  -> configuration management. The exam tests whether you can stand up a well-engineered
  app against the Claude API: requirements traced to design, the API used correctly,
  config managed, the life cycle understood.
- **D5 Model selection**: LLM + technical fundamentals drive the choice; select on
  trade-offs (cost, latency, quality, capability); manage tokens and cost explicitly.
- **D1 Agents**: smallest architecture that meets the need (direct call / fixed workflow
  / agentic loop); construct with the Agent SDK; know the patterns and when each applies.
- **D6 Prompt & context**: system prompts, few-shot, constraints; context engineering
  (window as budget: retrieve, summarise, cache); output handling (structured, validated).
- **D8 Tools & MCPs**: each tool = narrow purpose + description + input schema + auth
  boundary + structured failure result; MCP servers map client<->server<->credentials
  <->allowed operations; agentic customisation extends the loop.
- **D7 Security**: application security, guardrails + safe deployment, hooks, identity
  and key management. Security is designed in, not bolted on.
- **D3 Claude Code**: operate under a permission model; durable project context; package
  workflows as Skills and plugins.
- **D4 Evals & debugging**: build evals that resemble real tasks; debugging + error
  handling - lightweight on the exam but never absent.

## Recurring themes

- Production-grade: "code that holds up when real users are depending on it" - a prompt
  that looks solid can fail on an untested input; a tool call can break halfway; a
  stream can interrupt; an agent can run past budget.
- Retry only when it can change the outcome (tools and model calls).
- Schema-compliant != semantically correct: tool_use + JSON schemas kill syntax errors
  only; add programmatic validation for meaning.
- The Batches API is a cost tool, not a speed tool: no SLA, never for user-facing
  real-time paths.
- Extended thinking is managed explicitly across multi-turn work, not assumed.

## Study plan shape (4 weeks)

- **Week 1**: D2 (33%): requirements->design traceability, Claude API mechanics
  (messages, streaming, tool use, batches), software engineering foundations, config
  management. Build one small end-to-end app against the API.
- **Week 2**: D5 + D6 (28%): model tiers + cost/token management; prompt engineering
  (system, few-shot, constraints) + context engineering. Redesign Week 1 app with the
  right tier and context strategy.
- **Week 3**: D1 + D8 (25%): agent patterns with the Agent SDK; tool schemas + MCP
  server development. Add a tool + agent loop + structured output + human-approval gate.
- **Week 4**: D7 + D3 + D4 (14%): guardrails, hooks, secrets; Claude Code operation;
  evals + debugging. Then 53-item timed mocks (target 900+); review every
  wrong-answer rationale; exam day.

Daily loop: 10 practice questions, read explanations, 1 anti-pattern. The skewed
weights are the study plan: spend a third of the time on Applications & Integration.

## Free prep (official, free registration on the Skilljar portal)

- CCDV-F prep course: MSO Foundations; Production-Grade Prompting, Agents & Tool Use;
  Claude Code, MCP & Integration; Production Engineering, Evals & Security; Accelerators
  & IP Contribution.
- Prerequisite courses recommended: Claude 101, Claude Code 101, Claude Platform 101,
  Claude Code in Action, AI Fluency: Framework & Foundations, Building with the Claude
  API, Introduction to MCP, Model Context Protocol: Advanced Topics, AI Capabilities and
  Limitations.
- Full third-party prep track at claudecertificationguide.com was "coming soon" as of
  2026-10-13; the free CCAR-F track shares the technical spine (agents, tools/MCP,
  prompting, context) and is a useful bridge.
