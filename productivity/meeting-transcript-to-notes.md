# Meeting Transcript to Notes

> Raw meeting transcript → structured notes with decisions, action items, and summary.

## Context

After a meeting you have a raw transcript (from Granola, Otter, Fireflies, or manual notes) and need a clean, structured memo. Anyone who missed the meeting should be able to read it in 2 minutes and know exactly what was decided, who owns what, and what's still unresolved. The output drops straight into Obsidian, Notion, or any Markdown system.

## Instructions

1. I will paste a meeting transcript or rough notes.

2. **Extract action items** — review the entire transcript for:
   - Explicit commitments: "I'll do X", "Alex will review Y"
   - Assigned tasks: "Nathan and Damian should schedule..."
   - Follow-up items: "We need to...", "Let's make sure to..."
   - Decisions requiring action: "We should deploy X before Y"

   Format as a bulleted list. Use **bold** for person names. Include context for what needs to be done and why. Order by priority when evident.

3. **Write a summary** that captures:
   - Main topics discussed
   - Key decisions made (with who made or approved each one)
   - Technical approach or architecture agreed upon (if applicable)
   - Timeline and next steps
   - Important context or constraints

   Keep it factual and outcome-focused. Use subsections for major topics. Include enough detail that someone not in the meeting can understand what happened.

4. **Add frontmatter** (YAML):
   ```yaml
   title: Meeting Title
   date: YYYY-MM-DD
   type: meeting
   attendees: [Person 1, Person 2, ...]
   tags: [meeting, relevant-tags]
   status: complete
   key_topics:
     - Topic 1
     - Topic 2
   action_items:
     - "Action item 1"
     - "Action item 2"
   decisions:
     - Decision 1
     - Decision 2
   ```

5. **Assemble the final note** in this order:
   1. YAML frontmatter
   2. Links section (if any Notion/Linear/GitHub links were mentioned)
   3. `# Action Items` section
   4. `# Summary` section
   5. `# Transcript` section (original transcript preserved for reference)

6. If something is ambiguous in the notes, flag it with `[unclear from transcript]` rather than guessing.
7. Format so it can be pasted directly into Obsidian, Notion, Slack, or email.

## Example

### Input

```
standup 5/28, me, sarah, james
talked about the launch timeline - sarah says eng can ship by june 10 but 
wants 3 extra days for load testing. james pushed back, said marketing already 
announced june 10. we agreed to keep june 10 as external date but do a soft 
launch june 7 for internal users. james will update the landing page copy by 
friday. sarah needs to loop in devops for the load test environment. i'll 
draft the internal comms. also someone needs to figure out the pricing page 
- nobody owned it yet.
```

### Output

```yaml
---
title: Launch Timeline Standup
date: 2025-05-28
type: meeting
attendees: [Author, Sarah, James]
tags: [meeting, launch, timeline]
status: complete
key_topics:
  - Launch timeline and phasing
  - Load testing environment
  - Pricing page ownership
action_items:
  - "James: Update landing page copy by Friday"
  - "Sarah: Loop in DevOps for load test environment"
  - "Author: Draft internal launch comms"
  - "TBD: Pricing page ownership unassigned"
decisions:
  - "Keep June 10 as external launch date"
  - "Add soft launch June 7 for internal users"
---
```

# Action Items

- **James**: Update landing page copy by Friday May 30
- **Sarah** (+ DevOps): Set up load test environment (due TBD)
- **Author**: Draft internal launch comms (due TBD)
- **Unassigned**: Pricing page — raised but no owner assigned

# Summary

The team aligned on a two-phase launch: internal soft launch on June 7, public launch on June 10. Load testing will happen in between.

**Key decisions:**
1. Keep June 10 as the external launch date (James — marketing already announced).
2. Add a soft launch on June 7 for internal users to de-risk (proposed by Sarah, agreed by all).

**Open:** Pricing page ownership is unresolved. Raised but not assigned.

# Transcript

*(original transcript preserved here)*

---

## Source

Initial raw source: [dgalarza/claude-code-workflows](https://github.com/dgalarza/claude-code-workflows) (meeting-transcript plugin)
