# Deep Research

> An 8-phase research pipeline with source credibility scoring and automated validation.

## What it does

Deep Research is an enterprise-grade research engine for AI agents. It produces citation-backed reports with source credibility scoring, multi-provider search, and automated validation. The output is a polished report (Markdown, HTML in McKinsey style, and PDF) with a full bibliography, evidence chains, and quality checks.

The pipeline runs 5-10 concurrent searches, dispatches 2-3 focused sub-agents for deep dives, triangulates findings across sources, and applies multi-persona red teaming (Skeptical Practitioner, Adversarial Reviewer, Implementation Engineer) before finalizing the report.

## Why it matters

Asking an AI to "research X" typically produces a wall of text with no sources, no validation, and no way to verify claims. Deep Research turns research into a rigorous process: every claim is backed by 3+ sources, every source is scored for credibility, and the final report passes 9 automated quality checks. This is the difference between "AI-generated content" and actual research you can present to stakeholders.

Great for market analysis, competitive intelligence, technology evaluations, and any situation where you need structured research with citations.

## How to install

```bash
git clone https://github.com/199-biotechnologies/claude-deep-research-skill.git ~/.claude/skills/deep-research
```

**Optional** — install `search-cli` for multi-provider search (Brave, Serper, Exa, Jina, Firecrawl):
```bash
brew tap 199-biotechnologies/tap && brew install search-cli
search config set keys.brave YOUR_KEY
```

Without `search-cli`, the skill falls back to the agent's built-in web search.

## Key commands / features

**Usage:**
```
deep research on the current state of quantum computing
deep research in ultradeep mode: compare PostgreSQL vs Supabase for our stack
```

**Research modes:**

| Mode | Phases | Duration | Best for |
|------|--------|----------|----------|
| Quick | 3 | 2-5 min | Initial exploration |
| Standard | 6 | 5-10 min | Most research questions |
| Deep | 8 | 10-20 min | Complex topics, critical decisions |
| UltraDeep | 8+ | 20-45 min | Comprehensive reports, maximum rigor |

**8-phase pipeline:**
1. Scope definition
2. Research plan
3. Parallel retrieval (5-10 searches + sub-agents)
4. Triangulation across sources
5. Outline refinement
6. Synthesis with critique loop-back
7. Multi-persona red teaming
8. Final packaging (Markdown + HTML + PDF)

**Output:**
Reports are saved to `~/Documents/[Topic]_Research_[Date]/` with:
- Markdown (primary source of truth)
- HTML (McKinsey-style, auto-opened in browser)
- PDF (professional print via WeasyPrint)
- `sources.jsonl`, `evidence.jsonl`, `claims.jsonl` for full audit trail

**Quality standards:**
- 10+ sources minimum, 3+ per major claim
- Executive summary 200-400 words
- Full bibliography with URLs, no placeholders
- Automated validation: structure checks + citation/hallucination detection

---

## Source

Initial raw source: [199-biotechnologies/claude-deep-research-skill](https://github.com/199-biotechnologies/claude-deep-research-skill)
