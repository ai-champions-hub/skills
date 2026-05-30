# Composio

> MCP integration layer that gives AI agents direct access to 500+ external services.

## What it does

Composio is not a skill but an MCP (Model Context Protocol) integration that connects AI agents to external services. Gmail, Slack, GitHub, Notion, Telegram, Figma, Google Sheets, Salesforce, Jira, Linear, and 500+ more apps become directly accessible from within your agent session. Claude executes actions inside these services, manages authorization (OAuth, API keys), and automates workflows across multiple tools at once.

Think of it as the plumbing that lets your AI agent actually *do things* in the real world instead of just generating text about doing things.

## Why it matters

Without Composio (or similar MCP integrations), the agent can only read and write files on your local machine. With it, the agent can send emails, post to Slack, create GitHub issues, update Notion databases, schedule calendar events, and orchestrate multi-tool workflows — all from a single conversation.

This is especially powerful for non-developers who need AI to operate across their existing tool stack without writing any integration code.

## How to install

1. **Sign up** at [composio.dev](https://composio.dev)
2. **Connect your tools** via the Composio dashboard (OAuth flow for each service)
3. **Add the MCP server** to your agent:

**Cursor** — add to `.cursor/mcp.json`:
```json
{
  "mcpServers": {
    "composio": {
      "url": "https://mcp.composio.dev/sse?api_key=YOUR_API_KEY"
    }
  }
}
```

**Claude Code** — add via Claude Code MCP settings.

4. **Verify** by asking your agent to list available Composio tools.

## Key features

- **500+ app integrations** — Gmail, Slack, GitHub, Notion, Figma, Google Sheets, Salesforce, Jira, Linear, Airtable, Stripe, HubSpot, and more
- **Managed auth** — handles OAuth flows, token refresh, and API key management
- **Action execution** — the agent doesn't just read data, it takes actions (send email, create issue, post message)
- **Multi-tool workflows** — chain actions across services (e.g., "when a GitHub issue is created, post to Slack and add to Notion")
- **Custom actions** — define your own actions for internal tools

## Example use cases

- "Send a weekly summary email to the team based on this week's GitHub activity"
- "Create a Notion page from these meeting notes and post the link to Slack"
- "Draft a reply to the latest unread email from [person] and wait for my approval before sending"
- "Pull the latest metrics from Google Sheets and create a status update in Linear"

---

## Source

Initial raw source: [Composio](https://composio.dev/toolkits/composio/framework/claude-code)
