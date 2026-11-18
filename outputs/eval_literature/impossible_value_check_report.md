# Impossible-Value Check Audit on B1 & B2 Arms (SYNTHETIC / SIMULATION)

> **SYNTHETIC / SIMULATION** — Literature-basis sensitivity checks on frozen v3 models; nothing here is validated on real data.

| arm | runs | windows | max window node tilt (deg) | runs > 15 deg limit | runs >= 3.5 deg (ThresholdRule implausible) | validation_checks.check_impossible messages |
|---|---:|---:|---:|---:|---:|---|
| `gaussian_control` | 60 | 5700 | **3.085** | **0** (0 win) | **0** (0 win) | NONE |
| `high_tilt_3_6` | 60 | 5700 | **6.025** | **0** (0 win) | **30** (1420 win) | basin peak_tilt_deg outside configured [0.05, 3.0] deg |
| `high_tilt_6_12` | 60 | 5700 | **10.696** | **0** (0 win) | **60** (3034 win) | basin peak_tilt_deg outside configured [0.05, 3.0] deg |
| `depth_all_gt_1p5` | 140 | 13300 | **3.201** | **0** (0 win) | **0** (0 win) | NONE |
| `H100_tanB1p5` | 20 | 1900 | **3.201** | **0** (0 win) | **0** (0 win) | NONE |
| `H200_tanB1p5` | 20 | 1900 | **2.324** | **0** (0 win) | **0** (0 win) | NONE |
| `H200_tanB2p0` | 20 | 1900 | **2.636** | **0** (0 win) | **0** (0 win) | NONE |
| `H200_tanB2p5` | 20 | 1900 | **3.110** | **0** (0 win) | **0** (0 win) | NONE |
| `H300_tanB1p5` | 20 | 1900 | **2.452** | **0** (0 win) | **0** (0 win) | NONE |
| `H300_tanB2p0` | 20 | 1900 | **2.180** | **0** (0 win) | **0** (0 win) | NONE |
| `H300_tanB2p5` | 20 | 1900 | **1.852** | **0** (0 win) | **0** (0 win) | NONE |
