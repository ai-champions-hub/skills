# Brief from Scratch

> Raw idea → polished one-pager brief ready for review.

## Context

You have a rough idea for a project, feature, or initiative — maybe a few bullet points, a voice memo transcription, or just a paragraph of stream-of-consciousness. You need to turn it into a structured one-pager that you can share with your team or stakeholders to get alignment before starting work.

## Instructions

1. I will describe an idea in whatever format I have (bullets, paragraph, rough notes).
2. Turn it into a one-pager brief with these sections:
   - **Title**: clear, descriptive project name.
   - **Problem**: what pain point or opportunity does this address? (2-3 sentences)
   - **Proposal**: what are we building or doing? (3-5 sentences, concrete enough to evaluate)
   - **Target audience**: who benefits from this?
   - **Success metrics**: how will we know it worked? (2-4 measurable outcomes)
   - **Scope**: what's included and, just as important, what's explicitly out of scope.
   - **Timeline**: rough phases or milestones if I provided any; otherwise write "TBD — to be estimated after alignment."
   - **Open questions**: things that need answers before or during execution.
   - **Ask**: what decision or approval is needed from the reader.
3. Keep the total length under 500 words.
4. Use plain language. No buzzwords. Write for a busy executive who will skim it.
5. If I haven't provided enough detail for a section, write a clear placeholder like "[Need input: estimated timeline]" instead of making something up.

## Example

### Input

```
idea: we should add a slack bot that posts a weekly summary of all the PRs 
merged in our repo. eng team is growing and nobody reads all the PRs anymore. 
managers keep asking "what shipped this week" and we waste time in standups 
going through it. should be pretty simple, just hit the github api.
```

### Output

**Title**: Weekly PR Digest Slack Bot

**Problem**
As the engineering team grows, nobody reads every pull request. Managers repeatedly ask "what shipped this week?" and standups waste time on status recaps that could be automated.

**Proposal**
Build a Slack bot that posts a weekly summary of all merged PRs to a designated channel every Monday morning. The summary will include PR title, author, merge date, and a link. It pulls data from the GitHub API and requires no manual input once configured.

**Target audience**
Engineering managers, product managers, and team leads who need a high-level view of shipping velocity without reading every PR.

**Success metrics**
- 100% of merged PRs appear in the weekly digest (accuracy).
- Reduction in "what shipped?" questions in standups (qualitative, survey after 4 weeks).
- Bot is running autonomously within 2 weeks of starting work.

**Scope**
- **In scope**: GitHub PR data, Slack integration, weekly cadence, one repo.
- **Out of scope**: multi-repo support (v2), PR quality analysis, custom filtering.

**Timeline**
TBD — to be estimated after alignment. Rough guess: 1 week of eng time.

**Open questions**
- Which Slack channel should it post to?
- Do we want to include draft PRs or only merged?
- Should it tag PR authors in the Slack message?

**Ask**
Approve the idea so engineering can estimate and schedule it in the next sprint.
