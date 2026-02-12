---
name: check-earnings
description: "Check your pending reflection earnings on DumbMoney — see how much SOL you've earned from holding reflection tokens."
---

# Check DumbMoney Earnings

Use the DumbMoney MCP tools to check reflection earnings for a wallet.

## Instructions

1. You need two pieces of info:
   - The token's **mint address** (Solana base58 address)
   - The holder's **wallet address** (Solana base58 address)

2. Use the `check_earnings` tool with both addresses.

3. The response includes:
   - `pendingSol` — pending SOL earnings
   - `pendingUsd` — USD value of earnings
   - `sharePercent` — your share of the reflection pool
   - `holderShares` / `totalShares` — your position relative to all holders

4. If the user wants to check earnings across multiple tokens, use `list_tokens` first to get all tokens, then check earnings for each one they hold.

## Example usage

$ARGUMENTS

Present the earnings in a clear format. If the wallet has significant earnings, highlight the passive income angle.
