---
name: claude-ccar-f
description: Study companion for Anthropic's Claude Certified Architect - Foundations (CCAR-F) exam. Use when preparing for or reviewing the CCAR-F certification, studying its domains/anti-patterns/logistics, or choosing among the four Claude certification tracks.
metadata:
  short-description: CCAR-F certification study skill
---

# Claude CCAR-F Study Companion

Use this skill to prepare for the **CCAR-F** exam and to route questions about the broader Claude certification family. The exam is scenario-based: 60 items, 5 domains, 120 min, pass 720/1000.

Read [references/ccar-f-facts.md](references/ccar-f-facts.md) for the quick-fact card and the four-certification family (CCAO-F / CCDV-F / CCAR-F / CCAR-P). Read [references/ccar-f-domains.md](references/ccar-f-domains.md) when a question is about domains, sub-topics, the anti-patterns, or how to study. Read [references/ccar-f-logistics.md](references/ccar-f-logistics.md) for exam-day mechanics, fees, retake policy, and access paths.

## How to answer

- Lead with the **decision and its trade-off**, not trivia. Scenario-format questions reward a defensible design call; the distractors are mistakes real engineers make.
- Cite the domain weight when prioritising: Domains 1+5 = 42% (agentic architecture + context/reliability) is the study backbone; Domains 3+4 = 40%; Domain 2 = 18%.
- When a user says "which cert should I take", route by role, not difficulty: no-code productivity users -> CCAO-F; engineers shipping Claude apps -> CCDV-F; architects owning system design -> CCAR-F; senior architects with governance/safety/risk ownership -> CCAR-P.
- Never claim exam questions or content verbatim; use the study notes and anti-patterns as the study spine. Facts are time-sensitive (exam guide v1.0, effective July 2026); re-verify dates, fees, and access paths against the primary sources in [sources/ccar-f/README.md](../../../sources/ccar-f/README.md) before advising.

## What "good" looks like

- [ ] The user can name the 30 sub-topics (1.1-5.6) and the 7 anti-patterns unaided.
- [ ] The user can produce an architecture decision record: users, data read, step order, what each tool may do, what happens on step failure, how it is tested.
- [ ] Logistics are settled: access path, Pearson profile name matches ID, reschedule window known (48h).
