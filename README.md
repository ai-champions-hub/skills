# AI Champions — Skill Library

<p align="center">
  <img src="assets/banner.svg" alt="AI Champions Skill Library" width="100%">
</p>

**One file. One skill. Drop it into Cursor, Claude, or ChatGPT and go.**

This repo is the open catalog of curated AI skills maintained by the [AI Champions](https://ai-champions-platform.vercel.app) community. Each skill is a self-contained `.md` file with instructions that turn a general-purpose AI into a specialist for a specific task.

---

## Quick start

1. Browse the catalog below
2. Open the `.md` file and copy its contents (or download the raw file)
3. Paste into Cursor rules, Claude project instructions, or a ChatGPT custom GPT

**Cursor** — save the `.md` file to your project's `.cursor/rules/` directory or `~/.cursor/rules/` for global access.

**Claude** — paste the contents into Project Knowledge or use it as a system prompt.

**ChatGPT** — paste into Custom Instructions or as the first message in a conversation.

---

## Foundations

Core frameworks and plugins that you install once. These underpin everything else — they change how the AI agent works, not just what it knows.

| Tool | What it does |
|------|-------------|
| [superpowers.md](foundations/superpowers.md) | Composable skill framework — enforces brainstorm → plan → execute → review |
| [get-shit-done.md](foundations/get-shit-done.md) | Splits projects into plan/execute/review phases with fresh context windows |
| [composio.md](foundations/composio.md) | MCP integration for 500+ external services (Gmail, Slack, Notion, etc.) |
| [deep-research.md](foundations/deep-research.md) | 8-phase research pipeline with source credibility scoring |
| [nuwa.md](foundations/nuwa.md) | Build virtual copies of experts — extract mental models into reusable skills |

## Skills

### Product Management

| Skill | What it does |
|-------|-------------|
| [write-spec-prd.md](product-management/write-spec-prd.md) | Problem statement → full PRD with goals, user stories, and acceptance criteria |
| [prd-critique.md](product-management/prd-critique.md) | Existing PRD → structured feedback with rubric scores and specific fixes |
| [okr-coach.md](product-management/okr-coach.md) | Draft or existing OKRs → critique, refinement, and lifecycle management |

### Marketing

| Skill | What it does |
|-------|-------------|
| [marketing-skills-bundle.md](marketing/marketing-skills-bundle.md) | 42-skill marketing toolkit: CRO, copywriting, SEO, ads, email, retention |
| [linkedin-voice-writer.md](marketing/linkedin-voice-writer.md) | Your voice + a topic → human-sounding LinkedIn posts using proven hook formulas |

### Productivity

| Skill | What it does |
|-------|-------------|
| [stakeholder-update.md](productivity/stakeholder-update.md) | Working notes → polished stakeholder-ready status update |
| [meeting-transcript-to-notes.md](productivity/meeting-transcript-to-notes.md) | Raw transcript → structured notes with decisions, action items, and summary |
| [pyramid-principle-memo.md](productivity/pyramid-principle-memo.md) | Topic + arguments → strategic memo using Barbara Minto's Pyramid Principle |

### Presentations

| Skill | What it does |
|-------|-------------|
| [frontend-slides.md](presentations/frontend-slides.md) | Topic or content → beautiful slide deck as a single HTML file |

### Leadership

| Skill | What it does |
|-------|-------------|
| [decision-stress-test.md](leadership/decision-stress-test.md) | Decision or idea → rigorous challenge against cognitive biases |
| [interview-coach.md](leadership/interview-coach.md) | Interview prep, transcript analysis, and practice drills with STAR/CAR scoring |

### Design

| Skill | What it does |
|-------|-------------|
| [figma-review.md](design/figma-review.md) | Figma file → structured design review with comments posted directly into Figma |

---

## Extended resources

Looking for more skills beyond this catalog? See **[RESOURCES.md](RESOURCES.md)** — a curated list of 30+ external repositories and aggregators organized by domain (PM, marketing, knowledge work, sales, finance, and more).

---

## Skill format

Every skill follows a consistent structure (see [SKILL_TEMPLATE.md](SKILL_TEMPLATE.md)):

```
# Skill name
> One-line description of what it does

## Context
When and why you'd use this skill.

## Instructions
Step-by-step instructions for the AI.

## Example
A concrete input/output example.

## Source
Link to the original source.
```

---

## Contributing

We welcome new skills from the community. See [CONTRIBUTING.md](CONTRIBUTING.md) for the full guide.

**TL;DR:**

1. Fork this repo
2. Copy `SKILL_TEMPLATE.md` into the right category folder
3. Rename it using `kebab-case.md`
4. Fill in the template
5. Open a PR

---

## Links

- [AI Champions Platform](https://ai-champions-platform.vercel.app) — sprint recordings, live sessions, community
- [Skill Library on the web](https://ai-champions-platform.vercel.app/skills) — visual catalog with one-click copy

---

*Built by the [AI Champions](https://github.com/ai-champions-hub) community.*
