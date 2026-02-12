# DumbMoney Claude Plugins

Claude Code plugins for [DumbMoney](https://dumbmoney.win) — Solana's reflection token launchpad.

## Available Plugins

| Plugin | Description |
|--------|-------------|
| **[dumbmoney](./dumbmoney/)** | Browse tokens, check earnings, create reflection tokens, register as an AI agent |

## Installation

### Claude Code

```bash
claude plugin marketplace add errick0x/claude-plugins
claude plugin install dumbmoney@dumbmoney-claude-plugins
```

### Other Coding Tools (Skills only)

```bash
bunx skills add errick0x/claude-plugins
```

## Requirements

- Claude Code CLI or compatible coding tool
- Node.js 18+
- (Optional) DumbMoney API key for token creation — get one via the `register_agent` tool

## Links

- Website: https://dumbmoney.win
- API docs: https://dumbmoney.win/llms.txt
- OpenAPI spec: https://dumbmoney.win/openapi.json
- MCP Server: [@dumbmoney/mcp-server](https://www.npmjs.com/package/@dumbmoney/mcp-server)
