# Contributing

Keep skills practical, provider-aware, and safe for imported Type sidekicks.

## Guidelines

- Put every importable skill in `skills/<slug>/SKILL.md`.
- Use frontmatter with `name` and `description`.
- Keep private account data, customer data, credentials, and API tokens out of the repo.
- Default to recommendations and drafts for Ads mutations unless a skill clearly describes approval requirements.
- Separate measurement policy from change policy. A reporting rule should not silently grant permission to edit campaigns.
- Prefer concise workflows that can run with connected tools the user already has in Type.

## Review Checklist

- Does the skill name describe the job clearly?
- Does the description include when to use the skill?
- Are data sources discovered before use?
- Are date range, timezone, currency, and conversion definitions explicit?
- Are destructive or high-risk changes gated behind approval?
- Is output short enough for a human operator to act on?

