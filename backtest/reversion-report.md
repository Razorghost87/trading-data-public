# Job B — Flush / Mean-Reversion Entry Science

_Flush: (prevClose−low)/ATR14 ≥2 OR (high5−low)/ATR14 ≥3.5; vol ≥2.5×av50; bottom-40% close OR next-day reclaim; price ≥$5. Stop = flush_low − 0.5 ATR. R vs that stop. Full cache history._

**1697 flush events** detected across the universe.

## Master table — 9 entry×exit combos

| Entry×Exit | n | Win% | AvgWinR | AvgLossR | ExpR | PF | AvgDays |
|---|---|---|---|---|---|---|---|
| E0_X3 | 1645 | 34.65 | 2.631 | -0.963 | 0.283 | 1.449 | 10.7 |
| E0_X2 | 1645 | 54.35 | 1.168 | -0.954 | 0.199 | 1.458 | 2.7 |
| E0_X1 | 1656 | 46.07 | 1.419 | -0.917 | 0.159 | 1.321 | 3.6 |
| E2_X3 | 1397 | 40.87 | 1.588 | -0.883 | 0.127 | 1.243 | 13.6 |
| E1_X3 | 585 | 53.5 | 0.819 | -0.761 | 0.084 | 1.239 | 17.2 |
| E2_X2 | 1397 | 54.76 | 0.519 | -0.524 | 0.047 | 1.2 | 1.8 |
| E2_X1 | 1405 | 46.12 | 0.887 | -0.692 | 0.036 | 1.098 | 3.9 |
| E1_X2 | 585 | 52.31 | 0.225 | -0.278 | -0.015 | 0.889 | 1.7 |
| E1_X1 | 591 | 35.87 | 0.356 | -0.407 | -0.134 | 0.489 | 3.1 |

_E0 catch · E1 reclaim (close>flush high ≤5d) · E2 RSI2>30 turn ≤5d. X1 retrace-50% (t10) · X2 close>SMA5 (t20) · X3 hold-20._

## Slice tables — best 2 combos (E0_X3, E0_X2)

### E0_X3

**trend_200**
| Slice | n | Win% | ExpR | PF |
|---|---|---|---|---|
| SHORT | 391 | 42.2 | 0.472 | 1.843 |
| ABOVE | 406 | 33.5 | 0.324 | 1.52 |
| BELOW | 848 | 31.72 | 0.176 | 1.265 |

**event_type**
| Slice | n | Win% | ExpR | PF |
|---|---|---|---|---|
| EARNINGS_PROXY | 256 | 39.84 | 0.445 | 1.769 |
| NON_EVENT | 1389 | 33.69 | 0.253 | 1.396 |

**drop_atr_bucket**
| Slice | n | Win% | ExpR | PF |
|---|---|---|---|---|
| >6 | 151 | 39.74 | 0.349 | 1.589 |
| 3-4 | 542 | 33.39 | 0.301 | 1.475 |
| 4-6 | 815 | 35.21 | 0.28 | 1.448 |
| 2-3 | 137 | 30.66 | 0.152 | 1.225 |

**vol_bucket**
| Slice | n | Win% | ExpR | PF |
|---|---|---|---|---|
| >8 | 66 | 45.45 | 0.582 | 2.107 |
| 2.5-4 | 1184 | 33.95 | 0.283 | 1.445 |
| 4-8 | 395 | 34.94 | 0.232 | 1.37 |

**rsi14_bucket**
| Slice | n | Win% | ExpR | PF |
|---|---|---|---|---|
| <25 | 371 | 36.93 | 0.472 | 1.762 |
| >35 | 660 | 36.21 | 0.278 | 1.462 |
| 25-35 | 614 | 31.6 | 0.174 | 1.261 |

**mkt_regime**
| Slice | n | Win% | ExpR | PF |
|---|---|---|---|---|
| BELOW | 424 | 33.73 | 0.32 | 1.503 |
| ABOVE | 1175 | 34.89 | 0.281 | 1.447 |
| UNKNOWN | 46 | 36.96 | -0.009 | 0.984 |

**sector_sympathy**
| Slice | n | Win% | ExpR | PF |
|---|---|---|---|---|
| NONE | 1209 | 34.82 | 0.325 | 1.521 |
| SYMPATHY | 436 | 34.17 | 0.166 | 1.258 |

