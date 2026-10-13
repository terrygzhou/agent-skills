# claude-cert source registry (crawled 2026-10-13)

Primary sources behind `skills/claude-cert/` (all four tracks). Facts are time-sensitive
(exam guide v1.0, effective July 2026; logistics re-verified 2026-10-13); re-verify
fees, access paths, and prep availability here before advising. Per-track detail lives
in the skill's own references; this registry is the single re-verification point.

| Source | URL | Crawled | Note |
|---|---|---|---|
| Anthropic Partner Academy - Partner Certifications (Skilljar) | https://anthropic-partners.skilljar.com/page/partner-certifications | 2026-10-13 | all 4 certs: codes, pricing table ($99/$125/$125/$175), tier counting (CCAO-F excluded), role descriptions, SME network |
| Anthropic Partner Academy - Certification FAQ | https://anthropic-partners.skilljar.com/page/faq-certifications | 2026-10-13 | program overview, eligibility/access (partner-only, 18+, email-domain rules), registration (5-yr validity), ID, retakes (14/30/90, max 4/12mo), recert, OnVUE exclusions, appeals |
| Anthropic Partner Academy - Certification Policies | https://anthropic-partners.skilljar.com/page/policies-certifications | 2026-10-13 | reschedule/cancel 48h rule, retake cadence, 12-month validity, on-time free recert, proctoring/conduct, appeals (14 days) |
| Skilljar - CCAO-F certification page | https://anthropic-partners.skilljar.com/claude-certified-associate-foundations-certification | 2026-10-13 | register-and-pay flow; exam guide + 3 PDFs linked there |
| Skilljar - CCDV-F certification page | https://anthropic-partners.skilljar.com/claude-certified-developer-foundations-certification | 2026-10-13 | register-and-pay flow; exam guide + 3 PDFs linked there |
| Skilljar - CCAR-F certification page | https://anthropic-partners.skilljar.com/claude-certified-architect-foundations-certification | 2026-10-13 | register-and-pay; $125; 3 PDFs (Exam Guide, T&Cs, Exam Policy) - S3-hosted |
| Skilljar - CCAR-P certification page | https://anthropic-partners.skilljar.com/claude-certified-architect-professional-certification | 2026-10-13 | register-and-pay; learning objectives; recommended prerequisites |
| Skilljar - CCAO-F prep course | https://anthropic-partners.skilljar.com/path/claude-certified-associate-foundations | 2026-10-13 | 8 lessons (Platform & Model Foundations; Prompting & Task Execution; Evaluating & Validating Output; Workflow Integration & Solution Design; Configuration & Knowledge Management; Governance, Risk & Responsible Use; Troubleshooting & Optimization; Course Summary) |
| Skilljar - CCDV-F prep course | https://anthropic-partners.skilljar.com/path/claude-certified-developer-foundations | 2026-10-13 | 5 lessons (MSO Foundations; Production-Grade Prompting, Agents & Tool Use; Claude Code, MCP & Integration; Production Engineering, Evals & Security; Accelerators & IP Contribution) |
| Skilljar - CCAR-P prep course | https://anthropic-partners.skilljar.com/path/claude-certified-architect-professional | 2026-10-13 | 5 lessons (Platform & Solution Design; Enterprise Integration & Production; Responsible AI, Safety & Risk; Stakeholder Engagement, Lifecycle & GTM; Team Enablement & Operational Productivity) |
| CCG - CCAO-F blueprint | https://claudecertificationguide.com/ccao-f | 2026-10-13 | exam facts table + 7-domain blueprint with official weights and sub-topics; full prep track "coming soon" as of 2026-10-13 |
| CCG - CCDV-F blueprint | https://claudecertificationguide.com/ccdv-f | 2026-10-13 | exam facts table + 8-domain/25-sub-skill blueprint with official weights; full prep track "coming soon" as of 2026-10-13 |
| CCG - CCAR-P blueprint | https://claudecertificationguide.com/ccar-p | 2026-10-13 | exam facts table + 7-domain blueprint with official weights and sub-topics; full prep track "coming soon" as of 2026-10-13 |
| CCG - four-cert overview | https://claudecertificationguide.com/blog/new-claude-certifications-2026 | 2026-10-13 | the 4-cert family, role-based routing, Foundations vs Professional split, shared mechanics |
| CCG - CCAR-F blueprint | https://claudecertificationguide.com/architect-foundations | 2026-10-13 | CCAR-F 5-domain blueprint; free CCAR-F curriculum (30 lessons, 250+ practice questions, timed mock) |
| CCG - CCAO-F exam guide post | https://claudecertificationguide.com/blog/claude-certified-associate-foundations-exam-guide | 2026-10-13 | CCAO-F deep-dive: audience, 7 domains, model tiers (Haiku/Sonnet/Opus), prep guidance |
| CCG - CCDV-F exam guide post | https://claudecertificationguide.com/blog/claude-certified-developer-foundations-exam-guide | 2026-10-13 | CCDV-F deep-dive: audience, 8 domains, Applications & Integration dominance (33.1%) |
| CCG - CCAR-P exam guide post | https://claudecertificationguide.com/blog/claude-certified-architect-professional-exam-guide | 2026-10-13 | CCAR-P deep-dive: audience, 7 domains, the 35% that separates Professional from Foundations |
| CCG - CCAR-F study guide post | https://claudecertificationguide.com/blog/how-to-pass-claude-certified-architect-exam | 2026-10-13 | CCAR-F study strategy, common traps, resources |
| CCG resources | https://claudecertificationguide.com/resources | 2026-10-13 | official docs, Anthropic cookbooks, MCP spec, Skilljar prep courses |
| TimoLabs CCAR-F exam guide | https://www.timolabs.dev/certifications/architect-foundations | 2026-10-10 | CCAR-F weights, 30-topic checklist, worked supplier-review example |
| Unofficial GitHub study guide | https://github.com/dnacenta/claude-certified-architect | 2026-10-10 | community CCAR-F study guide |
| Official docs (referenced, not crawled) | https://docs.anthropic.com, https://github.com/modelcontextprotocol, https://github.com/anthropics/anthropic-cookbook, https://github.com/anthropics/claude-agent-sdk-python | - | primary technical references the skills point to |

## Crawl notes

- 2026-10-13: crawled with direct HTTP fetches (crawl4ai not installed on this host; the
  2026-10-10 CCAR-F crawl used the same method, recorded in `sources/ccar-f/README.md`).
  All Skilljar and claudecertificationguide.com URLs returned HTTP 200 with no redirects
  away from the target host.
- Verified against the 2026-10-10 CCAR-F baseline: shared mechanics unchanged (120 min,
  pass 720/1000, 12-month validity, 14/30/90-day retake cadence, 48h reschedule/cancel
  window, name-mismatch rule, Pearson VUE delivery).
- Pricing confirmed from the official Partner Certifications page and Certification FAQ:
  CCAO-F $99, CCDV-F $125, CCAR-F $125, CCAR-P $175 (USD, before partner-tier discount).
  CCAO-F is the only cert that does not count toward Claude Partner Network tier
  eligibility.
- Domain weights and sub-topics for all four tracks taken verbatim from the CCG
  blueprint pages (exam guide v1.0, effective July 2026). Re-crawl when the "as of"
  marker goes stale or a new exam-guide version is published.
