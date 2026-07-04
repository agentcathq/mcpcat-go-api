> [!IMPORTANT]
> **MCPcat is now AgentCat 🐱** — same team, same product, new name.
> This module is **frozen**. It keeps working forever (nothing is retracted, old version pins keep resolving), but new development happens in **[`go.agentcat.com/api`](https://github.com/agentcathq/agentcat-go-api)**.
> This is an internal generated client consumed by the SDK — don't use it directly. See **[MIGRATION.md](./MIGRATION.md)**.

# ⚠️ This is NOT the MCPCat Go SDK

**This directory contains internal API client code used by the MCPCat Go SDK. It is not intended for direct use.**

## Looking for the MCPCat Go SDK?

The official MCPCat Go SDK for integrating MCPCat analytics into your MCP servers is located at:

**https://github.com/mcpcat/mcpcat-go-sdk**

## What is this directory?

This directory (`mcpcat-go-api`) contains internal API client implementation code that is used as a dependency within the MCPCat Go SDK. It provides low-level API communication functionality and should not be used directly in your applications.

## For MCP Server Developers

If you're building an MCP server and want to add MCPCat analytics:
- ✅ Use the official Go SDK: https://github.com/mcpcat/mcpcat-go-sdk
- ❌ Do NOT use this internal API client directly
