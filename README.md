# EyWALink agent skills

Curated agent skills for EyWALink: certification prep, engineering workflows, and operational
tooling. Modelled on [mattpocock/skills](https://github.com/mattpocock/skills):

- Skills live in `skills/<bucket>/<skill-name>/SKILL.md`, grouped into bucket folders.
- Every promoted skill has a one-line entry in this README and in its bucket README, with the
  name linked to its `SKILL.md`.
- Crawled/research sources live in `sources/<topic>/` with a registry (`README.md`) listing URL,
  crawl date, and notes - the skill references point there for primary-source re-verification.
- Repo governance lives in `.agents/` (writing docs, invocation, out-of-scope decisions).

## Buckets

- `skills/claude-cert/` - certification preparation skills: one skill per Anthropic Claude
  certification track (CCAO-F, CCDV-F, CCAR-F, CCAR-P) plus shared family references. As
  the program matures, other cert tracks join the same layout.

## Skills

| Skill | What it does |
|---|---|
| [claude-ccao-f](skills/claude-cert/ccao-f/SKILL.md) | CCAO-F (Associate - Foundations): get work done with Claude well - structured prompting, judging output, model/product selection, Projects config, responsible use - and prepare for the no-code cert |
| [claude-ccdv-f](skills/claude-cert/ccdv-f/SKILL.md) | CCDV-F (Developer - Foundations): build and ship production-grade Claude apps, agents, and workflows - API mechanics, tools/MCP, cost, evals, security - and prepare for the builder cert |
| [claude-ccar-f](skills/claude-cert/ccar-f/SKILL.md) | CCAR-F (Architect - Foundations): design Claude systems end to end - agentic architecture, tool/MCP, Claude Code, prompt engineering, context and reliability - and prepare for the only scenario-based cert |
| [claude-ccar-p](skills/claude-cert/ccar-p/SKILL.md) | CCAR-P (Architect - Professional): own a production Claude system - enterprise integration, evaluation, governance/safety/risk, stakeholder communication, lifecycle, team enablement - and prepare for the senior cert |

## Conventions

- One task, one owner; skill updates go through the same review bar as any other deliverable:
  verify against the done-definition, record the check in the issue thread.
- Facts in skill references are time-sensitive; each carries a "as of" marker and a pointer to
  `sources/<topic>/` for re-verification.
- No em-dashes in skill prose; no unstyled placeholder content; every `SKILL.md` has valid
  frontmatter (`name`, `description`).
