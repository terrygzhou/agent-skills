---
name: claude-ccar-p
description: Companion for Anthropic's Claude Certified Architect - Professional (CCAR-P) cert and for doing the senior-architect's actual job: owning a production Claude system end to end - solution design, enterprise integration, evaluation, governance/safety/risk, stakeholder communication, lifecycle, and team enablement. Use when preparing for CCAR-P or when accountable for a production Claude system in front of stakeholders, auditors, and a roadmap. Not for first-time architecture (CCAR-F) or no-code work (CCAO-F).
metadata:
  short-description: CCAR-P certification + senior Claude-system ownership skill
---

# Claude CCAR-P (Architect - Professional)

Two uses, one skill: (a) get an agent skillful at the senior-architect job - owning a
production Claude system end to end, including the conversations that surround the build
- and (b) prepare for the CCAR-P exam (63 items, 7 domains, 120 min, pass 720/1000,
$175 USD, the most senior of the four credentials; counts toward the Claude Partner
Network tier). Professional does not require Foundations; if it matches the user's work,
sit it directly.

Read [references/ccar-p-blueprint.md](references/ccar-p-blueprint.md) for the 7-domain
blueprint with official weights, sub-topics, and the "what good looks like" per domain.
Read [references/ccar-p-logistics.md](references/ccar-p-logistics.md) for access, fees,
retake/renewal, and free prep. Read
[../references/claude-cert-family.md](../references/claude-cert-family.md) for the
four-cert family and role routing, and [../ccar-f/references/ccar-f-domains.md](../ccar-f/references/ccar-f-domains.md)
for the Foundations domains this exam builds on.

## The senior architect's discipline (task guidance)

Where CCAR-F tests whether a working system can be designed, CCAR-P tests whether it can
be owned: build it, ship it, defend the decisions to stakeholders, and keep it safe and
compliant over its lifecycle.

- **Solution design first, code never**: reference architecture, model, context strategy,
  and entry point are chosen before anyone writes a line of code; a wrong reference
  architecture is expensive to switch. Translate an ambiguous business problem into a
  scoped Claude solution; align to business value pillars (efficiency, transformation,
  productivity, cost, performance SLAs).
- **Integration is the heaviest domain (19%)**: production Claude systems live inside a
  mess of existing enterprise systems. Evaluate tool/agent configuration for capability
  bloat; authn/z gaps; accuracy-latency trade-offs; observability at scale; RAG pipeline
  design (chunking, indexing, retrieval matched to data shape and query pattern);
  connection-protocol choice (MCP, API/CLI, agent-to-agent); progressive discovery vs
  monolithic context.
- **Safety stack is placed, not assumed**: input screening, output screening, and
  tool-call authorization, with the system failing closed rather than open when a control
  fails. Guardrails and safety controls; LLM failure modes; human-in-the-loop
  validation; compliance (GDPR, HIPAA, FedRAMP, etc.); ethics (bias, fairness,
  transparency).
- **Evals are the gate**: build evaluations as acceptance criteria; use them as the gate
  before any model or architecture change. Define metrics (accuracy, latency, cost,
  safety, security); mixed-methodology datasets; A/B testing; diagnose prompt failure /
  hallucination / model mismatch; optimise token/latency/cost; monitor with logging and
  observability.
- **Route decisions deliberately**: route each decision to the right reviewer based on
  confidence, reversibility, and cost; map each compliance obligation to a named
  control, owner, and evidence artifact.
- **Stakeholder work is 14% of the exam**: structured discovery with non-technical
  stakeholders; present architectural trade-offs they can act on; manage feedback loops
  and expectation alignment (including SLAs); document architectures with
  implementation guidance; support the full lifecycle (discovery, design, handoff,
  monitoring, iteration). Design a handoff that survives your absence.
- **Enable the team (7%)**: configure Claude tools/environments for the team (e.g.
  Claude Code); AI-assisted developer workflows; operational issue resolution - so the
  team can run the system without depending on you.

## How to answer exam-style questions

- Lead with the decision and its trade-off; cite the weight when prioritising:
  Integration 19% + Solution Design 17% + Evals 16% = 52% is the spine; Governance
  14% + Stakeholder 14% = 28% is what separates this exam from Foundations; Models &
  Prompting 13% + Enablement 7%.
- Architecture questions: state the pattern chosen (workflow, agentic, augmented LLM)
  and why a simpler one does not suffice; name what each tool may do and what happens on
  step failure.
- Risk questions: name the control, the owner, the evidence artifact; fail closed.
- Stakeholder questions: the handoff test - "a design only you understand falls apart
  the moment you leave the room."
- Never claim exam content verbatim; use the blueprint and discipline above as the
  spine. Facts are time-sensitive (exam guide v1.0, effective July 2026; logistics
  re-verified 2026-10-13); re-verify fees, access, and prep availability against
  [sources/claude-cert/README.md](../../../sources/claude-cert/README.md) before advising.

## What "good" looks like

- [ ] The user can take an ambiguous business problem to a scoped Claude architecture:
      reference architecture, model, context strategy, entry point, and the business
      value pillars it serves - with the cost/latency/reliability-to-budget mapping.
- [ ] The user can produce the full safety stack placement (input screening, output
      screening, tool-call authorization, fail-closed behaviour) and the eval that gates
      every model or architecture change.
- [ ] The user can run the stakeholder pass: structured discovery, trade-off presentation
      a non-technical audience can act on, and a handoff document that survives the
      architect's absence.
