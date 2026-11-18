# Radial Convergence Feature Distributions Across B1 & B2 Arms (SYNTHETIC / SIMULATION)

> **SYNTHETIC / SIMULATION** — Literature-basis sensitivity checks on frozen v3 models; nothing here is validated on real data.

| arm | subset | windows | residual_m p10 / **p50** / p90 (mean) | weighted_cos p10 / **p50** / p90 (mean) | pairwise_cos p50 |
|---|---|---:|---|---|---:|
| `gaussian_control` | active_windows_all_snr | 3824 | 1.57 / **6.88** / 17.28 (8.56) | -0.796 / **0.722** / 0.994 (0.378) | -0.065 |
| `gaussian_control` | active_windows_snr_gt_2 | 1819 | 1.07 / **3.23** / 11.55 (5.27) | -0.427 / **0.952** / 0.998 (0.623) | -0.065 |
| `high_tilt_3_6` | active_windows_all_snr | 3916 | 0.63 / **2.80** / 11.22 (4.39) | -0.672 / **0.976** / 1.000 (0.582) | -0.005 |
| `high_tilt_3_6` | active_windows_snr_gt_2 | 3916 | 0.63 / **2.80** / 11.22 (4.39) | -0.672 / **0.976** / 1.000 (0.582) | -0.005 |
| `high_tilt_6_12` | active_windows_all_snr | 3898 | 0.31 / **1.74** / 7.20 (3.11) | -0.484 / **0.993** / 1.000 (0.734) | 0.285 |
| `high_tilt_6_12` | active_windows_snr_gt_2 | 3898 | 0.31 / **1.74** / 7.20 (3.11) | -0.484 / **0.993** / 1.000 (0.734) | 0.285 |
| `depth_all_gt_1p5` | active_windows_all_snr | 9026 | 0.42 / **4.06** / 13.71 (5.95) | -0.277 / **0.943** / 1.000 (0.639) | 0.116 |
| `depth_all_gt_1p5` | active_windows_snr_gt_2 | 4436 | 0.25 / **1.20** / 8.37 (2.92) | 0.485 / **0.996** / 1.000 (0.856) | 0.286 |
| `H100_tanB1p5` | active_windows_all_snr | 1319 | 0.28 / **3.26** / 13.19 (5.43) | -0.045 / **0.972** / 1.000 (0.727) | 0.116 |
| `H100_tanB1p5` | active_windows_snr_gt_2 | 681 | 0.18 / **1.15** / 9.94 (3.12) | 0.359 / **0.995** / 1.000 (0.854) | -0.007 |
| `H200_tanB1p5` | active_windows_all_snr | 1319 | 0.56 / **4.18** / 12.70 (5.52) | -0.151 / **0.922** / 0.999 (0.662) | 0.184 |
| `H200_tanB1p5` | active_windows_snr_gt_2 | 590 | 0.33 / **1.18** / 7.52 (2.88) | 0.386 / **0.993** / 0.999 (0.827) | 0.497 |
| `H200_tanB2p0` | active_windows_all_snr | 1232 | 0.44 / **4.06** / 13.32 (5.72) | -0.284 / **0.868** / 1.000 (0.597) | 0.103 |
| `H200_tanB2p0` | active_windows_snr_gt_2 | 654 | 0.30 / **1.26** / 5.76 (2.54) | 0.591 / **0.995** / 1.000 (0.853) | 0.236 |
| `H200_tanB2p5` | active_windows_all_snr | 1338 | 0.46 / **2.89** / 13.37 (5.16) | -0.247 / **0.960** / 1.000 (0.701) | 0.180 |
| `H200_tanB2p5` | active_windows_snr_gt_2 | 762 | 0.35 / **1.09** / 7.27 (2.90) | 0.537 / **0.996** / 1.000 (0.851) | 0.445 |
| `H300_tanB1p5` | active_windows_all_snr | 1332 | 0.48 / **5.54** / 16.96 (7.29) | -0.444 / **0.834** / 1.000 (0.525) | 0.037 |
| `H300_tanB1p5` | active_windows_snr_gt_2 | 640 | 0.25 / **1.08** / 8.44 (3.01) | 0.599 / **0.997** / 1.000 (0.859) | 0.373 |
| `H300_tanB2p0` | active_windows_all_snr | 1257 | 0.35 / **5.60** / 14.62 (7.01) | -0.446 / **0.829** / 0.999 (0.516) | 0.045 |
| `H300_tanB2p0` | active_windows_snr_gt_2 | 597 | 0.20 / **1.36** / 9.15 (3.23) | 0.505 / **0.995** / 1.000 (0.857) | 0.139 |
| `H300_tanB2p5` | active_windows_all_snr | 1229 | 0.50 / **3.80** / 12.42 (5.55) | -0.022 / **0.961** / 1.000 (0.741) | 0.122 |
| `H300_tanB2p5` | active_windows_snr_gt_2 | 512 | 0.25 / **1.07** / 7.89 (2.70) | 0.717 / **0.998** / 1.000 (0.904) | 0.209 |
