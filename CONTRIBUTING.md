# Contributing a Skill

Thanks for contributing to the AI Champions Skill Library. Every useful skill makes the community's AI workflows easier to reuse.

## Before You Start

- Check the [catalog](README.md#installable-skills) to make sure a similar skill does not already exist.
- Decide whether you're adding an installable one-file skill or an external tool guide.

## Repository Model

This repo has two surfaces:

- **Installable skills:** `skills/<skill-name>/SKILL.md`
- **Catalog pages:** category folders such as `product-management/`, `marketing/`, `productivity/`, `leadership/`, and `design/`

If your contribution is a true one-file skill, add both surfaces. If it is a full external package, MCP integration, plugin, or bundle with its own installer, add it as a catalog guide instead.

## Add an Installable Skill

1. Fork this repository.
2. Create a package directory:

```text
skills/<skill-name>/SKILL.md
```

3. Start `SKILL.md` with YAML frontmatter:

```markdown
---
name: skill-name
description: Specific third-person description. Include what it does and when to use it.
---
```

4. Fill in the body using [SKILL_TEMPLATE.md](SKILL_TEMPLATE.md).
5. Add a matching catalog page in the closest category folder:
   - `product-management/` — PRDs, OKRs, roadmaps, discovery, prioritization
   - `marketing/` — campaigns, copy, SEO, analytics, personal brand
   - `productivity/` — meetings, memos, updates, planning, note-taking
   - `presentations/` — slide decks, visual storytelling, pitch materials
   - `leadership/` — strategy, decisions, coaching, hiring, team management
   - `design/` — UI/UX review, design systems, Figma workflows
6. Add an `Install` section to the catalog page that points to the package.
7. Add source attribution at the bottom if based on external work:

```markdown
---

## Source

Initial raw source: [repo-name](https://github.com/...)
```

## Add an External Tool or Bundle

Use a catalog guide instead of `skills/` when the source is:

- A plugin with its own installation command
- A multi-skill bundle
- An MCP integration
- A repository that depends on scripts, subdirectories, or runtime-specific setup

For these, include:

- What it does
- Why it matters
- How to install
- Key commands or features
- Source link

## File Naming

- Use lowercase `kebab-case`: `meeting-transcript-to-notes`
- Directory name and frontmatter `name` must match
- No spaces or underscores

## Quality Checklist

Before submitting, make sure your contribution:

- [ ] Uses `skills/<skill-name>/SKILL.md` for installable skills
- [ ] Has YAML frontmatter with `name` and `description`
- [ ] Uses a specific description with trigger scenarios
- [ ] Includes step-by-step instructions for the AI
- [ ] Has at least one concrete example (input → output)
- [ ] Includes a Source section if based on external work
- [ ] Has a matching catalog page with install instructions
- [ ] Does not present external packages as local one-file skills

## Review Process

A maintainer will review your PR, usually within a few days. We may suggest edits to improve clarity, installability, or consistency. Once approved, your skill goes live in the catalog.

---

Questions? Reach out in the Champions community or open an issue.
