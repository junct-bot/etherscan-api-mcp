# Etherscan MCP Server

MCP server for Etherscan. Agent-ready API for Etherscan.

Hosted at [etherscan-api.mcp.junct.dev/mcp](https://etherscan-api.mcp.junct.dev/mcp). Free to use. No auth. No API key required.

Part of [Junct](https://junct.dev) — the agent-readiness layer for web3.

## Quick Start

Add to your MCP client config (Claude Desktop, Cursor, Windsurf):

```json
{
  "mcpServers": {
    "etherscan-api": {
      "url": "https://etherscan-api.mcp.junct.dev/mcp",
      "transport": "streamable-http"
    }
  }
}
```

## About

This MCP server is **deterministically generated** from the Etherscan API specification. Every tool maps 1:1 to a real API endpoint — no hallucinated endpoints.

- **Protocol:** Etherscan
- **Endpoint:** `https://etherscan-api.mcp.junct.dev/mcp`
- **Transport:** Streamable HTTP
- **Auth:** None required
- **Documentation:** [etherscan-api.mcp.junct.dev/llms.txt](https://etherscan-api.mcp.junct.dev/llms.txt)

## Links

- [Junct Dashboard](https://junct.dev/servers/etherscan-api)
- [llms.txt](https://etherscan-api.mcp.junct.dev/llms.txt)
- [agents.md](https://etherscan-api.mcp.junct.dev/agents.md)
- [OpenAPI spec](https://etherscan-api.mcp.junct.dev/openapi.json)

Keywords: Etherscan, MCP server, DeFi, AI agent, agent-ready API, crypto tools, Model Context Protocol
