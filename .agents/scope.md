# Scope

This repo is the set of agent skills EyWALink actually uses. It is curated:

- A new skill clears the bar if it describes an observed need (a task that failed without it)
  and does not duplicate an existing skill.
- Certification skills map 1:1 to a certification track; track-level routing (which cert for
  which role) lives in the track skill, not in a separate router skill.
- Out-of-scope: single-person preferences (put them in your own CLAUDE.md / AGENTS.md),
  harness-specific branches, and config-option bloat.
