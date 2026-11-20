# MTF checklist - XAUUSD M1

Source notes, paraphrased in own words, no copyrighted text copied:
- ~/workspace/research_notes/ict-michael/ict-michael-notes.md
- ~/workspace/research_notes/lit-reimfx/lit-notes.md
- ~/workspace/research_notes/cyzner/cyzner-notes.md

## Pre-session lock - once per kill zone

- H4 bias: bullish / bearish / neutral, from H4 structure + nearest external liquidity draw
- H1 key levels: PDH / PDL, prior day high / low, session high / low, Asia high / low
- M15 dealing range: high, low, 50% equilibrium, premium above, discount below
- Midnight open 00:00 ET: price above = expensive, below = cheap
- Kill zone active? London 11:30-14:30 Tehran, New York 16:30-19:30 Tehran, winter
- News filter: no red-folder US data within 30 min
- Written If-Then plan, one line: If London sweeps X and M1 MSS up, then long at FVG, SL behind MSS, TP1 next pool. If no sweep, WAIT.

## Kill zones - Tehran winter

London Open 10:30-13:30, Silver Bullet London 11:30-12:30
New York AM 17:00-19:30, Silver Bullet NY AM 18:30-19:30
London Close 18:30-20:30
New York PM 22:00-00:30

Ali monitor windows, slightly wider, govern live checks: London 11:30-14:30, New York 16:30-19:30 Tehran, Mon-Fri.

Summer EDT: subtract 1 hour from winter Tehran times. US DST changes first Sun Nov to second Sun Mar.

## In-session - M15 to M1

- Sweep: wick beyond named pool (BSL/SSL, PDH/PDL, equal H/L, Asia/London H/L) against bias, then close back inside
- Inducement: first pullback / minor swing / equal high-low between price and POI - was it swept?
- Trap vs run: body close back inside + displacement opposite = trap, tradeable. Body close through + hold = run, do not fade
- Displacement: full-bodied M1/M5 candles, decisive close through last opposing swing, leaves FVG
- MSS: 1m close beyond swing formed at/after sweep
- PD array: FVG/OB from displacement leg only, top/bottom/CE, in discount for long / premium for short
- OTE: M15 61.8-78.6%, ideal 70.5%, overlap with FVG/OB is a bonus
- SMT: XAGUSD and/or DXY non-confirmation on M5-M15 is +1, never a required delay
- MSNR: fresh level only, body-based, single price

## Entry and exit - M1

- Entry: tap / retest at FVG CE, only after pullback, never chase displacement candle
- SL: behind M1 MSS swing, 2.5-5$ max, never behind H1/M15 level
- TP1 = 2x SL, TP2 = next liquidity pool (PDH/PDL, session H/L)
- RR >= 1:2 or no trade
- Invalidation: 1m close beyond MSS swing / beyond sweep extreme wrong way
- One trade per kill zone, partial at TP1, runner to TP2, 2 losses = stop day

## Scoring

Start 0. +2 sweep of ERL, +1 inducement swept, +1 fresh MSNR POI, +1 displacement + MSS closed, +1 FVG retest held, +1 SMT non-confirmation, +1 OTE overlap.
-2 entry is inducement, -2 body-close break-and-hold, -2 outside kill zone.
Require >=60/100. Log inducement_swept, irl_or_erl, smt per check.

## Worked example - locked levels 2026-11-06 post-NFP

BSL / day high 4107.085, SSL / day low 4030.11, support below 4018.055, resistance 4039.66 and 4065.17, OB 4056-4064, bearish FVGs 4077-4082 and 4085.46.
Price ~4037 at 18:05 Tehran, whipsawing 4030-4041, bias bearish H4/H1/M15.
No fresh sweep + displacement + MSS + FVG in kill zone, price mid-range below OB, no M1 confirmation.
Decision by skill: WAIT, confidence 70/100 for WAIT, no entry/SL/TP.
Long re-opens only after M1 close above 4075 + bullish MSS, short only on M1 close below 4064 with displacement toward 4039/4035.775.
This example is a test case, not a live signal. Verify live price before any use.

## What NOT to do

- Do not trade sweep alone, do not chase displacement candle, do not buy premium / sell discount
- Do not use H1/M15 level as M1 stop, the $10-stop error Ali corrected 2026-11-06
- Do not trade mid-range, outside kill zones, news headline, or after a loss in same kill zone
- Do not copy win-rate claims: no audited ICT track record, no LIT backtest on XAUUSD M1 found, Cyzner ORB/PIVOTS are NQ-focused, vendor claims not audited
- Do not import NQ ORB parameters or unpublished PIVOTS formula to gold
