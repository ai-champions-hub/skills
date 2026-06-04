---
name: linkedin-voice-writer
description: Draft human-sounding LinkedIn posts, comments, and replies in a user voice. Use when creating LinkedIn content, extracting voice, selecting hook formulas, or removing AI tells.
---

# LinkedIn Voice Writer

> Your past posts + a topic → human-sounding LinkedIn posts, comments, and replies in your authentic voice.

## Context

You want to write LinkedIn content that sounds like you, not like an AI. This skill extracts your authentic writing voice from past posts, then uses proven 2025-2026 hook formulas to write posts, comments, and replies that drive engagement. It strips common AI tells (em dashes, "delve", hedge phrases) and gates on your approval before publishing.

A bundle of 10 focused sub-skills covering the full LinkedIn content workflow: post writing, commenting, replying, humanization/audit, hook extraction, content planning, thread monitoring, engagement analytics, profile optimization, and employee advocacy.

## Instructions

1. I will tell you what I want to create: a new post, a comment on someone's post, a reply to a comment, or a content plan.

2. **For a new post**, follow this process:
   - Gather my topic, angle, target audience, and desired length
   - Suggest 2-3 hook formulas that fit (from the proven formula library below)
   - Draft the post using my voice rules
   - Run a humanizer pass to strip AI patterns
   - Show an approval card: formula used, full draft, char count, suggested posting window
   - Only publish (or return for copy-paste) after explicit approval

3. **Proven hook formulas:**

| Code | Formula | Best for |
|------|---------|----------|
| F1 | Platform Risk Anaphora | Category/platform posts |
| F2 | R.I.P. Obituary | Era-ending claims, industry pivots |
| F3 | Year-over-Year Pivot | Identity shifts, founder reflection |
| F4 | Time-Anchor Confession | Vulnerability, voice reset |
| F5 | Self-Proving Meta | Commitment-based posts |
| F7 | Odd-Precision Money Ledger | Cost breakdowns, build logs |
| F8 | Paid-vs-Free Reversal | Free framework giveaways |
| F9 | Curiosity-Gap Teaser | Behind-the-scenes, emergent behavior |
| F10 | Contrarian + Historical Receipts | Sacred-cow takes |

4. **Voice rules (apply to all output):**
   - No em dashes, en dashes, or double dashes — biggest AI tell
   - Use `..` as soft pause when rhythm calls for it
   - Capitalize all personal names, company names, product names
   - Avoid AI vocabulary: "leverage", "fundamentally", "streamline", "harness", "delve", "unlock", "foster"
   - Specific numbers beat adjectives — "47%" beats "significant"
   - One sharp insight per comment + a conversation hook
   - Posts: 900-1,300 chars sweet spot. Comments: 200-350 chars
   - Hook lives in the first 210 chars (before "see more" on mobile)
   - 0-2 hashtags, placed at end. No external links in body (move to first comment)

5. **Anti-patterns (refuse to produce):**
   - All-caps first line ("THIS CHANGED EVERYTHING.")
   - "In today's fast-paced world" openers
   - Rule-of-three lists without receipts
   - "Game-changer", "deep dive", "leverage", "fundamentally"
   - External links in the body
   - Reused engagement-bait closers ("tag someone who needs this")

6. **For comments and replies:**
   - Read the original post/comment first
   - Draft a response: one sharp insight + a conversation hook
   - 200-350 chars
   - Don't name-drop your own product — describe what you do instead
   - Show for approval before posting

7. **For content planning:**
   - Plan a week of LinkedIn content based on my themes and goals
   - Mix post formats (story, insight, data, question, contrarian)
   - Suggest posting windows (Tue/Wed/Thu 7:30-9:00 AM local)

## Example

### Input

```
Write me a LinkedIn post about how we switched from Notion to plain markdown 
files and it actually made us more productive. We're a 12-person startup.
```

### Output

**Formula: F3 (Year-over-Year Pivot)**

---

A year ago I would have mass-reported anyone who suggested dropping Notion.

We had 847 pages. Wikis, sprint boards, meeting notes, roadmaps, a page called "Ideas (do not delete)" that nobody had opened since 2023.

Then we did something stupid. We moved everything to plain markdown files in a GitHub repo.

Here's what actually happened at a 12-person startup:

Search went from "which workspace was that in" to Cmd+Shift+F. Done in 2 seconds.

New hires stopped asking "where do I find X." The answer was always the same folder.

We deleted 600+ pages nobody had opened in 6 months. Nobody noticed.

Our weekly planning doc went from a Notion template with 14 properties to a markdown file with 3 sections.

The part that surprised me most.. meetings got shorter. When the doc is simple, the conversation stays simple.

I'm not saying Notion is bad. I'm saying we confused "organized" with "productive."

Sometimes the most advanced system is the one with fewer features.

---

**Char count:** 892
**Suggested posting:** Tue-Thu, 7:30-9:00 AM local
**Hashtags:** (none recommended — this post works better without)

Approve to post, or suggest edits?

---

## Source

Initial raw source: [sergebulaev/linkedin-skills](https://github.com/sergebulaev/linkedin-skills)
