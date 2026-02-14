---
name: mcp-bridge
description: Connect to external MCP servers for extended tool access
version: 1.0.0
author: Cupcake
---

# MCP Bridge

Cupcake can connect to MCP (Model Context Protocol) servers to access external tools.

## Available MCP Endpoints

### n8n MCP Server
- URL: https://automate.hales.ai/webhook/mcp-test/.../sse
- Capabilities: Gmail tools via MCP protocol
- Status: Active (workflow 5wTZ95FtVh1hOAAu)

### OpenClaw MCP Server
- Cupcake can expose itself as an MCP server for other AI tools
- Tools: openclaw_chat, openclaw_status, openclaw_task_list
- Gateway: http://localhost:18789

## Integration Pattern
1. Client connects to MCP server via SSE
2. Server advertises available tools
3. Client calls tools with JSON-RPC
4. Server executes and returns results

## When to Use MCP
- When a direct API isn't available
- When you need standardized tool access across multiple AI systems
- When integrating with Claude Desktop, Cursor, or other MCP-aware clients
