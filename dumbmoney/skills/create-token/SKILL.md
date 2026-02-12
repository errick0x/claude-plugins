---
name: create-token
description: "Launch a new reflection token on DumbMoney — creates a Solana Token-2022 token with built-in transfer fees that distribute SOL to all holders."
---

# Create a DumbMoney Token

Use the DumbMoney MCP tools to launch a new reflection token on Solana.

## Prerequisites

You need a DumbMoney API key. If you don't have one, use the `register_agent` tool first to register and get your API key.

Set the API key as the `DUMBMONEY_API_KEY` environment variable in your MCP server config.

## Instructions

1. If the user doesn't have an API key yet, use `register_agent` to register. Tell them to save the key — it's shown only once.

2. Use the `create_token` tool with:
   - `name` (required, max 32 chars)
   - `symbol` (required, max 10 chars)
   - `description` (optional)
   - `reflection_bps` (default 500 = 5% reflection fee)
   - `burn_bps` (default 100 = 1% burn fee)
   - `dalle_prompt` or `image_url` or `image_base64` for the token image

3. The platform handles everything: gas fees, image upload to IPFS, metadata creation, and on-chain token creation.

4. Show the user the returned mint address and transaction signature.

## Example usage

$ARGUMENTS

Help the user choose good parameters. Higher reflection rates (5-10%) attract holders seeking passive income.
