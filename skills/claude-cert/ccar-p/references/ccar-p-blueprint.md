# CCAR-P Blueprint (exam guide v1.0, effective July 2026)

- **Exam code**: CCAR-P (Claude Certified Architect - Professional)
- **Audience**: mid- to senior-level solution architects, AI/ML engineers, technical
  leads, senior software engineers, across regulated/complex sectors (financial
  services, healthcare, retail, technology, education, government). Recommended: 3+
  years in systems architecture or platform engineering, 6+ months hands-on with Claude
  or comparable LLM systems in production, real end-to-end delivery. Recommended, not
  required. Not a fit for entry-level developers or prompt-only roles.
- **Format**: 63 items, standalone MC + multiple-response, 120 min, pass 720/1000, fee
  $175 USD (the highest of the four), 12-month validity. Counts toward the Claude
  Partner Network tier.
- **Relationship to CCAR-F**: separate exam; no prerequisite. Foundations is
  scenario-based, 60 items, 5 domains, ~6 months typical experience. Professional is
  standalone, 63 items, 7 domains, 3+ years typical experience. If Professional matches
  the user's work, sit it directly.

## Seven domains (official weights, heaviest first)

| # | Domain | Weight |
|---|---|---|
| 3 | Integration | 19% |
| 1 | Solution Design & Architecture | 17% |
| 4 | Evaluation, Testing & Optimisation | 16% |
| 5 | Governance, Safety & Risk Management | 14% |
| 6 | Stakeholder Communication & Lifecycle Management | 14% |
| 2 | Claude Models, Prompting & Context Engineering | 13% |
| 7 | Developer Productivity & Operational Enablement | 7% |

**Integration + Solution Design + Evals = 52%** is the spine; the three domains that mark
Professional out from Foundations (Governance, Stakeholder, Enablement) are 35% of the
exam and none appear on the Foundations blueprint.

## Sub-topics per domain

**D3 Integration (19%)**
3.1 evaluate tool/agent configuration for capability bloat - 3.2 analyse authn/z
requirements to identify security gaps - 3.3 evaluate accuracy-latency trade-offs and
justify configuration decisions - 3.4 analyse observability challenges; select
monitoring strategies at scale - 3.5 design a RAG pipeline with appropriate chunking
and indexing - 3.6 apply retrieval strategies matched to data shape and query pattern -
3.7 evaluate connection protocols; select the integration mechanism (MCP, API/CLI,
agent-to-agent) - 3.8 evaluate progressive discovery vs monolithic context strategy

**D1 Solution Design & Architecture (17%)**
1.1 translate business problems into Claude-based AI solutions - 1.2 design end-to-end
architectures (input -> processing -> output -> feedback loops) - 1.3 select
architectural patterns (workflow, agentic, augmented LLM) - 1.4 design multi-agent
systems and orchestration strategies - 1.5 apply decomposition for complex problems -
1.6 align solutions to business value pillars (efficiency, transformation, productivity,
cost, performance SLAs)

**D4 Evaluation, Testing & Optimisation (16%)**
4.1 define evaluation metrics (accuracy, latency, cost, safety, security) - 4.2 design
evaluation datasets and test frameworks using mixed methodologies - 4.3 A/B testing and
iterative improvement - 4.4 diagnose system issues (prompt failure, hallucinations,
model mismatch) - 4.5 optimise token usage, latency, cost-performance trade-offs - 4.6
monitor system performance with logging and observability

**D5 Governance, Safety & Risk Management (14%)**
5.1 implement guardrails and safety controls - 5.2 identify risks, limitations, failure
modes of LLM systems - 5.3 apply human-in-the-loop validation - 5.4 ensure compliance
(GDPR, HIPAA, FedRAMP, etc.) - 5.5 address ethical AI (bias, fairness, transparency)

**D6 Stakeholder Communication & Lifecycle Management (14%)**
6.1 conduct structured discovery and requirement gathering - 6.2 communicate
architectural decisions and trade-offs - 6.3 manage stakeholder feedback loops and
expectation alignment (including SLAs) - 6.4 document architectures with
implementation guidance - 6.5 support lifecycle phases (discovery, design, handoff,
monitoring, iteration)

**D2 Claude Models, Prompting & Context Engineering (13%)**
2.1 select Claude models on trade-offs - 2.2 design system prompts, templates,
guardrails - 2.3 apply prompt engineering (zero-shot, few-shot, chain-of-thought) - 2.4
optimise context windows; manage token usage - 2.5 prompt reuse strategies (caching,
modular prompts, Skills)

