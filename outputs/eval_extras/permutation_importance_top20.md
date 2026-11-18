# Top 20 Permutation Feature Importance (Random Forest on VAL Only; Grouped by Run)

> **Methodology:** Permutations are executed across whole runs (preserving temporal autocorrelation within runs) on the **VAL split only**. Repeats = 5. Importance metric = drop in Window Macro-F1.

| Rank | Feature | Feature Group | Mean Macro-F1 Drop | Std (Spread) | Min | Max |
|---|---|---|---|---|---|---|
| 1 | `comm_missing_frac_net` | comm | **0.03560** | 0.00550 | 0.03010 | 0.04347 |
| 2 | `comm_max_burst_len` | comm | **0.03500** | 0.00680 | 0.02922 | 0.04611 |
| 3 | `comm_latency_mean_s` | comm | **0.02354** | 0.00471 | 0.01661 | 0.02968 |
| 4 | `NODE_03_mean` | magnitude | **0.02299** | 0.00202 | 0.02025 | 0.02524 |
| 5 | `comm_latency_max_s` | comm | **0.02205** | 0.00297 | 0.01921 | 0.02635 |
| 6 | `long_slope_max_deg_s` | long_horizon | **0.01850** | 0.00427 | 0.01194 | 0.02296 |
| 7 | `NODE_01_std` | magnitude | **0.01056** | 0.00763 | -0.00250 | 0.01592 |
| 8 | `NODE_04_mean` | magnitude | **0.01010** | 0.00242 | 0.00741 | 0.01391 |
| 9 | `NODE_03_std` | magnitude | **0.00829** | 0.00370 | 0.00377 | 0.01244 |
| 10 | `dir_convergence_residual_m` | direction | **0.00780** | 0.00347 | 0.00212 | 0.01120 |
| 11 | `NODE_04_missing_frac` | comm | **0.00694** | 0.00134 | 0.00551 | 0.00897 |
| 12 | `dir_convergence_align_cos` | direction | **0.00646** | 0.00705 | -0.00034 | 0.01460 |
| 13 | `NODE_02_mean` | magnitude | **0.00607** | 0.00444 | -0.00136 | 0.00977 |
| 14 | `NODE_04_std` | magnitude | **0.00542** | 0.00541 | -0.00175 | 0.01123 |
| 15 | `dir_convergence_weighted_cos` | direction | **0.00536** | 0.00235 | 0.00268 | 0.00864 |
| 16 | `NODE_04_tilt_angle_rad` | direction | **0.00496** | 0.00326 | 0.00007 | 0.00838 |
| 17 | `hub_common_mode_m` | hub | **0.00411** | 0.00330 | -0.00066 | 0.00762 |
| 18 | `NODE_03_long_slope_deg_s` | long_horizon | **0.00255** | 0.00109 | 0.00155 | 0.00439 |
| 19 | `NODE_04_long_slope_deg_s` | long_horizon | **0.00207** | 0.00113 | 0.00062 | 0.00370 |
| 20 | `NODE_01_long_slope_deg_s` | long_horizon | **0.00195** | 0.00050 | 0.00120 | 0.00234 |
