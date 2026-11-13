# Burnrate — brakes for AI agents

Agents now hold your API keys and your wallet. Burnrate puts the limits **outside the agent** — hard budgets, action policies and on-chain enforcement — where the agent can't talk its way past them.

| | | |
|---|---|---|
| **Burnrate Shield** | agent-agnostic containment layer for AI-agent wallets: inspects every transaction and blocks the drain **before it is signed** — proven on third-party agent harnesses | [burnrate-shield](https://github.com/Talap-creator/burnrate-shield) · [burnrate-bench](https://github.com/Talap-creator/burnrate-bench) |
| **Burnrate for Claude Code** | live 5h/7d limits, cache-miss watchdog, a brake that blocks subagents and wide scans near the cap | [burnrate](https://github.com/burnrate-ai/burnrate) · [mcp-token-saver](https://github.com/burnrate-ai/mcp-token-saver) |
| **Burnrate Gateway** | OpenAI-compatible proxy: every agent gets its own key, USD budget and rate limit | private beta |
| **Burnrate Vault** | policy vault for AI trading agents on Solana: an AI risk oracle scores the token, the vault refuses the swap | [solana-scam-check](https://github.com/burnrate-ai/solana-scam-check) |

**Proof — independent benchmark.** [burnrate-bench](https://github.com/Talap-creator/burnrate-bench) pits an AI agent under attack with **no shield** vs **with Burnrate Shield**. Without it the agent drains the wallet; with it, contained. Verified live on two third-party harnesses: **SolVerdict** (Solana, scenario A2 full-drain, new shield **20/20**, bare agent 0/20) and **Coinbase AgentKit** (Sepolia, a real on-chain drain blocked). The bench is built to fail the product — it found 5 gaps (which we then closed) and still reports the residuals it has.

**Also — program-risk pipeline.** Our Solana/Anchor pipeline found a real claim-frequency over-mint in GMX-Solana's LP program, reproduced as a PoC over-minting by **56.9%** (Immunefi-confirmed valid finding; a duplicate, so no payout).

```
/plugin marketplace add burnrate-ai/burnrate
/plugin install burnrate@burnrate
```

→ [burnrate-hq.vercel.app](https://burnrate-hq.vercel.app)
