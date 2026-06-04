# Nuwa (女娲)

> Build virtual copies of experts — extract their mental models, decision heuristics, and thinking patterns into reusable AI skills.

## What it does

Nuwa spawns 6 parallel research agents that dig through a person's books, podcasts, interviews, social media, and public record. The output is a ready-to-use "think like X" skill file containing their mental models, decision-making heuristics, expression patterns, and values. This is not role-playing — it extracts actual cognitive architecture from real sources.

The repo ships pre-built skills for Steve Jobs, Elon Musk, Charlie Munger, Andrej Karpathy, Richard Feynman, Naval Ravikant, and 7+ others. You can also distill any person with enough public material.

## Why it matters

Instead of asking the AI to "pretend to be Steve Jobs," Nuwa gives it a researched, structured representation of how that person actually thinks. The skill file captures specific mental models (e.g., Munger's "invert, always invert"), decision heuristics (e.g., Jobs's "say no to 1000 things"), and expression DNA (e.g., sentence patterns, vocabulary choices). The result is dramatically more authentic and useful than generic role-playing.

Use cases: strategic decision-making through the lens of a specific thinker, brainstorming sessions channeling a particular expert's approach, learning frameworks from historical figures.

## How to install

**Note:** This is an external package or integration, not a local one-file skill. Follow the install instructions below rather than copying it into `skills/`.

```bash
npx skills add alchaincyf/nuwa-skill
```

Or clone manually:
```bash
git clone https://github.com/alchaincyf/nuwa-skill.git ~/.claude/skills/nuwa
```

## Key commands / features

**Usage:**
```
Use nuwa to create a thinking skill for [person name]
```

**5-phase pipeline:**

1. **Research** (6 parallel agents) — writings, conversations, expression patterns, external views, key decisions, career timeline
2. **Research review** — checkpoint to verify coverage before synthesis
3. **Framework synthesis** — distill mental models, decision heuristics, expression DNA, values and anti-patterns
4. **Skill construction** — assemble into a structured skill file using the template
5. **Quality validation** — sanity check, edge case testing, voice authenticity check, dual-agent refinement

**Pre-built person skills:**
Steve Jobs, Elon Musk, Charlie Munger, Richard Feynman, Naval Ravikant, Andrej Karpathy, Paul Graham, and others.

**What each skill captures:**
- Mental models with specific examples
- Decision-making heuristics (when/how they decide)
- Expression DNA (sentence structure, vocabulary, rhetorical patterns)
- Values and anti-patterns (what they would never do)
- Key decisions with reasoning chains

---

## Source

Initial raw source: [alchaincyf/nuwa-skill](https://github.com/alchaincyf/nuwa-skill)
