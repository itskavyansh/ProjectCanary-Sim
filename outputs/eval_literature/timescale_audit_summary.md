# Part C: Timescale Audit of Frozen Gradual Runs (SYNTHETIC / SIMULATION)

> **SYNTHETIC / SIMULATION** — Literature-basis sensitivity checks on frozen v3 models; nothing here is validated on real data.

> **Reference Notice:** Real-world comparison value `0.1 deg/day` (from ~`60 mm/m` [`3.4 deg`] over ~`30 days`) is **DERIVED, ORDER OF MAGNITUDE**, not a cited value.

| subset | gradual runs | faster than 0.1 deg/day (share) | implied deg/day at 360x: min / p10 / **p50** / mean / p90 / max | speedup factor vs 0.1 deg/day: min / **p50** / mean / p90 / max |
|---|---:|---|---|---|
| `ALL_GRADUAL_RUNS` | 165 | **161 / 165** (97.6%) | 0.087 / 0.150 / **0.763** / 1.547 / 4.495 / 6.597 | 0.87x / **7.63x** / 15.47x / 44.95x / 65.97x |
| `split:train` | 60 | **59 / 60** (98.3%) | 0.087 / 0.173 / **0.760** / 1.474 / 4.270 / 5.955 | 0.87x / **7.60x** / 14.74x / 42.70x / 59.55x |
| `split:val` | 20 | **20 / 20** (100.0%) | 0.118 / 0.148 / **0.870** / 1.459 / 3.501 / 6.002 | 1.18x / **8.70x** / 14.59x / 35.01x / 60.02x |
| `split:test` | 20 | **19 / 20** (95.0%) | 0.100 / 0.175 / **0.686** / 1.422 / 3.544 / 5.636 | 1.00x / **6.86x** / 14.22x / 35.44x / 56.37x |
| `split:shifted_test` | 15 | **14 / 15** (93.3%) | 0.088 / 0.160 / **0.714** / 1.555 / 3.880 / 6.597 | 0.88x / **7.14x** / 15.55x / 38.80x / 65.97x |
| `split:broad_basin` | 20 | **20 / 20** (100.0%) | 0.106 / 0.134 / **0.680** / 1.586 / 4.189 / 6.457 | 1.06x / **6.80x** / 15.86x / 41.89x / 64.57x |
| `split:stress` | 30 | **29 / 30** (96.7%) | 0.093 / 0.126 / **1.033** / 1.803 / 4.736 / 5.482 | 0.93x / **10.33x** / 18.03x / 47.36x / 54.82x |
