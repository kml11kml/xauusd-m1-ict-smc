# XAUUSD M1 ICT SMC Analysis

Use this skill for every XAUUSD M1 scalp analysis for Ali. It combines Michael Huddleston ICT, ReimFX LIT Liquidity Inducement Theory, and Ben Cyzner TradeX Labs discipline into one deterministic sequence. It never forces a trade. It uses only closed candles and verified live prices. It never invents a level or a price.

## Lock the higher timeframes first

- Decide the H4 bias before you look at M1.
- Score the bias from H4 structure and the nearest external liquidity pool.
- Treat a neutral bias as a range bias and trade only at the range edges.
- Lock the H1 key levels once per session and reuse them for fast checks.
- Mark prior day high and low and session high and low and Asia high and low and the dealing range equilibrium.
- Mark internal range liquidity inside the range separately from external range liquidity outside the range.
- Note the midnight open at 00 00 New York time as the daily fulcrum.
- Treat price above the midnight open as expensive and price below it as cheap.
- Re-lock a level only after a closed 1m candle beyond it.
- Read the full locked level list and the M15 checklist in [references/mtf-checklist.md](references/mtf-checklist.md).

## Trade only in a kill zone

- Trade only in London 11 30 to 14 30 Tehran or New York 16 30 to 19 30 Tehran on Monday to Friday in winter time.
- Convert the windows with daylight saving time when New York moves between EST and EDT.
- Stay out of Asia range building time and out of the lunch drift.
- Skip every new entry for 30 minutes before and after red folder United States data such as NFP and CPI and FOMC.
- Trade the post news structure after the data and never trade the headline candle itself.
- Treat a perfect shape outside a kill zone as no trade.

## Apply the LIT trap filter

- Ask whether an inducement sits in front of the point of interest.
- Treat the first pullback and the nearest minor swing and the obvious equal high or low as inducement by default.
- Treat the deeper order block or fair value gap behind that inducement as the real point of interest.
- Mark a fresh Malaysian support and resistance level only when no wick has touched it yet.
- Treat a wicked level as unfresh and do not fade it.
- Check quarterly theory only as a timing tie breaker and never trade it alone.
- Let H4 win whenever quarterly theory disagrees with H4.
- Check smart money divergence on M5 to M15 only when you can do it fast.
- Treat a silver or dollar non confirmation as one extra confluence point and never delay an M1 entry to wait for a second chart.
- Veto the trade when the entry itself is the inducement.

## Wait for sweep then displacement then shift then gap

- Wait for a sweep against the bias in a kill zone.
- Require a wick beyond a named pool and a close back inside the range.
- Treat a close through the pool that holds as a real break and never fade it.
- Require displacement after the sweep on closed M1 candles.
- Require full bodied candles that close decisively through structure and leave a fair value gap.
- Require a market structure shift on M1 after displacement.
- Record the swing price and the time of the shift.
- Enter only on the pullback into the displacement leg fair value gap or order block.
- Prefer the 50 percent consequent encroachment of that gap.
- Use only the first presented gap from the displacement leg and ignore stale gaps.
- Check premium and discount on M15 before entry.
- Buy only in discount and sell only in premium.
- Use optimal trade entry at 61 8 to 78 6 percent on M15 as a zone filter and never enter M1 on Fibonacci alone.

## Size risk and set targets

- Place the stop behind the M1 market structure shift swing and never behind an H1 or M15 level.
- Clamp the stop to 2 5 to 5 dollars maximum on gold.
- Skip the setup when the sweep extreme stop is wider than 5 dollars.
- Require reward to risk of at least 1 to 2 before you propose an entry.
- Set the first target at 2 times the stop and the second target at the next liquidity pool.
- Take a partial at the first target and move the stop to breakeven for the runner.
- Take only one best setup per kill zone.
- Stop for the session after two consecutive losses.
- Exit when a closed 1m candle goes beyond the shift swing or beyond the sweep extreme in the wrong direction.
- Log the sweep pool and the shift price and the gap and the stop and the targets and the outcome for every check.

## Score the setup before you decide

- Score bias plus sweep plus displacement plus shift plus gap plus premium discount plus kill zone plus optimal trade entry overlap.
- Add 2 points for a sweep of external liquidity and 1 point for a swept inducement before the point of interest.
- Add 1 point for a fresh Malaysian level and 1 point for a held gap retest and 1 point for smart money non confirmation.
- Subtract 2 points when the entry is the inducement and 2 points for a body close break and hold and 2 points outside a kill zone.
- Require at least 60 out of 100 before you propose an entry.
- Return WAIT when any required box is unticked.
- Return WAIT when the score is below threshold even when the shape looks good.

## Present the result in short Persian

- Give the live price and the time in Tehran and the day high and the day low first.
- Give the H4 and H1 bias in one line.
- Give the buy side and sell side liquidity pools and the resistance and the support and the order block and the bearish or bullish gaps.
- Give only one setup or WAIT and never give two competing entries.
- Give entry and stop and first target and second target and invalidation and confidence when the setup is confirmed.
- Give no entry and no stop and no target when the decision is WAIT.
- Keep the whole answer short and plain and free of padding.
- Name the exact closed candle that confirmed or invalidated the setup.

## Available connectors

- Use `muse.connector_search` to find other connectors and `muse.skill_search` to find related skills.
- If nothing here fits, look on the web for a maintained API or MCP server and set it up with [Custom Connectors and MCPs](/opt/muse/skills/custom-connector-setup/SKILL.md), or build a custom connector.

## Websites

- Use [Inner Circle Trader YouTube](https://www.youtube.com/channel/UChlDYGqtnxuiSo4B2MwvOWw) for the free 2022 Mentorship with 41 episodes and the 2024 Mentorship.
- Use [The Inner Circle Trader](https://theinnercircletrader.com/) for the free library and core content.
- Use [Liquidity Sweeps](https://liquiditysweeps.com/) for free progressive ICT and SMC tutorials on sweeps and gaps and order blocks and kill zones.
- Use [ICT Archivist](https://ictarchivist.com/2022/) for dated summaries of the 2022 material in study order.
- Use [LIT Style Guide](https://otetmarkets.com/blog/articles/lit-style-forex/) for the public LIT inducement and internal versus external liquidity explanation.
- Use [TradeX Labs About](https://www.tradexlabs.io/about) for Cyzner background and quantified system principles.
- Open the user TradingView chart with `browser.browse` and read exact prices from closed candles only.
- Search results find sources and they never confirm a live price or a completed action.
