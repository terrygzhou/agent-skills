---
name: claude-ccao-f
description: Companion for Anthropic's Claude Certified Associate - Foundations (CCAO-F) cert and for doing the Associate's actual job: structured prompting, judging Claude output, picking model/product features, configuring Claude Projects, and responsible use. Use when preparing for CCAO-F, or when a non-code knowledge worker needs to get work done with Claude well. Not for API/MCP building (that is CCDV-F/CCAR-F).
metadata:
  short-description: CCAO-F certification + everyday Claude-as-productivity-tool skill
---

# Claude CCAO-F (Associate - Foundations)

Two uses, one skill: (a) get an agent skillful at the Associate job itself - prompting well,
judging output, choosing models and product features, configuring Projects, using AI
responsibly - and (b) prepare for the CCAO-F exam (60 items, 7 domains, 120 min, pass
720/1000, $99 USD, the programme's no-code credential).

Read [references/ccao-f-blueprint.md](references/ccao-f-blueprint.md) for the 7-domain
blueprint with official weights and sub-topics, and the "what good looks like" per domain.
Read [references/ccao-f-logistics.md](references/ccao-f-logistics.md) for access, fees,
retake/renewal, and free prep. Read
[../references/claude-cert-family.md](../references/claude-cert-family.md) for the
four-cert family and role routing.

## The Associate's discipline (task guidance)

The Associate's value is not generating text; it is knowing whether the text is right,
complete, and safe to ship. Output Evaluation and Validation is the heaviest exam domain
(21%) for a reason - that judgement is the whole job.

- **Before prompting, set the ceiling**: pick the entry point (Projects / chat / research
  mode / artifacts), the model tier (Haiku cheap+fast, Sonnet balanced, Opus strongest),
  and the context strategy. These four decisions (entry point, feature, model, context)
  bound everything that follows.
- **Prompt as a communication discipline**: use a repeatable structure - task, context,
  constraints, output format, audience. Decompose complex requests into steps; iterate
  diagnostically (identify which component failed, fix that one, re-run) instead of
  rewriting the whole prompt.
- **Evaluate before shipping**: accuracy and completeness; hallucination, inconsistency,
  and bias; when to fact-check against a source; when a human must verify (irreversible,
  high-stakes, externally-facing outputs). Edit, adapt, and reformat for the intended
  audience. A fluent paragraph without provenance is not a usable deliverable.
- **Integrate, don't just use**: decide which steps of a workflow to delegate to Claude
  and which to keep human; communicate Claude's value and limits to stakeholders
  accurately - never oversell.
- **Configure once, benefit always**: Claude Projects with the right instructions and
  knowledge sources (uploads, connectors); keep instructions current so they stop
  contradicting reality.
- **Governance is the 15% domain**: data sensitivity, privacy, and regulatory fit
  before use; appropriate vs inappropriate use cases; follow organisational AI policy.
  Escalate technical/complex work to developers or architects - recognising the limit of
  your remit is itself a tested skill.
- **Troubleshoot by root cause**: underperforming output -> prompt defect, missing
  context, wrong model/feature, or task mismatch; fix the cause so it persists.

## How to answer exam-style questions

- Lead with the decision and its trade-off; cite the domain weight when prioritising:
  Output Evaluation + Governance + Workflow Integration = 52% is the spine; Prompting +
  Configuration + Model Selection = 38%; Troubleshooting = 10%.
- Model-tier questions: match cost/speed/quality to the task - Haiku for volume/cheap,
  Sonnet default, Opus when quality is the constraint.
- Context questions: when to restart, summarise, or persist knowledge in a Project.
- Never claim exam content verbatim; use the blueprint and discipline above as the spine.
  Facts are time-sensitive (exam guide v1.0, effective July 2026; logistics re-verified
  2026-10-13); re-verify fees, access, and prep availability against
  [sources/claude-cert/README.md](../../../sources/claude-cert/README.md) before advising.

## What "good" looks like

- [ ] The user can operate Claude end to end on a real task: pick entry point + model +
      context, write a structured prompt, decompose the task, iterate diagnostically.
- [ ] The user can reject a plausible-but-wrong output and say exactly why (accuracy,
      completeness, provenance, bias) and what would make it shippable.
- [ ] The user can stand up a Claude Project (instructions + knowledge) that another
      person can reuse, and state the governance checks (data sensitivity, policy fit)
      that must pass before first use.
