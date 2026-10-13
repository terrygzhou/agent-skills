# Claude Certification Family (as of exam guide v1.0, effective July 2026; logistics re-verified 2026-10-13)

## The four certifications

| Code | Credential | Audience | Items | Domains | Format | Fee (USD) | Counts to Partner Network tier |
|---|---|---|---|---|---|---|---|
| CCAO-F | Claude Certified Associate - Foundations | Business/productivity users, no code required | 60 | 7 | Standalone MC + multiple-response | $99 | No |
| CCDV-F | Claude Certified Developer - Foundations | Engineers building/shipping Claude apps | 53 | 8 | Standalone MC + multiple-response | $125 | Yes |
| CCAR-F | Claude Certified Architect - Foundations | Solution architects designing Claude systems | 60 | 5 | Scenario-based (4 of 6 scenarios) | $125 | Yes |
| CCAR-P | Claude Certified Architect - Professional | Senior architects owning production Claude systems end to end | 63 | 7 | Standalone MC + multiple-response | $175 | Yes |

## Shared mechanics (all four)

- 120 min test time; plan ~135 min total seat time (check-in, instructions, post-exam survey).
- Pass: scaled 720 on a 100-1,000 scale (not 72%).
- Delivery: Pearson VUE, online proctored (OnVUE) or test centre.
- Validity: 12 months from award. On-time renewal = free non-proctored assessment on the Anthropic Partner Academy (extends validity 12 months from current expiry; may be retaken as needed). Lapsed = full resit at full fee.
- Retakes: wait 14 days after 1st failed attempt, 30 days after 2nd, 90 days after 3rd. Max 4 attempts per exam per rolling 12 months. Each attempt costs the standard fee; partner discount applies to retakes the same way. Passing bars re-take to improve score.
- Registration: valid 5 years from purchase; schedule within that window, no sitting deadline.
- ID: valid unexpired government-issued ID; name must match registration exactly (mismatch = no entry + fee forfeited). Age 18+ verified at check-in.
- Reschedule/cancel: free and full-refund at least 48h before the appointment; inside 48h (or no-show) forfeits the fee.
- Results: pass/fail with scaled score plus percent-correct by domain.

## Access path (the real bottleneck)

- Certification is open to people at **Claude Partner Network** organisations. Registration requires a partner email on a recognized company domain; personal emails fail. Customers/non-partners are currently excluded.
- Portal: `anthropic-partners.skilljar.com` (old `anthropic.skilljar.com` redirects). Each certification page has the exam guide, prep courses, and the register-and-pay link.
- Unknown email domains: email partner-support@anthropic.com; domain addition takes 7-10 days - request before planning a sit date.
- OnVUE exclusions: IDs from Belarus, Cuba, North Korea, Russia, Syria, or restricted regions of Ukraine are not eligible for online proctoring (use a test centre). Iran has a separate OFAC-driven policy.
- Individual without a qualifying org: start the free prep courses on the Skilljar portal immediately; broader public access was expected later in 2026 (no confirmed timeline).

## Role routing (pick by job, not difficulty)

- No-code productivity users who judge output, pick models/features, and configure Projects -> CCAO-F.
- Engineers shipping Claude apps through the API, Agent SDK, Claude Code, MCP -> CCDV-F.
- Architects owning end-to-end system design (the only scenario exam) -> CCAR-F.
- Senior architects accountable for production systems in front of stakeholders, auditors, roadmaps (governance, safety, risk, lifecycle) -> CCAR-P.
- No cert lists another as a prerequisite; recommended experience is recommended, not required. Professional does not require Foundations.

## Free prep (gated via Skilljar, free registration)

- CCAO-F prep course: Claude Platform & Model Foundations; Prompting & Task Execution; Evaluating & Validating Claude's Output; Workflow Integration & Solution Design; Configuration & Knowledge Management; Governance, Risk & Responsible Use; Troubleshooting & Optimization; Course Summary.
- CCDV-F prep course: MSO Foundations; Production-Grade Prompting, Agents & Tool Use; Claude Code, MCP & Integration; Production Engineering, Evals & Security; Accelerators & IP Contribution.
- CCAR-P prep course: Claude Platform & Solution Design; Enterprise Integration & Production; Responsible AI, Safety & Risk for Architects; Stakeholder Engagement, Lifecycle & GTM; Team Enablement & Operational Productivity.
- CCAR-F prep: Architect Foundations prep courses on the portal.
- Recommended prerequisite courses across tracks: Claude 101, Claude Code 101, Claude Platform 101, Claude Code in Action, AI Fluency: Framework & Foundations, Building with the Claude API, Introduction to MCP (+ Advanced Topics for CCDV-F), AI Capabilities and Limitations.
- Three PDFs to read before any exam: Exam Guide, Certification Terms & Conditions, Anthropic Certification Exam Policy (linked from the certification page).

## Unofficial resources

- claudecertificationguide.com: per-cert blueprint pages (`/ccao-f`, `/ccdv-f`, `/architect-foundations`, `/ccar-p`); free CCAR-F curriculum (30 lessons, 250+ practice questions, timed mock). CCAO-F/CCDV-F/CCAR-P full prep tracks were "coming soon" as of 2026-10-13.
- TimoLabs CCAR-F exam guide (weights, 30-topic checklist, worked example).
- github.com/dnacenta/claude-certified-architect (community study guide).
- Official docs: docs.anthropic.com (API, prompt engineering, agent SDK), github.com/modelcontextprotocol (MCP spec), github.com/anthropics/anthropic-cookbook.
