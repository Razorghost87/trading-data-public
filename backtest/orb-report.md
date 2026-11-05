# Job C — Opening-Range Breakout (stocks-in-play, 5m)

_OR = 09:30-09:35 bar. Enter first subsequent 5m close beyond OR, only when OR-bar vol ≥2.5× its 14-day avg. One trade/ticker/day. Costs: 1 tick + $1/100sh each side. ~40 trading days (Yahoo 5m limit). 32 instruments._

## Config matrix (stop × target)

| Stop/Target | n | Win% | ExpR | PF | MaxDD@2%% | MaxConsecL |
|---|---|---|---|---|---|---|
| atr10/eod | 64 | 14.06 | -0.205 | 0.786 | 49.29 | 15 |
| atr10/2R | 64 | 28.13 | -0.269 | 0.666 | 40.58 | 9 |
| oropp/eod | 64 | 59.38 | 0.165 | 1.643 | 4.74 | 3 |
| oropp/2R | 64 | 60.94 | 0.245 | 2.02 | 4.74 | 3 |

_Primary = atr10/eod. R vs stop distance; MaxDD@2% = equity curve risking 2%/trade, sequential (ignores concurrency)._

## Primary (atr10/eod) slices

### By instrument
| Slice | n | Win% | ExpR | PF |
|---|---|---|---|---|
| DASH | 3 | 66.67 | 2.965 | 9.489 |
| FISV | 3 | 33.33 | 2.555 | 4.09 |
| FLEX | 4 | 75 | 2.422 | 10.012 |
| UHS | 4 | 25 | 1.553 | 2.925 |
| FICO | 6 | 16.67 | 0.142 | 1.169 |
| MMM | 4 | 25 | -0.294 | 0.648 |
| DELL | 1 | 0 | -1.013 | 0 |
| REGN | 3 | 0 | -1.018 | 0 |
| DE | 1 | 0 | -1.021 | 0 |
| SNPS | 1 | 0 | -1.025 | 0 |
| IDXX | 3 | 0 | -1.029 | 0 |
| MRNA | 1 | 0 | -1.03 | 0 |
| HCA | 3 | 0 | -1.032 | 0 |
| VRT | 2 | 0 | -1.035 | 0 |
| QQQ | 1 | 0 | -1.042 | 0 |

### By day-of-week
| Slice | n | Win% | ExpR | PF |
|---|---|---|---|---|
| Wed | 17 | 17.65 | 0.031 | 1.035 |
| Thu | 16 | 12.5 | -0.06 | 0.938 |
| Tue | 12 | 16.67 | -0.145 | 0.854 |
| Fri | 11 | 9.09 | -0.501 | 0.517 |
| Mon | 8 | 12.5 | -0.684 | 0.283 |

### By SPY regime (close vs SMA20)
| Slice | n | Win% | ExpR | PF |
|---|---|---|---|---|
| ABOVE | 17 | 23.53 | 0.032 | 1.039 |
| BELOW | 47 | 10.64 | -0.291 | 0.713 |

## Example trades (primary config)

| Ticker | Date | Dir | OR hi/lo | Entry (time) | Exit | R |
|---|---|---|---|---|---|---|
| AMT | 2026-10-09 | long | 180.44/175.02 | 180.77 (11:25) | stop 11:30 | -1.107 |
| AMT | 2026-10-23 | short | 202.50/192.44 | 192.18 (09:55) | stop 10:00 | -1.085 |
| CCI | 2026-10-23 | short | 91.45/88.00 | 87.77 (09:50) | stop 09:55 | -1.148 |

_Resolutions: "next close beyond OR" = first subsequent 5m close past the OR boundary (first-breakout). Rel-vol = OR-bar volume vs its own 14-day average._
