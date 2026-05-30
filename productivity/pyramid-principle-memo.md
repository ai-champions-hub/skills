# Pyramid Principle Memo Writer

> Topic + key arguments → strategic memo structured using Barbara Minto's Pyramid Principle.

## Context

You need to write a strategic memo, board note, investment thesis, or executive brief. This skill applies Barbara Minto's Pyramid Principle — governing thought first, insight-statement headers, first-sentence test — to produce documents that busy executives can read top-down, getting the conclusion first and drilling into evidence only if they want to. This is the closest publicly available substitute for the Amazon 6-pager pattern.

Use for: strategy docs, board presentations, investment memos, executive decision briefs, quarterly business reviews, and any document where the reader's time is extremely limited.

## Instructions

1. I will describe the topic, the decision or recommendation, and any supporting arguments or data I have.

2. **Apply the Pyramid Principle structure:**

   **Governing Thought** (1-2 sentences at the top)
   - The single most important conclusion, recommendation, or insight
   - This is what the reader should take away even if they read nothing else
   - Must be actionable: "We should do X because Y" — not "This document explores X"

   **Key Arguments** (3-5 sections, each with an insight-statement header)
   - Each section header is a complete sentence that states the insight, not a label
   - BAD: "Market Analysis" / GOOD: "The addressable market grew 34% YoY, driven by SMB adoption"
   - Each section supports the governing thought with evidence
   - Order: strongest argument first, or logical sequence if arguments build on each other

   **Supporting Evidence** (within each section)
   - Data points, examples, comparisons, quotes
   - Specific numbers beat adjectives
   - Source citations where applicable

   **Implications / Next Steps** (final section)
   - What the reader needs to decide or approve
   - Timeline and ownership
   - Risks of inaction

3. **Apply the first-sentence test:** every paragraph's first sentence should convey the paragraph's main point. A reader skimming only first sentences should get the full argument.

4. **Formatting rules:**
   - Total length: 1-3 pages (500-1500 words)
   - Short paragraphs (max 4 sentences)
   - Use bold for key figures and conclusions
   - Use tables for comparisons (max 5 rows)
   - No bullet-point lists longer than 5 items
   - No jargon the intended reader wouldn't know

5. **Anti-patterns to avoid:**
   - Burying the recommendation at the end
   - Label headers instead of insight-statement headers
   - Leading with methodology/process instead of conclusions
   - Hedging language: "it might be worth considering" → "we should"
   - Listing data without interpreting it

## Example

### Input

```
I need to write a memo recommending we sunset our freemium tier and move 
to a free trial model. Key points: freemium users convert at 2.1% vs 
industry average 5%, support cost per freemium user is $4.20/mo, free trial 
converts at 14% in our A/B test, we're losing $380K/year on freemium support 
costs, and three competitors switched to free trial in the last 6 months.
```

### Output

**MEMO: Sunset the freemium tier and switch to 14-day free trial**

**Recommendation:** Sunset our freemium tier and replace it with a 14-day free trial. Our A/B test shows 14% trial-to-paid conversion vs. 2.1% freemium conversion, and the switch eliminates $380K/year in freemium support costs.

---

**Our freemium conversion rate is less than half the industry benchmark.** Our freemium-to-paid conversion rate is 2.1%, compared to a 5% industry average for comparable SaaS products. Of the 12,400 freemium users active in the last 90 days, only 260 converted to paid. The median time from signup to conversion is 47 days — suggesting that users who will convert do so within the first month, and long-tail freemium users rarely upgrade.

**Freemium support costs consume $380K/year with negative ROI.** Each freemium user costs $4.20/month in support (tickets, infrastructure, onboarding emails). Across 7,500 monthly active freemium users, that's **$31.5K/month or $378K/year**. The lifetime revenue of a converted freemium user ($840 average) does not offset the cumulative support cost for the 97.9% who never convert.

**A 14-day free trial converts at 6.7x the rate of freemium.** In our 8-week A/B test (n=2,400), the free trial arm converted at **14%** vs. 2.1% for the freemium control. Trial users engaged with 3.2x more features during their first week, suggesting the time constraint drives exploration. Net revenue per cohort was 4.1x higher in the trial arm.

**The market is moving in the same direction.** Three direct competitors (Acme, Widget Co, and ToolStack) switched from freemium to free trial in the last 6 months. Acme publicly reported a 2.8x increase in conversion rate post-switch. We risk becoming the "free alternative" in the category if we remain the only freemium option.

---

**Next steps:**
1. **Approve the switch** — decision needed by June 15 to hit Q3 launch
2. **Migration plan** — existing freemium users get 90-day grace period with upgrade prompts (PM owns, 2-week design)
3. **Risk:** ~15% of freemium users will churn loudly on social media. Mitigation: proactive email campaign + discounted annual plan for long-standing users

---

## Source

Initial raw source: [mcpmarket.com/tools/skills/ceo-advisor-strategic-leadership](https://mcpmarket.com/tools/skills/ceo-advisor-strategic-leadership)