**D7 Developer Productivity & Operational Enablement (7%)**
7.1 configure Claude tools and environments for teams (e.g. Claude Code) - 7.2 improve
developer workflows with AI-assisted tooling - 7.3 support debugging and operational
issue resolution

## The decision, not the fact (per domain)

- **Integration (19%, the spine)**: production Claude systems live inside existing
  enterprise systems; value is in connecting them well. Capability bloat, authn/z gaps,
  accuracy-latency, observability, RAG pipeline design, retrieval matched to data shape,
  protocol choice, progressive discovery vs monolithic context - each is a defensible
  call with a stated trade-off.
- **Solution Design (17%)**: the reference architecture, model, context strategy, and
  entry point are chosen before code; a wrong reference architecture is expensive to
  switch. Align to the business value pillars that fund the system.
- **Evals (16%)**: evals are acceptance criteria and the gate before any model or
  architecture change; diagnosis = prompt failure / hallucination / model mismatch.
- **Governance (14%)**: fail closed, not open; every compliance obligation maps to a
  named control, owner, and evidence artifact; human-in-the-loop where the cost of error
  is high.
- **Stakeholder (14%)**: "a design only you understand falls apart the moment you leave
  the room" - the handoff test; structured discovery, actionable trade-offs, SLA
  alignment, documentation that survives your absence.
- **Models & prompting (13%)**: selection on trade-offs; system prompts + guardrails;
  context as budget; reuse via caching, modular prompts, Skills.
- **Enablement (7%)**: the team runs the system without you - configured environments,
  AI-assisted workflows, operational issue resolution.

## What separates CCAR-P from CCAR-F (the three new domains, 35%)

- **Governance, Safety & Risk (14%)**: compliance (GDPR, HIPAA, FedRAMP, etc.),
  guardrail placement, failure modes, ethics - not present on Foundations.
- **Stakeholder Communication & Lifecycle (14%)**: discovery, communication, SLAs,
  handoff, lifecycle - not present on Foundations.
- **Developer Productivity & Enablement (7%)**: team tooling and operations - not
  present on Foundations.

## Recurring themes

- Own it end to end: build, ship, defend, keep safe over the lifecycle - the exam tests
  accountability, not just design.
- Fail closed: the safety stack must degrade safely; a control merely assumed fails at
  the worst moment.
- Route decisions deliberately: confidence, reversibility, cost decide who reviews what;
  multi-team, high-reversibility, high-cost decisions go to a committee with a named
  evidence artifact.
- Evals are the contract: acceptance criteria written before the build; the gate before
  every model or architecture change.
- Handoff that survives absence: documentation + a team that can operate without you.

## Study plan shape (4 weeks)

- **Week 1**: D3 + D1 (36%): integration patterns, RAG pipeline design, capability
  bloat, observability; solution design patterns (workflow, agentic, augmented LLM),
  multi-agent orchestration, business value pillars.
- **Week 2**: D4 + D5 (30%): eval design as acceptance criteria, metrics, A/B testing,
  diagnosis; guardrail placement, failure modes, compliance mapping, human-in-the-loop.
- **Week 3**: D6 + D2 (27%): structured discovery, trade-off communication, SLA
  alignment, handoff documentation; model selection on trade-offs, system prompts +
  guardrails, context budget, prompt reuse.
- **Week 4**: D7 + timed 63-item mocks (target 900+), review every wrong-answer
  rationale; exam day.

Daily loop: 10 practice questions, read explanations, 1 anti-pattern. The 35% that
separates Professional from Foundations is the study differentiator: governance,
stakeholder, enablement.

## Free prep (official, free registration on the Skilljar portal)

- CCAR-P prep course: Claude Platform & Solution Design; Enterprise Integration &
  Production; Responsible AI, Safety & Risk for Architects; Stakeholder Engagement,
  Lifecycle & GTM; Team Enablement & Operational Productivity.
- Prerequisite courses recommended: Claude 101, Claude Code in Action, AI Fluency:
  Framework & Foundations, Building with the Claude API, Introduction to Model Context
  Protocol, AI Capabilities and Limitations.
- The free CCAR-F track (claudecertificationguide.com) covers the technical spine
  (agentic architecture, tool/MCP design, Claude Code, prompt engineering, context
  management) this exam assumes; it will not cover the governance and stakeholder
  domains. Full third-party CCAR-P prep was "coming soon" as of 2026-10-13.
