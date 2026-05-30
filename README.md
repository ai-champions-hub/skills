<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/banner.svg">
  <img alt="AI Champions — Skill Library" src="assets/banner.svg" width="100%">
</picture>

<br>
<br>

**One file. One skill. Drop it into Cursor, Claude, or ChatGPT and go.**

[![Skills](https://img.shields.io/badge/skills-6-00d26a?style=for-the-badge)](https://github.com/ai-champions-hub/skills)
[![Platform](https://img.shields.io/badge/platform-AI%20Champions-1a1a2e?style=for-the-badge)](https://ai-champions-platform.vercel.app)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-00b4d8?style=for-the-badge)](CONTRIBUTING.md)

</div>

<br>

This repo is the open catalog of reusable AI skills maintained by the [AI Champions](https://ai-champions-platform.vercel.app) community. Each skill is a self-contained `.md` file with instructions that turn a general-purpose AI into a specialist for a specific task.

New skills are added weekly from live sessions and the conference archive.

---

<br>

## ⚡ Quick start

<table>
<tr>
<td width="60" align="center"><h2>1</h2></td>
<td><strong>Browse</strong> the skill catalog below and pick a skill</td>
</tr>
<tr>
<td align="center"><h2>2</h2></td>
<td><strong>Copy</strong> the <code>.md</code> file contents or download the raw file</td>
</tr>
<tr>
<td align="center"><h2>3</h2></td>
<td><strong>Load</strong> it into your AI tool of choice</td>
</tr>
</table>

<br>

<details>
<summary><strong>📋 Setup instructions per tool</strong></summary>
<br>

| Tool | How to load a skill |
|------|-------------------|
| **Cursor** | Save the `.md` file to `.cursor/rules/` in your project (or `~/.cursor/rules/` for global access) |
| **Claude** | Paste into Project Knowledge or use as a system prompt |
| **ChatGPT** | Paste into Custom Instructions or send as the first message |

</details>

<br>

---

<br>

## 📚 Skill catalog

### 🟢 Productivity

<table>
<tr>
<td width="400">

**[weekly-metrics-narrator.md](productivity/weekly-metrics-narrator.md)**
<br>
<sub>KPI dashboard → narrated update</sub>

</td>
<td width="400">

**[meeting-notes-to-memo.md](productivity/meeting-notes-to-memo.md)**
<br>
<sub>Transcript → exec-ready memo</sub>

</td>
</tr>
<tr>
<td>

**[brief-from-scratch.md](productivity/brief-from-scratch.md)**
<br>
<sub>Raw idea → polished one-pager</sub>

</td>
<td>
<sub><em>More coming soon</em></sub>
</td>
</tr>
</table>

### 🔵 Communication

<table>
<tr>
<td width="400">

**[objection-handler.md](communication/objection-handler.md)**
<br>
<sub>Draft responses to tough objections</sub>

</td>
<td width="400">
<sub><em>More coming soon</em></sub>
</td>
</tr>
</table>

### ⚙️ Engineering

<table>
<tr>
<td width="400">

**[agent-deploy-checklist.md](engineering/agent-deploy-checklist.md)**
<br>
<sub>Ship an agent to prod in 45 min</sub>

</td>
<td width="400">

**[orchestration-planner.md](engineering/orchestration-planner.md)**
<br>
<sub>Multi-agent task graph from a goal</sub>

</td>
</tr>
</table>

### 📣 Marketing

<table>
<tr>
<td width="400">
<sub><em>Coming soon — contribute the first one!</em></sub>
</td>
<td width="400">
</td>
</tr>
</table>

<br>

---

<br>

## 🧩 Skill format

Every skill follows a consistent structure — see [`SKILL_TEMPLATE.md`](SKILL_TEMPLATE.md):

```
# Skill name
> One-line description of what it does

## Context         ← when and why you'd use this
## Instructions    ← step-by-step for the AI
## Example         ← concrete input → output
```

<br>

---

<br>

## 🤝 Contributing

We welcome new skills from the community — see the full guide in [`CONTRIBUTING.md`](CONTRIBUTING.md).

**TL;DR:**

> **Fork** → copy `SKILL_TEMPLATE.md` into the right folder → rename to `kebab-case.md` → fill it in → **open a PR**

<br>

---

<br>

<div align="center">

**[AI Champions Platform](https://ai-champions-platform.vercel.app)** · **[Skill Library](https://github.com/ai-champions-hub/skills)** · **[Organization](https://github.com/ai-champions-hub)**

<br>

<sub>Built by the <a href="https://github.com/ai-champions-hub">AI Champions</a> community</sub>

</div>
