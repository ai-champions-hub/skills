# Superpowers

> A composable skill framework that turns AI agents into structured, methodical collaborators.

## What it does

Superpowers is the top-rated agent skill framework (150k+ GitHub stars) that enforces a disciplined workflow on AI coding agents. Instead of letting the agent charge in and start writing code immediately, Superpowers adds mandatory phases: brainstorm first, plan second, execute third, review last. Each phase is a composable skill that auto-triggers during agent sessions.

The framework works across Claude Code, Cursor, Codex, Gemini CLI, GitHub Copilot CLI, and 50+ other agent runtimes.

## Why it matters

Without Superpowers, AI agents behave like hyperactive juniors — they start coding before understanding the problem, skip edge cases, and produce work that looks impressive but falls apart under scrutiny. Superpowers imposes the same discipline a senior engineer would: understand the problem, explore the design space, write a plan, execute in small verified steps, and review against the original spec before declaring victory.

This is the mandatory first install for any serious AI-assisted workflow.

## How to install

**Cursor:**
```
/add-plugin superpowers
```
Or search for "superpowers" in the Cursor plugin marketplace.

**Claude Code:**
```bash
/plugin install superpowers@claude-plugins-official
```

**Other runtimes** (Codex, Gemini CLI, OpenCode, etc.) — see the repo README for runtime-specific instructions.

## Key commands / features

- `/brainstorm` — the agent asks clarifying questions BEFORE starting, explores 2-3 approaches, produces a design doc, and waits for your approval before writing any code.
- `/write-plan` — breaks a task into bite-sized steps (2-5 min each) with exact file paths and verification steps. Shows you the plan before execution so you can correct course early.
- `/execute-plan` — runs multiple sub-agents in parallel, each with a fresh context window, and verifies the result at the end with a two-stage review.
- **Test-Driven Development** — enforces RED-GREEN-REFACTOR: write tests first, always.
- **Git Worktrees** — creates isolated workspaces on new branches for feature work.
- **Code Review** — reviews completed work against the original plan and spec.
- **Finishing a Branch** — offers merge/PR/keep/discard options when work is done.

## Philosophy

- Test-Driven Development — write tests first, always
- Systematic over ad-hoc — process over guessing
- Complexity reduction — simplicity as the primary goal
- Evidence over claims — verify before declaring success

---

## Source

Initial raw source: [obra/superpowers](https://github.com/obra/superpowers)
