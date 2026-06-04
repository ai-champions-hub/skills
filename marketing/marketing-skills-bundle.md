# Marketing Skills Bundle

> A comprehensive pack of 42 marketing skills: CRO, copywriting, SEO, analytics, ads, growth, retention, and sales enablement.

## Context

You need a full marketing toolkit that covers the entire funnel — from positioning and messaging to SEO, paid ads, email sequences, retention, and sales enablement. This bundle provides 42 specialized skills that cross-reference each other, with `product-marketing` as the foundation skill. Configure it once for your brand (audience, tone, positioning) and stop re-explaining to the agent who your audience is and what style to use.

Works with Claude Code, Cursor, Codex, Windsurf, and any Agent Skills-compatible runtime.

## Instructions

This is a bundle, not a single skill. Install it once and the individual skills become available in your agent session. The key skills include:

**Positioning & Messaging**
- Product Marketing (foundation skill — configure once with your brand context)
- Positioning Framework (Geoffrey Moore-style positioning statement)
- Messaging Matrix (audience segments × key messages × proof points)
- Competitive Analysis (feature matrix, positioning gaps, battlecards)

**Content & Copy**
- Copywriting (headlines, landing pages, email subject lines)
- Blog Strategy (topic clusters, content calendar, SEO alignment)
- Social Media (platform-specific content, scheduling, engagement)
- Case Study Writer (customer story extraction and formatting)

**SEO & Analytics**
- SEO Audit (technical SEO, on-page, content gaps)
- Keyword Research (intent mapping, difficulty/volume analysis)
- Analytics Setup (GA4 configuration, event tracking, dashboards)
- Conversion Rate Optimization (A/B test design, funnel analysis)

**Paid Acquisition**
- Google Ads (campaign structure, ad copy, bidding strategy)
- Meta Ads (audience targeting, creative strategy, budget allocation)
- Landing Page Optimization (above-fold, CTA, social proof)

**Email & Retention**
- Email Sequences (onboarding, nurture, re-engagement, win-back)
- Newsletter Strategy (content mix, growth tactics, monetization)
- Retention Analysis (cohort analysis, churn drivers, intervention design)

**Sales Enablement**
- Sales Deck Builder (narrative arc, objection handling slides)
- Battlecard Generator (competitive positioning, talk tracks)
- Demo Script (feature-benefit mapping, discovery questions)

## How to install

**Note:** This is an external package or integration, not a local one-file skill. Follow the install instructions below rather than copying it into `skills/`.

```bash
npx skills add coreyhaines31/marketingskills
```

Or clone manually:
```bash
git clone https://github.com/coreyhaines31/marketingskills.git ~/.claude/skills/marketing
```

## How to use

After installation, start with the product-marketing foundation skill to set your brand context:
```
Use the product-marketing skill to set up my brand context. My company is [name], 
we sell [product] to [audience].
```

Then invoke any specific skill:
```
Use the seo-audit skill to review my website at [url]
Use the copywriting skill to write a landing page headline for [feature]
Use the email-sequences skill to create an onboarding sequence for [product]
```

Skills cross-reference each other — the copywriting skill pulls tone and positioning from the product-marketing foundation, the SEO skill feeds into the blog strategy, etc.

---

## Source

Initial raw source: [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills)
