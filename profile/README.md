<div align="center">

# 🦎 Gecko

### The decision firewall for Solana.

*Every tool checks the contract. Gecko checks the market is real.*

[![Docs](https://img.shields.io/badge/docs-geckovision.tech-448aff?style=flat-square)](https://docs.geckovision.tech)
[![App](https://img.shields.io/badge/app-app.geckovision.tech-2962ff?style=flat-square)](https://app.geckovision.tech)
[![Install](https://img.shields.io/badge/install-skill.md-82b1ff?style=flat-square)](https://app.geckovision.tech/skill.md)

</div>

---

## Most Solana launches are fake markets. **Gecko tells you before you buy.**

Over half of Solana token launches are sniped in the first block; ~99% of buyers
lose. Every safety tool checks a token's **contract** — mint, freeze, honeypot.
None of them check whether the **market** (price, volume, holders, demand) was
*manufactured* by snipers, wash trades, sybil wallets, or a poisoned oracle. A
token can have clean code and a completely fake market — and that is what drains
people.

**Gecko is the decision firewall:** one pre-trade call tells an AI trading agent or
a launchpad — before any capital moves — whether a launch is **genuine or
manufactured**, as a single `ok / caution / block` + reasons. It fuses behavioral
signals across **wallets × slots × pools** — the market-integrity axis no contract
scanner and no single-venue terminal can see.

> Jito's BAM made *execution* trustworthy. **Gecko makes the *decision* trustworthy.**
> Execution has BAM. Decisions have Gecko.

## The moat

Every verdict is **committed before a launch resolves, then graded by outcome** — a
time-stamped, outcome-labeled record of what was fake that no competitor can
backfill. A rival can clone the detector and outspend us on distribution, but they
cannot backfill a pre-commitment they never made. *Distribution buys traffic, not
truth.*

## How it's built

- **Verify, never execute.** Gecko reads the market and returns a verdict. It never trades, custodies funds, or reorders transactions.
- **Agent-native + verifiable.** A neutral, callable, pre-trade verdict (not a human dashboard), and every verdict can carry an on-chain **Decision Receipt** — proof it preceded the outcome.
- **Pay-as-you-go.** The free `/safety` firewall is the wedge; the deep oracle (multi-voice debate + surviving dissent + citations) is priced per call via x402 on Solana.
- **Neutral.** Distributed where agents already run — a SendAI / Solana Agent Kit adapter, MCP, and direct launchpad integrations.

## ⚠️ Status (honest)

The firewall **engine** is real and **fork-proven**; the on-chain **Decision
Receipt** is **devnet-verified**; the **verdict ledger** writes its first rows. The
firewall is **DARK in production**, and **live-launch detection precision is not yet
proven** — the real-launch backtest (the gate to charging) showed the current
signals over-block, and a re-tune is underway. We ship what's proven and never claim
live accuracy we haven't earned.

## What's in this org

| Repo | What it is |
|---|---|
| [`gecko-mcpay-api`](https://github.com/GeckoVision/gecko-mcpay-api) | The Python backend — the firewall engine, SDK, MCP server, FastAPI, CLI. **Positioning source of truth.** |
| [`gecko-claude`](https://github.com/GeckoVision/gecko-claude) | Public docs, the `skill.md` install surface, and the Claude Code skills (`curl \| bash` → use) |
| [`gecko-mcpay-app`](https://github.com/GeckoVision/gecko-mcpay-app) | The Next.js app at `app.geckovision.tech` |
| [`gecko-programs`](https://github.com/GeckoVision/gecko-programs) | Solana programs — Token-2022 firewall hook + Decision Receipt PDA (devnet-only) |

> The trade oracle and trading bot you'll see in the docs are the engine's deeper
> paid layer and a **proof artifact** — they demonstrate the verification stack. The
> product is the firewall. We lead with the verdict, the dissent, and the rigor —
> never with a PnL number.

---

<div align="center">

**[Read the docs →](https://docs.geckovision.tech)** · **[Open the app →](https://app.geckovision.tech)** · **[Install the skill →](https://app.geckovision.tech/skill.md)**

</div>
