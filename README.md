# AI Champions — Skill Library

**One file. One skill. Drop it into Cursor, Claude, or ChatGPT and go.**

This repo is the open catalog of reusable AI skills maintained by the [AI Champions](https://ai-champions-platform.vercel.app) community. Each skill is a self-contained `.md` file with instructions that turn a general-purpose AI into a specialist for a specific task.

New skills are added weekly from live sessions and the conference archive.

---

## Quick start

```text
1. Browse the catalog below
2. Open the .md file and copy its contents (or download the raw file)
3. Paste into Cursor rules, Claude project instructions, or a ChatGPT custom GPT
```

**Cursor** — save the `.md` file to your project's `.cursor/rules/` directory or `~/.cursor/rules/` for global access.

**Claude** — paste the contents into Project Knowledge or use it as a system prompt.

**ChatGPT** — paste into Custom Instructions or as the first message in a conversation.

---

## Skill catalog

### Productivity

| Skill | What it does |
|-------|-------------|
| [weekly-metrics-narrator.md](productivity/weekly-metrics-narrator.md) | KPI dashboard → narrated update |
| [meeting-notes-to-memo.md](productivity/meeting-notes-to-memo.md) | Transcript → exec-ready memo |
| [brief-from-scratch.md](productivity/brief-from-scratch.md) | Raw idea → polished one-pager |

### Communication

| Skill | What it does |
|-------|-------------|
| [objection-handler.md](communication/objection-handler.md) | Draft responses to tough objections |

### Engineering

| Skill | What it does |
|-------|-------------|
| [agent-deploy-checklist.md](engineering/agent-deploy-checklist.md) | Ship an agent to prod in 45 min |
| [orchestration-planner.md](engineering/orchestration-planner.md) | Multi-agent task graph from a goal |

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
