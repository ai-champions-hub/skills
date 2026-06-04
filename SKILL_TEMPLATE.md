# Skill Package Template

Create installable skills as directories:

```text
skills/<skill-name>/
  SKILL.md
```

`SKILL.md` must start with YAML frontmatter:

```markdown
---
name: skill-name
description: Specific third-person description. Include what the skill does and when to use it.
---

# Skill Name

> One-line description: what goes in → what comes out.

## Context

<!-- When would someone use this skill? What problem does it solve? (2-3 sentences) -->

## Instructions

<!--
Step-by-step instructions for the AI. Write these as if you're briefing a sharp intern:
- Be specific about the output format
- Define constraints and guardrails
- Include tone or style guidance if it matters
-->

## Example

### Input

<!-- Paste a realistic example input -->

### Output

<!-- Paste the expected output for the input above -->

---

## Source

<!-- If this skill is based on an external source, add attribution here:
Initial raw source: [repo-name](https://github.com/...)
-->
```

## Description Guidance

The `description` field is how Cursor discovers when to use the skill. Write it in third person and include both:

- What the skill does
- When the agent should use it

Example:

```yaml
description: Write a PRD from a problem statement or feature idea. Use when scoping product features, defining success metrics, writing user stories, or creating acceptance criteria.
```

## Catalog Pages

Human-friendly catalog pages live in category folders such as `product-management/` or `productivity/`. If you add an installable skill, add or update both:

- `skills/<skill-name>/SKILL.md`
- `<category>/<skill-name>.md`

External tools and bundles with their own installation flow should be documented as guides, not copied into `skills/` as one-file skills.
