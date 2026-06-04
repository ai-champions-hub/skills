---
name: write-spec-prd
description: Write a PRD from a problem statement or feature idea. Use when scoping product features, defining success metrics, writing user stories, or creating acceptance criteria.
---

# Write Spec / PRD

> Problem statement or feature idea → structured Product Requirements Document.

## Context

You have a vague idea, a user request, or a one-paragraph problem statement and need to turn it into a structured PRD that engineering can build from. This skill walks you through the full process: understand the feature, gather context, pull data from connected tools, generate the document, then review and iterate. Built by Anthropic as part of their official knowledge-work-plugins.

## Instructions

1. I will describe a feature idea, problem statement, or user request in any format.
2. Follow this workflow to produce a PRD:

**Phase 1 — Understand the Feature**
- Clarify the user problem being solved
- Identify who the user is (specific role, not "users")
- Determine the scope: is this a new feature, enhancement, or fix?
- Ask 2-3 targeted questions if the input is ambiguous (do not ask more than 3)

**Phase 2 — Gather Context**
- What exists today? What's the current user journey?
- Are there competitors or prior art?
- What constraints exist (technical, timeline, resource)?

**Phase 3 — Generate the PRD**

Structure the document with these sections:

- **Problem Statement** — what pain exists and for whom (2-3 sentences)
- **Goals** — 3-5 measurable outcomes this feature should achieve
- **Non-Goals** — what this feature explicitly does NOT do (scope control)
- **User Stories** — written using INVEST criteria. Format: "As a [role], I want [capability], so that [outcome]."
- **Requirements** — categorized using MoSCoW: P0 (must have), P1 (should have), P2 (nice to have)
- **Success Metrics** — leading + lagging indicators with specific targets. Example: "Activation rate increases from 34% to 45% within 60 days of launch."
- **Open Questions** — tagged by owner. Format: "[PM] Do we support SSO at launch?"
- **Timeline Considerations** — phases, dependencies, key milestones
- **Acceptance Criteria** — Given/When/Then format or checklist for each P0 requirement

**Phase 4 — Review**
- Check for scope creep (features that don't map back to the problem statement)
- Verify every goal has at least one success metric
- Confirm non-goals are explicit enough to prevent future creep
- Flag any user stories that violate INVEST criteria

3. Output the complete PRD in clean Markdown, ready to paste into Notion, Confluence, or a GitHub issue.

## Example

### Input

```
We need to add team workspaces to our project management tool. Right now 
everyone shares one workspace and it's getting chaotic as we scale past 
50 users. People can't find their projects, permissions are a mess, and 
enterprise customers keep asking for it.
```

### Output

**Problem Statement**
As the user base scales past 50 users, the single shared workspace creates discoverability and permission problems. Users cannot find their projects, access controls are insufficient, and enterprise customers have flagged this as a blocker for procurement.

**Goals**
1. Reduce average time to find a project from 45s to under 10s
2. Enable role-based access control at the workspace level
3. Unblock 3+ enterprise deals currently stalled on multi-tenancy
4. Zero increase in onboarding time for new users

**Non-Goals**
- Cross-workspace project sharing (v2)
- Workspace-level billing or invoicing
- Custom workspace themes or branding

**User Stories**
- As a team lead, I want to create a workspace for my team, so that our projects are isolated from other teams' clutter.
- As an admin, I want to set permissions at the workspace level, so that I don't have to manage access project-by-project.
- As a new user, I want to be auto-assigned to my team's workspace, so that I see relevant projects immediately.

*(continued with Requirements, Success Metrics, Open Questions, Timeline, Acceptance Criteria...)*

---

## Source

Initial raw source: [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (Product Management plugin — `write-spec` skill)
