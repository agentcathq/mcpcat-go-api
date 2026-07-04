# Migrating from `github.com/mcpcat/mcpcat-go-api` to `go.agentcat.com/api`

MCPcat is now AgentCat — same team, same product, new name. This repository is
**frozen**: it receives no new features or dependency updates. Its successor is
[`go.agentcat.com/api`](https://github.com/agentcathq/agentcat-go-api).

## This is an internal client

This module is a generated API client consumed by the SDK. It is **not meant
for direct use** in your applications. If you are integrating analytics into
an MCP server, use the SDK instead:

- New SDK: [`go.agentcat.com/sdk`](https://github.com/agentcathq/agentcat-go-sdk)
  (`go get go.agentcat.com/sdk`)
- Its migration guide:
  [mcpcat-go-sdk MIGRATION.md](https://github.com/agentcathq/mcpcat-go-sdk/blob/main/MIGRATION.md)

## Nothing breaks if you stay

The old module stays published and is not retracted. Existing version pins keep
resolving via the Go module proxy and direct fetch, forever.

## If you do depend on this module directly

Replace the import path:

| Before | After |
| --- | --- |
| `github.com/mcpcat/mcpcat-go-api` | `go.agentcat.com/api` |

```bash
go get go.agentcat.com/api
go mod tidy
```
