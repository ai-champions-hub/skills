# Agent Deploy Checklist

> Ship an AI agent to production in 45 minutes with a structured checklist.

## Context

You've built an AI agent (using Cursor, LangChain, CrewAI, or any framework) and it works locally. Now you need to get it running in production reliably. This skill walks you through a deployment checklist so nothing falls through the cracks — from environment variables to monitoring.

## Instructions

1. I will describe my agent: what it does, what framework/stack it uses, and where I want to deploy it.
2. Generate a deployment checklist customized to my setup, covering these areas:

   **Pre-deploy**
   - [ ] All API keys and secrets are in environment variables (not hardcoded)
   - [ ] Rate limits and retry logic are implemented for all LLM API calls
   - [ ] Input validation is in place (max token length, content filtering)
   - [ ] Error handling covers: API timeouts, malformed responses, rate limit errors
   - [ ] Cost guardrails: max tokens per request, daily spend cap if applicable
   - [ ] Logging: every LLM call logs prompt hash, model, tokens used, latency, and status

   **Infrastructure**
   - [ ] Deployment target is configured (container, serverless, VM — specify based on my stack)
   - [ ] Health check endpoint exists
   - [ ] Secrets manager is set up (not .env files in production)
   - [ ] Auto-restart / crash recovery is configured

   **Testing**
   - [ ] Tested with realistic inputs (not just happy-path examples)
   - [ ] Tested failure modes: what happens when the LLM is down or returns garbage?
   - [ ] Load tested if user-facing (even a basic k6/locust run)

   **Monitoring & observability**
   - [ ] Alerts on: error rate spike, latency P95 > threshold, cost anomaly
   - [ ] Dashboard or log query for: requests/min, success rate, avg latency, cost/day

   **Post-deploy**
   - [ ] Smoke test in production with a known input
   - [ ] Rollback plan documented (how to revert in < 5 min)
   - [ ] On-call or owner is assigned for the first 48 hours

3. Customize the checklist: remove items that don't apply to my stack, add specifics (e.g., exact commands, file paths) where I've given enough detail.
4. At the end, provide a **"Launch command sequence"** — the exact terminal commands to deploy, in order.

## Example

### Input

```
Agent: a customer support bot that answers questions from our docs. 
Stack: Python, FastAPI, OpenAI API, deployed on Railway.
```

### Output

*(A customized checklist with Railway-specific deploy steps, OpenAI rate limit handling, and a launch sequence like `railway up`, health check verification, smoke test curl command.)*
