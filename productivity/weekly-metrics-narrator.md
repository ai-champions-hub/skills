# Weekly Metrics Narrator

> KPI dashboard → narrated update for stakeholders.

## Context

You have a weekly KPI dashboard (spreadsheet, Looker, Tableau export, or raw numbers) and need to turn it into a clear written summary that leadership can skim in under 2 minutes. This skill generates a narrated update that highlights what changed, why it matters, and what to watch next week.

## Instructions

1. I will paste a set of KPIs with current and previous values.
2. For each metric, calculate the week-over-week change (absolute and percentage).
3. Write a narrated summary in this structure:
   - **Headline**: one sentence capturing the most important takeaway.
   - **Wins**: metrics that improved meaningfully (>5% change or hit a target).
   - **Watch list**: metrics that declined or are trending toward a threshold.
   - **Context**: any external factors I mention that explain the numbers.
   - **Next week**: 1-2 things to monitor based on current trends.
4. Keep the tone professional but conversational — this goes to a Slack channel or email.
5. Use bullet points. No tables. No jargon that wasn't in the original data.
6. If a metric lacks a previous value, note it as "new this week" and skip the comparison.

## Example

### Input

```
Revenue: $142K (last week: $135K)
Active users: 12,400 (last week: 12,800)
NPS: 47 (last week: 44)
Support tickets: 89 (last week: 62)
Churn rate: 2.1% (last week: 1.8%)
```

### Output

**This week in numbers: Revenue up, but churn and support tickets need attention.**

**Wins**
- Revenue climbed to $142K (+$7K / +5.2%) — strongest week this month.
- NPS ticked up to 47 (+3 points), continuing a steady upward trend.

**Watch list**
- Active users dipped to 12,400 (−400 / −3.1%). Worth checking if this is seasonal or tied to the onboarding flow change shipped last Tuesday.
- Support tickets jumped to 89 (+27 / +43.5%). The team should triage by category to spot any new issue clusters.
- Churn rate rose to 2.1% (+0.3pp). Still within acceptable range, but two consecutive weeks of increase would trigger a deeper look.

**Next week**
- Monitor whether the active-user decline continues or rebounds.
- Track support ticket categories to see if the spike is a one-off or a pattern.
