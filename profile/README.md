<div align="center">

# 🦎 Gecko

### The safety & verification layer for trading agents — not another agent.

[![Docs](https://img.shields.io/badge/docs-geckovision.tech-448aff?style=flat-square)](https://docs.geckovision.tech)
[![App](https://img.shields.io/badge/app-app.geckovision.tech-2962ff?style=flat-square)](https://app.geckovision.tech)
[![Install](https://img.shields.io/badge/install-skill.md-82b1ff?style=flat-square)](https://app.geckovision.tech/skill.md)

</div>

---

## Every trading agent tells you it's winning. **Gecko tells you when it's wrong.**

Gecko is a verification layer that sits *above* any trading agent — yours, ours, or anyone's. It is white-label infrastructure: a platform other builders and fintechs embed to make their own agents defensible.

- **Gates every order** against a pre-trade safety check — market-temperature read, price-impact caps, deny-by-default rules. The trade only fires if it survives the gate.
- **Monitors every yield position** against a hurdle rate and a liquidation buffer — and acts *before* a position bleeds.
- **Grades strategies** with default-REJECT backtest rigor (CPCV, PBO, Deflated Sharpe). An honest *null* is a valid, cheap outcome — most "edges" don't survive it.

The wedge is **independence**. Most agents grade their own thesis — the same engine that wants to trade decides whether the trade is good. Gecko is the second opinion that isn't paid when you trade: adversarial multi-voice debate, **surviving dissent**, and citations to external investor canon.

## How it's built

- **Non-custodial.** Signing happens inside a TEE (OKX Agentic Wallet) or a scoped embedded wallet. Keys never leave the enclave. Gecko never holds your private key, and withdrawals are never gated.
- **Pay-as-you-go.** Verdicts are priced per call via x402 on Solana. Self-hosting is free.
- **Venue- & chain-neutral.** Execution dispatches through swappable adapters (OKX, Jupiter, Kamino, Drift). The verification layer works above any of them.
- **Local-first.** Run the agent on your own machine; connect the app as a control surface.

## What's in this org

| Repo | What it is |
|---|---|
| [`gecko-claude`](https://github.com/GeckoVision/gecko-claude) | Public docs, the `skill.md` install surface, and example skills (`curl \| bash` → use) |
| [`gecko-mcpay-api`](https://github.com/GeckoVision/gecko-mcpay-api) | The Python backend — SDK, MCP server, FastAPI, CLI. The verification engine. |
| [`gecko-programs`](https://github.com/GeckoVision/gecko-programs) | Solana programs (custody-probe and on-chain components) |

> The trading bot and the profit vault you'll see in the docs are **proof artifacts** — they demonstrate the verification layer on live capital. The product is the layer, not the bot. We lead with the gate, the dissent, and the rigor — never with a PnL number.

---

<div align="center">

**[Read the docs →](https://docs.geckovision.tech)** · **[Open the app →](https://app.geckovision.tech)** · **[Install the skill →](https://app.geckovision.tech/skill.md)**

</div>
