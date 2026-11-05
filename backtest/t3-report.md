# Job A — T3 Event-Day Entry Timing (risk metrics)

_Event: gap ≥5% + vol ≥2.5× av50 + close top-40% of range. Hold 20, stop −7%. Full cache history (518 tickers). R = return ÷ 7% risk._

**336 events** across 214 tickers.

## Per-variant

| Arm | n | Win% | AvgRet% | Exp R | PF | AvgDays | MaxDD@2%% | MaxConsecL | WorstMonth |
|---|---|---|---|---|---|---|---|---|---|
| day-0 close | 336 | 43.45 | 1.09 | 0.156 | 1.326 | 14.2 | 33.66 | 11 | 2026-02 (-21.65%) |
| day-2 close | 336 | 46.73 | 1.74 | 0.249 | 1.559 | 15 | 31.26 | 10 | 2026-06 (-18.78%) |

## Expectancy by posture (SPY vs SMA50 on event day)

### day-0
| Slice | n | Win% | Exp R | AvgRet% |
|---|---|---|---|---|
| BELOW | 53 | 50.94 | 0.342 | 2.39 |
| ABOVE | 283 | 42.05 | 0.121 | 0.85 |

### day-2
| Slice | n | Win% | Exp R | AvgRet% |
|---|---|---|---|---|
| BELOW | 53 | 54.72 | 0.426 | 2.98 |
| ABOVE | 283 | 45.23 | 0.216 | 1.51 |

## Expectancy by cap bucket

### day-0
| Slice | n | Win% | Exp R | AvgRet% |
|---|---|---|---|---|
| mega (>200B) | 45 | 53.33 | 0.415 | 2.9 |
| large (10-200B) | 271 | 42.8 | 0.161 | 1.13 |
| UNKNOWN | 1 | 100 | 0.052 | 0.36 |
| mid (2-10B) | 16 | 31.25 | -0.437 | -3.06 |
| small (<2B) | 3 | 0 | -1 | -7 |

### day-2
| Slice | n | Win% | Exp R | AvgRet% |
|---|---|---|---|---|
| mega (>200B) | 45 | 60 | 0.479 | 3.35 |
| large (10-200B) | 271 | 46.49 | 0.262 | 1.83 |
| UNKNOWN | 1 | 0 | -0.023 | -0.16 |
| mid (2-10B) | 16 | 25 | -0.366 | -2.56 |
| small (<2B) | 3 | 0 | -1 | -7 |

_MaxDD@2% = max drawdown of equity curve risking 2% per trade, sequential by entry date (ignores concurrency). Stop differs from the Aug run's −8%; arms reduced to the two that carried the edge._
