<div align="center">

# 🦎 Gecko

### Make any API agent-usable — first-call-correct, no integration code.

[![PyPI](https://img.shields.io/badge/pip-gecko--surf-3775a9?style=flat-square)](https://pypi.org/project/gecko-surf/)
[![Engine](https://img.shields.io/badge/engine-gecko--surf-2962ff?style=flat-square)](https://github.com/GeckoVision/gecko-surf)
[![Site](https://img.shields.io/badge/site-geckovision.tech-448aff?style=flat-square)](https://geckovision.tech)

</div>

---

## The spec is free. The correct first call is not.

Docs and endpoints are built for humans. Coding agents one-shot the clean, well-documented APIs — and break on the **painful** ones: long-tail, paywalled, badly-documented, drifting. Wrong auth, wrong units, wrong shape — the call that fails before it ever reaches the endpoint.

**Gecko is the comprehension layer.** Point an agent at any API's spec and it:

- **Finds the right call** among hundreds of operations.
- **Injects the access** the spec doesn't explain — the auth handshake, the scope.
- **Makes the call correctly the first time** — params, units, idempotency, the exact shape.
- **Stays correct when the API drifts** — tools are a pure function of the surface; re-comprehend, don't hand-patch.

No integration code. **Control-plane only** — we store the API surface + the generated tools + correctness metadata, *never* your payloads, data, or secrets.

## The category line

Marketplaces help agents **discover** APIs. Payment rails help agents **pay** for them. **Gecko makes agents *use* them** — correctly, first call. We **compose on** x402, MCP, and [pay.sh](https://pay.sh) — we don't replace them.

## What we ship

- **[gecko-surf](https://github.com/GeckoVision/gecko-surf)** — the engine (MIT, on PyPI). Turns any OpenAPI 3.x into first-call-correct, question-shaped agent tools, served over MCP.
- **[solana-api-skill](https://github.com/GeckoVision/solana-api-skill)** — make any Solana/crypto API agent-usable (Helius, Jupiter, the CLMM protocols): the comprehension layer under every protocol skill.

## Status (honest)

V1 — comprehension — is **live on Solana mainnet** end-to-end (first-call-correct against a real, paywalled API). The compounding correctness corpus (V2) is designed, not yet built. Consumer willingness-to-pay is the real decider — validating now via discovery interviews. We don't read "a working demo" as "a proven business."

<div align="center">

**Make any API agent-usable.**  ·  [geckovision.tech](https://geckovision.tech)  ·  `pip install gecko-surf`

</div>
