# Installing AI Champions Skills

This repository has two surfaces:

- `skills/` contains installable Cursor skill packages. Each package has a `SKILL.md` file with YAML frontmatter (`name` and `description`).
- Category folders such as `product-management/`, `marketing/`, and `productivity/` are human-friendly catalog pages.
- `foundations/` contains install guides for external frameworks and integrations. These are not local one-file skills.

## Install One Skill With Cursor Agent

Open Cursor in your project and paste one of these prompts:

```text
Install the `write-spec-prd` skill from https://github.com/ai-champions-hub/skills/tree/main/skills/write-spec-prd into this project.
```

```text
Install the `linkedin-voice-writer` skill from https://github.com/ai-champions-hub/skills/tree/main/skills/linkedin-voice-writer into this project.
```

Cursor should create:

```text
.cursor/skills/<skill-name>/SKILL.md
```

and copy the package content from this repo.

## Install One Skill Manually

1. Pick a skill from the `skills/` directory.
2. Create this folder in your project:

```text
.cursor/skills/<skill-name>/
```

3. Copy the raw contents of `skills/<skill-name>/SKILL.md` into:

```text
.cursor/skills/<skill-name>/SKILL.md
```

4. Restart Cursor or start a new agent session so the skill can be discovered.

## Install Available Skills

| Skill | Package URL |
|-------|-------------|
| Write Spec / PRD | https://github.com/ai-champions-hub/skills/tree/main/skills/write-spec-prd |
| PRD Critique | https://github.com/ai-champions-hub/skills/tree/main/skills/prd-critique |
| OKR Coach | https://github.com/ai-champions-hub/skills/tree/main/skills/okr-coach |
| LinkedIn Voice Writer | https://github.com/ai-champions-hub/skills/tree/main/skills/linkedin-voice-writer |
| Stakeholder Update | https://github.com/ai-champions-hub/skills/tree/main/skills/stakeholder-update |
| Meeting Transcript to Notes | https://github.com/ai-champions-hub/skills/tree/main/skills/meeting-transcript-to-notes |
| Pyramid Principle Memo | https://github.com/ai-champions-hub/skills/tree/main/skills/pyramid-principle-memo |
| Frontend Slides | https://github.com/ai-champions-hub/skills/tree/main/skills/frontend-slides |
| Decision Stress-Test | https://github.com/ai-champions-hub/skills/tree/main/skills/decision-stress-test |
| Interview Coach | https://github.com/ai-champions-hub/skills/tree/main/skills/interview-coach |
| Figma Review | https://github.com/ai-champions-hub/skills/tree/main/skills/figma-review |

## External Tools and Bundles

Some catalog entries are better installed from their original projects because they include multiple skills, scripts, MCP setup, or runtime-specific plugin behavior:

| Tool | Install guide |
|------|---------------|
| Superpowers | `foundations/superpowers.md` |
| Get Shit Done | `foundations/get-shit-done.md` |
| Composio | `foundations/composio.md` |
| Deep Research | `foundations/deep-research.md` |
| Nuwa | `foundations/nuwa.md` |
| Marketing Skills Bundle | `marketing/marketing-skills-bundle.md` |

Do not copy these into `.cursor/skills/` unless you intentionally want a local note, not the full external package.
