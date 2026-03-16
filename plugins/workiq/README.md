# WorkIQ

Workplace intelligence plugin that connects AI agents to Microsoft 365 Copilot, providing access to organizational data from Outlook, Teams, SharePoint, OneDrive, and Calendar.

## What it does

WorkIQ grounds AI assistance in real workplace context by querying Microsoft 365 data sources. It enables agents to answer questions about:

- **Emails & messages** — Find and summarize email threads and Teams conversations
- **Meetings** — Retrieve decisions, action items, and context from calendar events
- **Documents** — Locate specs, design docs, and files across SharePoint and OneDrive
- **People** — Identify subject-matter experts, project owners, and organizational relationships
- **Priorities** — Surface what colleagues are focused on, team goals, and project status

## Skills

### `workiq`

Activated when a user asks about workplace context — what someone said, meeting outcomes, document locations, team priorities, or organizational knowledge. Uses the `ask_work_iq` MCP tool to query Microsoft 365 Copilot with natural language questions.

## MCP server

WorkIQ includes an MCP server configuration (`.mcp.json`) that runs the `@microsoft/workiq` package. Authentication is automatic using the connected user's existing Microsoft 365 credentials.

## Requirements

- Microsoft 365 account with Copilot access
