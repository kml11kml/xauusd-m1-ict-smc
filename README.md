# XAUUSD M1 ICT SMC — Claude Code Skill for Gold Scalping

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/kml11kml/xauusd-m1-ict-smc)](https://github.com/kml11kml/xauusd-m1-ict-smc/stargazers)
[![Claude Code Skill](https://img.shields.io/badge/Claude_Code-Agent_Skill-blueviolet)](https://github.com/anthropics/skills)
[![XAUUSD](https://img.shields.io/badge/XAUUSD-M1_ICT_SMC-gold)](https://github.com/kml11kml/xauusd-m1-ict-smc)

**Analyse OANDA XAUUSD (gold) on the 1-minute chart with multi-timeframe ICT SMC, a LIT trap filter and Cyzner bias discipline — and get one confirmed setup or WAIT, in short Persian.**

Most gold-trading prompts guess. This skill doesn't: it locks the H4 bias and H1 key levels first, waits for a liquidity sweep, then requires displacement, a market structure shift and a fair value gap retest before it ever proposes an entry. No sweep, no displacement, no shift — no trade. It returns **WAIT**.

## What it does

- **Multi-timeframe ICT SMC:** H4 bias → H1 key levels → M15 setup → M1 execution
- **Liquidity first:** trades only at liquidity pools (BSL/SSL, PDH/PDL, session highs/lows, equal highs/lows)
- **LIT trap filter:** the first pullback and the obvious equal high/low are treated as inducement by default; the real point of interest is the deeper order block or FVG behind it
- **Kill zones only:** London 11:30–14:30 and New York 16:30–19:30 Tehran, Monday to Friday
- **Tight risk:** stop 2.5–5$ behind the M1 shift swing, never behind an H1/M15 level; minimum reward-to-risk 1:2
- **Scored decisions:** at least 60/100 to propose an entry, otherwise WAIT
- **Short Persian output:** one setup or WAIT — entry, stop, TP1, TP2, invalidation, confidence

## Quick start

### Option A — install with the skills CLI

```bash
npx skills add kml11kml/xauusd-m1-ict-smc
```

### Option B — manual install (Claude Code)

```bash
mkdir -p ~/.claude/skills
cp -r xauusd-m1-ict-smc ~/.claude/skills/
```

Then ask Claude Code for an XAUUSD M1 analysis. The skill triggers on gold / XAUUSD scalping requests.

## How it works

```
H4 bias → H1 key levels → M15 setup
        → M1 sweep → displacement → market structure shift → FVG / OB retest
        → score ≥ 60 → one setup, or WAIT
```

| Step | Rule |
| --- | --- |
| Bias | H4 structure + nearest external liquidity pool; neutral bias = trade range edges only |
| Levels | H1 PDH/PDL, prior day high/low, session high/low, Asia high/low, midnight open (00:00 ET) |
| Kill zone | London 11:30–14:30 / New York 16:30–19:30 Tehran, Mon–Fri; skip ±30 min around red-folder US data (NFP, CPI, FOMC) |
| Sweep | Wick beyond a named pool, close back inside; a close through that holds is a real break — never fade it |
| Displacement | Full-bodied M1 candles closing decisively through structure, leaving a fair value gap |
| Entry | Pullback into the displacement-leg FVG / order block only; buy in discount, sell in premium |
| Risk | SL 2.5–5$ max behind the M1 MSS swing; TP1 = 2× SL, TP2 = next liquidity pool; one setup per kill zone |

## Example output

```
Live 4037 · 18:05 Tehran · Day high 4107 · Day low 4030
Bias: bearish H4 / H1 / M15
BSL 4107 · SSL 4030 · OB 4056–4064 · Bearish FVGs 4077–4082, 4085
WAIT — no fresh sweep + displacement + MSS + FVG in kill zone
```

(The example above is a test case from 2026-11-06, not a live signal. Always verify the live price before any use.)

## Why this skill

- **One sequence, no guessing:** sweep → displacement → shift → gap. Every box must be ticked.
- **Traps filtered out:** LIT inducement veto — if the entry itself is the inducement, the trade is vetoed.
- **Bank-trader discipline:** mid-range is a no-trade zone; no chasing, no FOMO, no revenge trading; stop for the session after two consecutive losses.
- **Built from free public sources:** Michael ICT 2022/2024 Mentorship, ReimFX LIT, Ben Cyzner / TradeX Labs — paraphrased, no pirated PDFs.

## FAQ

**Does this skill place trades?**
No. It analyses and proposes one setup or WAIT. It never executes a trade.

**Is it financial advice?**
No. It has no verified win rate and no backtest on M1 gold. Use it as an analysis framework, not a money-making product.

**Which markets and timeframes?**
OANDA XAUUSD (gold), M1 execution with H4 / H1 / M15 context. The rules are gold-specific (dollar stops, Tehran kill zones).

**Which AI tools does it work with?**
Claude Code, and any agent that loads `SKILL.md` files (Cursor, Codex, OpenCode via the skills CLI).

**What do I need for live prices?**
A live price feed or chart (e.g. TradingView). The skill uses closed candles and verified live prices only — it never invents a level or a price.

## Files

- `SKILL.md` — the full rule set
- `references/mtf-checklist.md` — multi-timeframe checklist with a worked example
- `skill.yaml` — skill metadata

## Custom work

Need a custom Claude Code skill, plugin or MCP built for your workflow? Ask about custom builds.

## Licence

MIT — see [LICENSE](LICENSE).
