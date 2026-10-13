# Invocation

Every skill is either user-invoked or model-invoked.

- **Model-invoked** (default): the skill's name + description enter the model's context; the
  model reaches for it when the description matches. Keep descriptions short and discriminating.
- **User-invoked**: set `disable-model-invocation: true` in frontmatter (and
  `policy.allow_implicit_invocation: false` in `agents/openai.yaml` when present) so only a
  human can invoke it by name.

When in doubt, default to model-invoked: certification-prep skills should surface when a user
mentions the cert.
