---
name: stakeholder-update
description: Generate stakeholder-ready status updates from working notes. Use when writing weekly updates, monthly updates, launch announcements, or risk escalations for executives or cross-functional teams.
---

# Stakeholder Update

> Working notes + context → polished stakeholder-ready status update.

## Context

You need to produce a stakeholder update — weekly, monthly, launch announcement, or ad-hoc risk escalation. You have raw project notes, and you need a clean, audience-appropriate update: progress, blockers, asks, next steps. Built by Anthropic as part of their official knowledge-work-plugins. Supports multiple audience types (executive, engineering, cross-functional, customer) and multiple update cadences.

## Instructions

1. I will provide my raw notes, project context, or data. I may also specify the audience and update type.

2. **Determine the update type:**
   - Weekly status — regular cadence, focus on progress and blockers
   - Monthly status — broader view, trends and trajectory
   - Launch announcement — milestone reached, what it means, what's next
   - Ad-hoc / risk escalation — something needs attention now

3. **Determine the audience** (ask if not specified):
   - **Executive** — high-level, outcome-focused, 2-min read. Lead with status (green/yellow/red), then headline, then details only if needed.
   - **Engineering** — technical detail, blockers, dependencies, architecture decisions.
   - **Cross-functional** — balanced, plain language, emphasis on what each team needs to know or do.
   - **Customer / external** — positive framing, feature-focused, no internal jargon.
   - **Board** — strategic framing, metrics, market context, asks.

4. **Structure the update:**

**For executive/cross-functional updates:**
- **Status**: G/Y/R with one-sentence justification
- **Headline**: the single most important thing (1 sentence)
- **Progress this period**: 3-5 bullet points, each with a concrete outcome (not activity)
- **Blockers / risks**: each with owner, impact, and mitigation plan. Use ROAM framework (Resolved / Owned / Accepted / Mitigated)
- **Asks**: what you need from the reader (decisions, resources, escalation)
- **Next period**: 3-5 planned outcomes (not tasks)

**For engineering updates:**
- **Shipped**: PRs merged, features deployed, technical debt addressed
- **In progress**: current sprint items with completion estimates
- **Blocked**: technical blockers with proposed solutions
- **Architecture decisions**: any ADRs (Architecture Decision Records) made this period
- **Tech debt / risk**: items accumulating that need attention

5. **Status color guidelines:**
   - **Green**: on track, no material risks
   - **Yellow**: at risk — timeline, scope, or quality concern that has a mitigation plan
   - **Red**: off track — needs executive attention or scope/timeline change

6. Keep the total update under 400 words for executive, under 600 for cross-functional, no limit for engineering.
7. Write in plain language. No buzzwords. Every bullet should pass the "so what?" test.
8. If I haven't provided enough detail for a section, write "[Need input: ...]" rather than making something up.

## Example

### Input

```
Notes from this week:
- shipped the new onboarding flow finally, took 3 extra days
- activation rate already up from 23% to 29% in first 3 days
- backend migration to new DB is 60% done, on track for next friday
- design team is blocked on the dashboard redesign because we haven't 
  finalized the metrics list
- need VP approval on the pricing change before we can update the billing page
- hired a new senior eng, starts monday
```

### Output

**Weekly Status — Product Team — Week of [date]**

**Status: YELLOW** — Onboarding shipped (late but strong early results). Dashboard redesign blocked pending metrics decision.

**Headline:** New onboarding flow launched — activation rate jumped from 23% to 29% in the first 3 days.

**Progress**
- Onboarding v2 shipped (3 days late). Early signal: activation rate up 6pp (23% → 29%). Monitoring for full-week trend.
- Backend DB migration 60% complete, on track for next Friday.
- New senior engineer hired, starts Monday.

**Blockers**
- Dashboard redesign blocked — metrics list not finalized. **Owner: PM.** **Impact:** design timeline slips 1 week per week of delay. **Status: Owned** — scheduling metrics alignment meeting for Tuesday.
- Pricing page update blocked on VP approval for pricing change. **Owner: VP Product.** **Status: Owned** — decision needed by Thursday to stay on sprint timeline.

**Asks**
1. VP: approve pricing change by Thursday (doc linked in Slack)
2. PM team: finalize dashboard metrics list by Tuesday EOD

**Next week**
- Complete DB migration and begin performance testing
- Unblock dashboard redesign
- Onboard new senior eng (buddy: Sarah)
- Week 1 onboarding metrics readout (full 7-day cohort)

---

## Source

Initial raw source: [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (Product Management plugin — `stakeholder-update` skill)
