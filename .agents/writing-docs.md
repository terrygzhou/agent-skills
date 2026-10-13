# Writing skill docs

- SKILL.md: frontmatter with `name` (kebab-case, unique in repo) and `description` (one line,
  names the capability + when it applies). Body: purpose, the essential workflow, real
  constraints, and links to references. No generic advice the model already knows.
- references/: material needed only in particular contexts (fact cards, logistics, checklists).
  SKILL.md links each reference where its use becomes relevant.
- sources/: crawled primary sources with a registry. Skill references must stay verifiable
  against it; re-crawl when the "as of" marker goes stale.
- Keep facts current: every time-sensitive fact carries an "as of" date.
