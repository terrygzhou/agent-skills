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

- `skills/claude-cert/` - certification preparation skills (Claude certs and, as the program
  matures, other cert tracks)

## Skills

| Skill | What it does |
|---|---|
| [claude-ccar-f](skills/claude-cert/ccar-f/SKILL.md) | Study companion for the CCAR-F exam: domains, anti-patterns, logistics, cert-family routing |

## Conventions

- One task, one owner; skill updates go through the same review bar as any other deliverable:
  verify against the done-definition, record the check in the issue thread.
- Facts in skill references are time-sensitive; each carries a "as of" marker and a pointer to
  `sources/<topic>/` for re-verification.
- No em-dashes in skill prose; no unstyled placeholder content; every `SKILL.md` has valid
  frontmatter (`name`, `description`).
