# CCAR-F source registry (crawled 2026-10-10, re-crawled 2026-10-13)

These are the primary sources behind `skills/claude-cert/ccar-f/`. Facts are time-sensitive
(exam guide v1.0, effective July 2026); re-verify dates, fees, and access paths here before
advising. Study notes live in the Obsidian vault at
`~/workspace/Obsidian Vault/Agentic/claude-cert/` (one deep-dive note per source).

| Source | URL | Crawled | Note |
|---|---|---|---|
| Anthropic Partner Academy (Skilljar) | https://anthropic-partners.skilljar.com/claude-certified-architect-foundations-certification | 2026-10-13 | official scope + the 3 PDFs to read; register-and-pay flow |
| Pearson VUE exam program | https://www.pearsonvue.com/us/en/anthropic.html | 2026-10-13 | exam-day mechanics: name/ID, 48h rule, retakes |
| Credly digital badge | https://www.credly.com/org/anthropic/badge/claude-certified-architect-foundations | 2026-10-13 | credential + official 11-skill taxonomy |
| 2026 four-cert guide | https://claudecertificationguide.com/blog/new-claude-certifications-2026 | 2026-10-13 | the 4-cert family + how to pick by role |
| TimoLabs CCAR-F exam guide | https://www.timolabs.dev/certifications/architect-foundations | 2026-10-13 | domain weights, 30-topic checklist, worked supplier-review example |
| Complete guide (anti-patterns, 6-scenario bank) | https://usefusefi.medium.com/the-complete-guide-to-the-claude-certified-architect-foundations-cca-f-13f3f1af605c | 2026-10-13 | the 7 anti-patterns + scenario bank + access path |
| Unofficial GitHub study guide | https://github.com/dnacenta/claude-certified-architect | 2026-10-13 | community study guide |

## Re-crawl verification (2026-10-13, crawl4ai)

All 7 URLs crawled successfully with crawl4ai (Playwright headless, all HTTP 200, no redirects
away from the target host). Verified unchanged against the 2026-10-10 baseline:

- Fee US$125, 12-month validity, 60 items / 5 domains / 120 min, pass 720/1000: unchanged.
- Domain weights (27/18/20/20/15) and 30 sub-topic structure: unchanged.
- 4-cert family (CCAO-F / CCDV-F / CCAR-F / CCAR-P) and shared mechanics
  (120 min, 720/1000 pass, 12-month validity, guide v1.0 eff. July 2026): unchanged.
- Retake cadence (14/30/90 days, max 4 per rolling 12 months) and 48h reschedule/cancel
  window (fee forfeited inside 48h): unchanged.
- Pearson VUE name-mismatch rule (no entry + fee forfeited) and the 24h name-correction
  window: unchanged.

## Crawl notes

- 2026-10-10: direct page fetches (crawl4ai not yet installed).
- 2026-10-13: re-crawled with crawl4ai. One real change: the Skilljar portal moved from
  `anthropic.skilljar.com` to `anthropic-partners.skilljar.com` (old URL now redirects) and the
  CCAR-F page is a register-and-pay page (`Price $125 USD`), not an access-request page. The
  launch fee-waiver ("first 5,000 partner-employee seats fee-waived at launch") no longer
  appears anywhere on the portal - launch has passed; the fee is standard. See
  `skills/claude-cert/ccar-f/references/ccar-f-logistics.md` for the updated access path.
- Scenario bank (CCAR-F): 4 scenarios drawn at random from a bank of 6 - customer support
  agents, code generation, multi-agent research, developer productivity, CI integration,
  structured data extraction.
