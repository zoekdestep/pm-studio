# Connectors

PM Studio uses MCP connectors to pull external data into every command. WorkIQ is the default connector and is always active. Other connectors are optional and use `~~category` conditional patterns.

## WorkIQ (Always On)

WorkIQ provides access to Microsoft 365 data: Outlook emails, Teams meetings and transcripts, OneDrive/SharePoint documents.

**Every command queries WorkIQ by default.** You do not need to ask for it. If you don't want WorkIQ data for a specific command, tell Claude to skip it.

**Configured in:** `.mcp.json` (starts automatically)

**What it provides:**

| Data Type | Examples |
|-----------|---------|
| Emails | Related threads, customer feedback, stakeholder discussions |
| Meetings | Transcripts, summaries, action items |
| Documents | Strategy docs, specs, decision records in SharePoint/OneDrive |
| Chat | Teams discussions and decisions |

**Setup:**
1. WorkIQ is pre-configured in `.mcp.json` and starts automatically
2. On first use, accept the EULA when prompted
3. Sign in with your Microsoft account

## Optional Connectors

Commands may reference `~~category` placeholders for additional data sources. These are conditional: if the connector isn't available, the section is skipped silently.

| Category | What it provides | Used by |
|----------|-----------------|---------|
| `~~product analytics` | Usage metrics, trends, behavioral data | `/strategy`, `/shipping` |
| `~~user feedback` | Support tickets, feature requests, sentiment | `/shipping`, `/note` |
| `~~project tracker` | Rollout status, work items, bugs | `/shipping` |

The `~~` prefix signals a conditional check. If no MCP server maps to that category, Claude skips the block and works with what it has.

## Plugin Connectors

The product-management plugin defines its own connectors in its `CONNECTORS.md`. Those connectors apply to plugin commands (`/product-management:*`). PM Studio's CLAUDE.md also instructs Claude to always query WorkIQ for plugin commands.

## Adding More Connectors

To add a new MCP server:

1. Add it to `.mcp.json`:
```json
{
  "mcpServers": {
    "workiq": { ... },
    "your-server": {
      "command": "npx",
      "args": ["-y", "@your-org/your-mcp-server"]
    }
  }
}
```

2. Map it to a `~~category` by updating the commands that should use it.
