# Meeting Notes to Memo

> Transcript → exec-ready memo with decisions, action items, and open questions.

## Context

After a meeting you have a raw transcript or rough notes. You need a clean, structured memo that anyone who missed the meeting can read in 2 minutes and know exactly what was decided, who owns what, and what's still unresolved.

## Instructions

1. I will paste a meeting transcript or rough notes.
2. Produce a memo with these sections:
   - **Meeting**: title, date, attendees (extract from transcript if possible).
   - **TL;DR**: 2-3 sentence summary of what happened.
   - **Decisions made**: numbered list of concrete decisions. Include who made or approved each one.
   - **Action items**: table with columns: Action | Owner | Due date. If no due date was mentioned, write "TBD".
   - **Open questions**: anything raised but not resolved.
   - **Key quotes**: (optional) 1-2 direct quotes that capture important context or rationale.
3. Keep language crisp and factual. No editorializing.
4. If something is ambiguous in the notes, flag it with "[unclear from notes]" rather than guessing.
5. Format the memo so it can be pasted directly into Slack, Notion, or email.

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

**Meeting**: Launch timeline standup — May 28
**Attendees**: Author, Sarah, James

**TL;DR**
The team aligned on a two-phase launch: internal soft launch on June 7, public launch on June 10. Load testing will happen in between. Pricing page ownership is still unassigned.

**Decisions made**
1. Keep June 10 as the external launch date (per James — marketing already announced).
2. Add a soft launch on June 7 for internal users to de-risk (proposed by Sarah, agreed by all).

**Action items**

| Action | Owner | Due |
|--------|-------|-----|
| Update landing page copy | James | Friday May 30 |
| Set up load test environment | Sarah (+ DevOps) | TBD |
| Draft internal launch comms | Author | TBD |

**Open questions**
- Who owns the pricing page? Raised but not assigned.