### E0_X2

**trend_200**
| Slice | n | Win% | ExpR | PF |
|---|---|---|---|---|
| SHORT | 391 | 60.61 | 0.311 | 1.838 |
| ABOVE | 406 | 59.61 | 0.305 | 1.793 |
| BELOW | 848 | 48.94 | 0.097 | 1.198 |

**event_type**
| Slice | n | Win% | ExpR | PF |
|---|---|---|---|---|
| EARNINGS_PROXY | 256 | 58.98 | 0.287 | 1.725 |
| NON_EVENT | 1389 | 53.49 | 0.183 | 1.414 |

**drop_atr_bucket**
| Slice | n | Win% | ExpR | PF |
|---|---|---|---|---|
| 4-6 | 815 | 55.58 | 0.243 | 1.582 |
| >6 | 151 | 52.32 | 0.192 | 1.419 |
| 3-4 | 542 | 54.43 | 0.177 | 1.403 |
| 2-3 | 137 | 48.91 | 0.032 | 1.065 |

**vol_bucket**
| Slice | n | Win% | ExpR | PF |
|---|---|---|---|---|
| >8 | 66 | 60.61 | 0.376 | 2.062 |
| 4-8 | 395 | 56.71 | 0.206 | 1.492 |
| 2.5-4 | 1184 | 53.21 | 0.187 | 1.42 |

**rsi14_bucket**
| Slice | n | Win% | ExpR | PF |
|---|---|---|---|---|
| >35 | 660 | 60.45 | 0.28 | 1.741 |
| <25 | 371 | 52.56 | 0.263 | 1.571 |
| 25-35 | 614 | 48.86 | 0.074 | 1.154 |

**mkt_regime**
| Slice | n | Win% | ExpR | PF |
|---|---|---|---|---|
| BELOW | 424 | 55.66 | 0.288 | 1.667 |
| ABOVE | 1175 | 53.79 | 0.174 | 1.397 |
| UNKNOWN | 46 | 56.52 | 0.022 | 1.055 |

**sector_sympathy**
| Slice | n | Win% | ExpR | PF |
|---|---|---|---|---|
| NONE | 1209 | 55.58 | 0.204 | 1.485 |
| SYMPATHY | 436 | 50.92 | 0.185 | 1.39 |

## Kill list (slice n≥15 AND expectancy ≤0 → hard gate)

_None._

## Stacked conditions (ABOVE200 + {NON_EVENT|SYMPATHY} + vol≥4× + rsi14<30)

| Combo | n | Win% | ExpR | PF |
|---|---|---|---|---|
| E0_X3 | 2 | 50 | -0.427 | 0.147 |
| E0_X2 | 2 | 100 | 0.944 | 99 |

## Sanity cases

| Case | Detected (±6d) | flush date | drop_atr | vol× | close%rng | why not? | trend_200 | event_type | E1 entry | X3 R |
|---|---|---|---|---|---|---|---|---|---|---|
| SPCX 2026-08-06 | ❌ | — | 0.288 | 2.24 | 92.2 | dS0.288/dM1.965 vol2.24× close@92.2% → fails drop<thr+vol<2.5 | — | — | — | — |
| BSX 2026-10-28 | ❌ | — | 3.646 | 3.733 | 65.75 | dS3.646/dM4.377 vol3.733× close@65.75% → fails close-gate | — | — | — | — |
| GOOG 2026-10-29 | ❌ | — | 4.165 | 5.538 | 49.51 | dS4.165/dM4.284 vol5.538× close@49.51% → fails close-gate | — | — | — | — |
| ON 2026-06-30 | ✅ | 2026-06-26 | 4.274 | 3.477 | — | — | ABOVE | NON_EVENT | none ≤5d | -1* |

_*E0_X3 shown when no E1 entry. ❌ rows show the exact-date diagnosis: the spec's "bottom-40% OR next-day reclaim" gate excludes gap-down (GOOG) and hammer (BSX) flushes, and SPCX's ~10%/day ATR makes −13.6% only ~1.7 ATR. Detector left frozen per no-tuning rule — gate relaxation listed as a follow-up. Market-breadth regime unavailable (no macro.json history); mkt_regime = SPY vs SMA50 only._
