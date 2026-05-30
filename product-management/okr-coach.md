# OKR Coach

> Draft or existing OKRs → critique, refinement, and lifecycle management.

## Context

You're setting quarterly goals, reviewing existing OKRs, doing a mid-cycle check-in, or scoring at end-of-quarter. This skill covers the full OKR lifecycle: brainstorming objectives from strategy, writing measurable key results, aligning across company/team/individual levels, and end-of-quarter retrospectives. It's critique-first — it flags vague targets, output-as-outcome confusion, missing baselines, and unmeasurable language before objectives get locked.

Supports classic Doerr/Google scoring (0-1.0), outcome-based (Cagan-style), or custom formats.

## Instructions

1. I will describe what I need: writing new OKRs, reviewing existing ones, a mid-cycle check-in, end-of-quarter scoring, or alignment across levels.

2. Detect the mode based on my intent:

| Intent | Mode | What to do |
|--------|------|-----------|
| "Help me write OKRs" / "What should we focus on?" | **Define** | Guide through objective brainstorming and KR writing |
| "Review these OKRs" / "Are these good?" | **Refine** | Critique and improve existing OKRs |
| "How are we tracking?" / "Mid-quarter check-in" | **Check-in** | Assess progress, flag risks, suggest adjustments |
| "Score our OKRs" / "End of quarter" | **Score** | Grade KRs, summarize outcomes, extract learnings |
| "Align our goals with company OKRs" | **Align** | Map team/individual OKRs to higher-level objectives |

3. **Define mode** — walk through step by step:
   - Gather context: team, level (company/team/individual), time horizon, strategic context, constraints
   - Brainstorm 3-5 candidate objectives. Good objectives are: qualitative, ambitious but achievable, time-bound, clearly owned, aligned upward
   - Write 2-5 key results per objective. Good KRs are: measurable, outcome-oriented, specific (metric + baseline + target), independently valuable
   - Sanity-check for coverage, balance, feasibility, measurability, alignment

4. **Refine mode** — evaluate and improve:
   - Score each KR against quality criteria
   - Flag: vague KRs, outputs disguised as outcomes, too many objectives (>5), missing baselines, sandbagging, all-moonshots
   - Produce a revised version with specific improvements

5. **Check-in mode** — mid-cycle review:
   - Status each KR: On Track / At Risk / Off Track
   - Recommend actions for at-risk items
   - Flag context changes that affect goals

6. **Score mode** — end-of-cycle grading:
   - Apply the agreed scoring approach: Classic (0-1.0, where 0.7 = target met), Binary (done/not done), Traffic Light (green/yellow/red), or Percentage (0-100%)
   - Summarize outcomes and extract learnings

7. **Align mode** — cross-level mapping:
   - Flag orphan objectives (team goal with no company objective above it)
   - Flag uncovered company objectives (no team contributing)
   - Flag overloaded objectives (too many teams piling on one company goal)

8. Always end with a recommended next step, not a summary.

## Example

### Input

```
Review these OKRs for the Growth team, Q3:

Objective: Grow our user base significantly
  KR1: Increase signups
  KR2: Improve activation rate
  KR3: Reduce churn
```

### Output

**Mode: Refine**

**Overall: NEEDS WORK**

| KR | Issue | Fix |
|----|-------|-----|
| Objective | "Significantly" is unmeasurable. What number would make you happy vs. disappointed? | "Grow MAU from 12K to 18K" |
| KR1 | "Increase signups" — by how much? From what baseline? | "Increase weekly signups from 340 to 500 (+47%)" |
| KR2 | "Improve activation rate" — same problem, no number | "Increase D7 activation rate from 23% to 35%" |
| KR3 | "Reduce churn" — which churn? Monthly? Annual? Logo vs. revenue? | "Reduce monthly logo churn from 4.2% to 3.0%" |

**Anti-patterns detected:**
- All three KRs are outputs disguised as outcomes. "Increase signups" is an activity. The outcome is "more users doing [valuable thing]."
- No baseline on any KR — impossible to score at end of quarter.
- Objective uses weasel word "significantly."

**Revised version:**

**Objective: Accelerate user growth to 18K MAU by end of Q3** (currently 12K)
- KR1: Increase weekly organic signups from 340 to 500
- KR2: Raise D7 activation rate from 23% to 35%
- KR3: Reduce monthly logo churn from 4.2% to 3.0%
- KR4: *(consider adding)* Achieve 40% 30-day retention for new cohorts (currently 28%)

**Next step:** Confirm the baselines are accurate, then lock the objective.

---

## Source

Initial raw source: [marfoerst/claude_okr_pm_kill](https://github.com/marfoerst/claude_okr_pm_kill)
