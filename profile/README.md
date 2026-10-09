# Burnrate — brakes for AI agents

Agents now hold your API keys and your wallet. Burnrate puts the limits **outside the agent** — hard budgets, action policies and on-chain enforcement — where the agent can't talk its way past them.

| | | |
|---|---|---|
| **Burnrate for Claude Code** | live 5h/7d limits, cache-miss watchdog, a brake that blocks subagents and wide scans near the cap | [burnrate](https://github.com/burnrate-ai/burnrate) · [mcp-token-saver](https://github.com/burnrate-ai/mcp-token-saver) |
| **Burnrate Gateway** | OpenAI-compatible proxy: every agent gets its own key, USD budget and rate limit | private beta |
| **Burnrate Vault** | policy vault for AI trading agents on Solana: an AI risk oracle scores the token, the vault refuses the swap | [solana-scam-check](https://github.com/burnrate-ai/solana-scam-check) |

```
/plugin marketplace add burnrate-ai/burnrate
/plugin install burnrate@burnrate
```

→ [burnrate-hq.vercel.app](https://burnrate-hq.vercel.app)
