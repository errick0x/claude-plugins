---
name: browse-tokens
description: "Browse DumbMoney reflection tokens on Solana — list all tokens, get details, check top earners, and find high-yield passive income opportunities."
---

# Browse DumbMoney Tokens

Use the DumbMoney MCP tools to explore reflection tokens on Solana.

## Instructions

When the user wants to browse or explore DumbMoney tokens, use these MCP tools:

1. **List all tokens**: Use the `list_tokens` tool to get all available reflection tokens with their prices, reflection rates, and bonding curve progress.

2. **Get token details**: Use the `get_token` tool with a Solana mint address to get detailed on-chain data for a specific token.

3. **Find top earners**: Use the `top_earners` tool to see the top 10 tokens ranked by total reflections paid to holders.

4. **Check earnings**: Use the `check_earnings` tool with a mint address and wallet address to see pending SOL earnings.

## Key concepts

- **Reflection rate**: Percentage of each sell distributed to holders as SOL (e.g., 5% = 500 bps)
- **Bonding curve**: Tokens launch on a bonding curve and graduate to Raydium at ~$69k market cap
- **Passive income**: Holders earn SOL automatically — no staking, no claiming needed

## Example usage

$ARGUMENTS

If no specific request, show the top earning tokens and highlight those with high reflection rates.
