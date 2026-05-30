# Orchestration Planner

> Multi-agent task graph from a goal — plan which agents do what, in what order.

## Context

You want to break down a complex goal into a multi-agent workflow: multiple AI agents (or steps) that each handle a specific subtask, passing outputs to the next. This skill generates the full orchestration plan — agents, their roles, inputs/outputs, dependencies, and execution order.

## Instructions

1. I will describe a goal or workflow I want to automate with multiple agents.
2. Analyze the goal and decompose it into discrete subtasks.
3. For each subtask, define an agent:
   - **Agent name**: short, descriptive (e.g., `ResearchAgent`, `DraftWriter`, `QAReviewer`).
   - **Role**: one sentence describing what this agent does.
   - **Input**: what it receives (from user or from a previous agent).
   - **Output**: what it produces.
   - **Model/tool suggestion**: which LLM or tool fits best (e.g., GPT-4o for reasoning, Claude for long docs, a web scraper for data gathering).
4. Draw the **dependency graph** as a text diagram showing execution order and data flow.
5. Identify which agents can run **in parallel** vs. which must run **sequentially**.
6. Flag any **failure points** — steps where the output quality is critical and a validation/retry loop is recommended.
7. Provide a rough **token/cost estimate** per agent if enough detail is available.

## Example

### Input

```
Goal: Every Monday, generate a competitive intelligence report. 
It should check 3 competitor websites for product updates, 
summarize changes, compare against our roadmap, and produce 
a 1-page brief for the product team.
```

### Output

**Agents**

| # | Agent | Role | Input | Output |
|---|-------|------|-------|--------|
| 1 | `WebScraper` | Fetch latest product/changelog pages from 3 competitor URLs | List of URLs | Raw HTML/text for each site |
| 2 | `ChangeSummarizer` | Summarize product updates from each competitor | Raw page text | Structured summary per competitor |
| 3 | `RoadmapComparer` | Compare competitor updates against our roadmap doc | Summaries + roadmap file | Comparison table with overlap/gaps |
| 4 | `BriefWriter` | Compile everything into a 1-page product brief | Comparison table + summaries | Final markdown brief |
| 5 | `QAReviewer` | Check brief for accuracy, formatting, and completeness | Final brief + source summaries | Approved brief or revision notes |

**Dependency graph**

```
         ┌──── WebScraper (competitor A) ────┐
         │                                    │
Start ───┼──── WebScraper (competitor B) ────┼──→ ChangeSummarizer ──→ RoadmapComparer ──→ BriefWriter ──→ QAReviewer ──→ Done
         │                                    │
         └──── WebScraper (competitor C) ────┘
                   (parallel)                          (sequential chain)
```

**Parallel opportunities**: The three `WebScraper` instances run in parallel. Everything else is sequential.

**Failure points**:
- `WebScraper`: sites may block scraping or change structure. Add retry + fallback (cached version).
- `QAReviewer`: if it flags issues, loop back to `BriefWriter` (max 2 retries).
