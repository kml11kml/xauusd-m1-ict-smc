# XAUUSD M1 ICT SMC Analysis

Analyse OANDA XAUUSD on M1 with multi-timeframe ICT SMC plus LIT trap filter and Cyzner bias discipline, and give one confirmed setup or WAIT in short Persian.

A Claude Code skill combining Michael ICT (2022/2024 Mentorship, free public sources), ReimFX LIT (Liquidity Inducement Theory) and Ben Cyzner / TradeX Labs discipline into one deterministic sequence:

H4 bias → H1 key levels → M15 setup → M1 execution only after sweep → displacement → market structure shift → FVG / order-block retest.

Rules baked in: trade only in London / New York kill zones, only at liquidity pools, buys only in discount / sells only in premium, tight stop 2.5–5$ behind the M1 shift swing, minimum reward-to-risk 1:2, score ≥ 60/100, otherwise WAIT. Output is one setup or WAIT, in short Persian.

## Install (Claude Code)

```bash
mkdir -p ~/.claude/skills
cp -r xauusd-m1-ict-smc ~/.claude/skills/
```

Then ask Claude Code for an XAUUSD M1 analysis; the skill triggers on gold / XAUUSD scalping requests.

## Files

- `SKILL.md` — the full rule set
- `references/mtf-checklist.md` — multi-timeframe checklist
- `skill.yaml` — skill metadata

## Honest limits

- NOT financial advice. No verified win rate, no backtest on M1 gold.
- Do not use it as a money-making trading product. Its value is as a working example of a structured ICT/SMC skill.
- Sources are paraphrased from free public material only; no pirated PDFs were used.

## Custom work

Need a custom Claude Code skill, plugin or MCP built for your workflow? Ask about custom builds.

## Licence

MIT — see [LICENSE](LICENSE).
