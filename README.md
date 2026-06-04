# AI Champions — Skill Library

<p align="center">
  <img src="assets/banner.svg" alt="AI Champions Skill Library" width="100%">
</p>

**Curated AI skills you can browse, install, and use in Cursor.**

This repo has two surfaces:

- **Browse:** category pages explain what each skill does, when to use it, examples, and sources.
- **Install:** `skills/<skill-name>/SKILL.md` packages are Cursor-compatible skills with `name` and `description` frontmatter.

Foundations such as Superpowers, GSD, Composio, Deep Research, Nuwa, and the Marketing Skills Bundle are external packages or integrations. They stay as install guides, not local one-file skills.

---

## Quick Start

### Install with Cursor

Open Cursor in your project and ask:

```text
Install the `write-spec-prd` skill from https://github.com/ai-champions-hub/skills/tree/main/skills/write-spec-prd into this project.
```

Cursor should create:

```text
.cursor/skills/write-spec-prd/SKILL.md
```

See [INSTALL.md](INSTALL.md) for all install prompts and manual instructions.

### Browse the Catalog

Use the tables below if you want to understand what a skill does before installing it.

---

## Foundations

Core frameworks and integrations that you install from their original projects.

| Tool | What it does | Guide |
|------|-------------|-------|
| Superpowers | Composable skill framework — enforces brainstorm → plan → execute → review | [guide](foundations/superpowers.md) |
| Get Shit Done | Splits projects into plan/execute/review phases with fresh context windows | [guide](foundations/get-shit-done.md) |
| Composio | MCP integration for 500+ external services (Gmail, Slack, Notion, etc.) | [guide](foundations/composio.md) |
| Deep Research | 8-phase research pipeline with source credibility scoring | [guide](foundations/deep-research.md) |
| Nuwa | Build virtual copies of experts — extract mental models into reusable skills | [guide](foundations/nuwa.md) |

## Installable Skills

### Product Management

| Skill | What it does | Browse | Installable package |
|-------|-------------|--------|---------------------|
| Write Spec / PRD | Problem statement → full PRD with goals, user stories, and acceptance criteria | [catalog](product-management/write-spec-prd.md) | [SKILL.md](skills/write-spec-prd/SKILL.md) |
| PRD Critique | Existing PRD → structured feedback with rubric scores and specific fixes | [catalog](product-management/prd-critique.md) | [SKILL.md](skills/prd-critique/SKILL.md) |
| OKR Coach | Draft or existing OKRs → critique, refinement, and lifecycle management | [catalog](product-management/okr-coach.md) | [SKILL.md](skills/okr-coach/SKILL.md) |

### Marketing

| Skill | What it does | Browse | Installable package |
|-------|-------------|--------|---------------------|
| LinkedIn Voice Writer | Your voice + a topic → human-sounding LinkedIn posts using proven hook formulas | [catalog](marketing/linkedin-voice-writer.md) | [SKILL.md](skills/linkedin-voice-writer/SKILL.md) |

### Productivity

| Skill | What it does | Browse | Installable package |
|-------|-------------|--------|---------------------|
| Stakeholder Update | Working notes → polished stakeholder-ready status update | [catalog](productivity/stakeholder-update.md) | [SKILL.md](skills/stakeholder-update/SKILL.md) |
| Meeting Transcript to Notes | Raw transcript → structured notes with decisions, action items, and summary | [catalog](productivity/meeting-transcript-to-notes.md) | [SKILL.md](skills/meeting-transcript-to-notes/SKILL.md) |
| Pyramid Principle Memo | Topic + arguments → strategic memo using Barbara Minto's Pyramid Principle | [catalog](productivity/pyramid-principle-memo.md) | [SKILL.md](skills/pyramid-principle-memo/SKILL.md) |

### Presentations

| Skill | What it does | Browse | Installable package |
|-------|-------------|--------|---------------------|
| Frontend Slides | Topic or content → beautiful slide deck as a single HTML file | [catalog](presentations/frontend-slides.md) | [SKILL.md](skills/frontend-slides/SKILL.md) |

### Leadership

| Skill | What it does | Browse | Installable package |
|-------|-------------|--------|---------------------|
| Decision Stress-Test | Decision or idea → rigorous challenge against cognitive biases | [catalog](leadership/decision-stress-test.md) | [SKILL.md](skills/decision-stress-test/SKILL.md) |
| Interview Coach | Interview prep, transcript analysis, and practice drills with STAR/CAR scoring | [catalog](leadership/interview-coach.md) | [SKILL.md](skills/interview-coach/SKILL.md) |

### Design

| Skill | What it does | Browse | Installable package |
|-------|-------------|--------|---------------------|
| Figma Review | Figma file → structured design review with comments posted directly into Figma | [catalog](design/figma-review.md) | [SKILL.md](skills/figma-review/SKILL.md) |

## External Bundles

| Bundle | What it does | Guide |
|--------|-------------|-------|
| Marketing Skills Bundle | 42-skill marketing toolkit: CRO, copywriting, SEO, ads, email, retention | [guide](marketing/marketing-skills-bundle.md) |

---

## Extended Resources

Looking for more skills beyond this catalog? See [RESOURCES.md](RESOURCES.md) — a curated list of 30+ external repositories and aggregators organized by domain.

---

## Skill Format

Installable skills live at `skills/<skill-name>/SKILL.md` and start with YAML frontmatter:

```markdown
---
name: write-spec-prd
description: Write a PRD from a problem statement or feature idea. Use when scoping product features, defining success metrics, writing user stories, or creating acceptance criteria.
---
```

See [SKILL_TEMPLATE.md](SKILL_TEMPLATE.md) for the full template.

---

## Contributing

We welcome new skills from the community. See [CONTRIBUTING.md](CONTRIBUTING.md) for the full guide.

---

## Links

- [AI Champions Platform](https://ai-champions-platform.vercel.app) — sprint recordings, live sessions, community
- [Skill Library on the web](https://ai-champions-platform.vercel.app/skills) — visual catalog with one-click copy

---

*Built by the [AI Champions](https://github.com/ai-champions-hub) community.*
