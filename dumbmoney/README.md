# DumbMoney Claude Plugin

Claude Code plugin for [DumbMoney](https://dumbmoney.win) — Solana's reflection token launchpad where holders earn passive SOL income from every trade.

## What It Does

This plugin gives Claude Code access to the DumbMoney platform via MCP tools:

| Tool | Description |
|------|-------------|
| `list_tokens` | List all reflection tokens with price, market cap, and reflection rates |
| `get_token` | Get detailed info about a specific token by mint address |
| `check_earnings` | Check a wallet's pending SOL earnings for a token |
| `top_earners` | Top 10 tokens ranked by total reflections paid |
| `register_agent` | Register as an AI agent to get an API key |
| `get_my_agent_info` | Check your agent profile and rate limits |
| `create_token` | Launch a new reflection token on-chain |

## Installation

### Claude Code

```bash
claude plugin marketplace add errick0x/dumbmoney
claude plugin install dumbmoney@dumbmoney
```

### Other Coding Tools

```bash
bunx skills add errick0x/dumbmoney
```

## Configuration

Read-only operations (browsing tokens, checking earnings) work out of the box.

To create tokens, register as an agent first (the `register_agent` tool handles this), then set your API key:

```json
{
  "mcpServers": {
    "dumbmoney": {
      "command": "npx",
      "args": ["@dumbmoney/mcp-server"],
      "env": {
        "DUMBMONEY_API_KEY": "dm_live_your_key_here"
      }
    }
  }
}
```

## Skills

| Skill | Description |
|-------|-------------|
| `/dumbmoney:browse-tokens` | Browse and explore reflection tokens |
| `/dumbmoney:create-token` | Launch a new reflection token |
| `/dumbmoney:check-earnings` | Check pending SOL earnings |

## Links

- Website: https://dumbmoney.win
- API docs: https://dumbmoney.win/llms.txt
- OpenAPI spec: https://dumbmoney.win/openapi.json
