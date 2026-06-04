# Get Shit Done (GSD)

> A meta-prompting system that splits projects into plan/execute/review phases with fresh context windows.

## What it does

GSD solves "context rot" — the quality degradation that happens as an AI agent fills its context window. After a couple of hours, an agent may start forgetting what it was doing and ship garbage at the end.

GSD fixes this by splitting a project into three isolated phases — **plan**, **execute**, **review**. Each phase starts with a clean 200k-token context and passes state to the next one through structured files on disk (`PROJECT.md`, `REQUIREMENTS.md`, `ROADMAP.md`, `STATE.md`, `CONTEXT.md`). Heavy work happens in fresh subagent contexts while the main window stays at 30-40% utilization.

Works with Claude Code, Cursor, Codex, Gemini CLI, OpenCode, Windsurf, and more.

## Why it matters

Long-running AI sessions degrade predictably. The more context an agent accumulates, the more it hallucinates, forgets instructions, and produces inconsistent output. GSD is an architectural fix: instead of hoping the agent holds it together, you give each phase a clean workspace and a clear handoff contract. The result is consistent quality even on multi-hour projects.

## How to install

**Note:** This is an external package or integration, not a local one-file skill. Follow the install instructions below rather than copying it into `skills/`.

```bash
npx @opengsd/get-shit-done-redux@latest
```

Works on Mac, Windows, Linux. The installer prompts for your runtime and offers global or local install.

**Profiles:**
- `--profile=core` — 6 core-loop skills only
- `--profile=standard` — core + phase management
- (default) — full install with all features

## Key commands / features

| Command | What it does |
|---------|-------------|
| `/gsd-new-project` | Interactive questions → research → requirements → roadmap |
| `/gsd-discuss-phase [N]` | Capture implementation decisions before planning |
| `/gsd-plan-phase [N]` | Research + plan + verify loop |
| `/gsd-execute-phase` | Execute plans in parallel waves with fresh subagent contexts |
| `/gsd-verify-work [N]` | Manual acceptance testing + diagnose-fix plans |
| `/gsd-ship [N]` | Create PR from verified phase work |
| `/gsd-progress --next` | Show current progress and suggest next action |

## Configuration

Settings live in `.planning/config.json`:
- `mode`: `interactive` (default) or `yolo` (auto-approve everything)
- Model profiles: `quality` / `balanced` / `budget`
- Research, plan-check, and verifier agent toggles
- Parallelization settings for subagents

---

## Source

Initial raw source: [open-gsd/get-shit-done-redux](https://github.com/open-gsd/get-shit-done-redux) (successor to [gsd-build/get-shit-done](https://github.com/gsd-build/get-shit-done))
