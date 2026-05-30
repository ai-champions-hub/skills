# Contributing a skill

Thanks for contributing to the AI Champions Skill Library! Every skill you add helps the whole community work smarter.

## Before you start

- Check the [catalog](README.md#skills) to make sure a similar skill doesn't already exist.
- One `.md` file = one skill. Keep it focused on a single task.

## Step by step

1. **Fork** this repository.
2. **Copy** `SKILL_TEMPLATE.md` into the category folder that fits best:
   - `foundations/` — core frameworks and plugins (install-once tools, not prompts)
   - `product-management/` — PRDs, OKRs, roadmaps, discovery, prioritization
   - `marketing/` — campaigns, copy, SEO, analytics, personal brand
   - `productivity/` — meetings, memos, updates, planning, note-taking
   - `presentations/` — slide decks, visual storytelling, pitch materials
   - `leadership/` — strategy, decisions, coaching, hiring, team management
   - `design/` — UI/UX review, design systems, Figma workflows
   - Not sure? Pick the closest one — we can always move it in review.
3. **Rename** the file using `kebab-case.md` (e.g., `weekly-report-writer.md`).
4. **Fill in** every section of the template. Delete the placeholder comments.
5. **Add a Source section** at the bottom if the skill is based on an external source:
   ```markdown
   ---

   ## Source

   Initial raw source: [repo-name](https://github.com/...)
   ```
6. **Test** the skill in at least one tool (Cursor, Claude, or ChatGPT) before submitting.
7. **Open a Pull Request** with:
   - A short title: `Add skill: your-skill-name`
   - A one-line description of what the skill does

## File naming

- Use lowercase `kebab-case`: `meeting-notes-to-memo.md`
- Keep it short but descriptive
- No spaces, no underscores

## Quality checklist

Before submitting, make sure your skill:

- [ ] Has a clear one-line description (input → output format)
- [ ] Includes step-by-step instructions for the AI
- [ ] Has at least one concrete example (input → output)
- [ ] Works when pasted directly into Cursor, Claude, or ChatGPT
- [ ] Doesn't duplicate an existing skill
- [ ] Includes a Source section if based on external work

## Review process

A maintainer will review your PR, usually within a few days. We may suggest edits to improve clarity or consistency. Once approved, your skill goes live in the catalog.

---

Questions? Reach out in the Champions community or open an issue.
