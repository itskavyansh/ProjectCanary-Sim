# Shared Normal Runs (40 Runs) False Alarms Across Shape Evaluations (SYNTHETIC / SIMULATION)

> **SYNTHETIC / SIMULATION** — Model-mismatch stress test on synthetic mathematical surfaces; NOT field data and NOT validated on real data.

| shape | model | regime | FA eps / run (95% CI) | A: FA/h (slow, 24h/run) | A: every | B: FA/h (sensor, 0.0667h/run) | B: every |
|---|---|---|---|---|---|---|---|
| gaussian_control | threshold_rule | raw (k=1) | 6.525 [3.697, 9.988] | 0.2719 | 3.7 h | 97.88 | 0.6 min |
| gaussian_control | threshold_rule | episode_fa<=1 (k=3,m=3) | 0.450 [0.175, 0.800] | 0.0187 | 53.3 h | 6.75 | 8.9 min |
| gaussian_control | threshold_rule | strict_window_fa<=1 | 0.100 [0.000, 0.225] | 0.0042 | 240.0 h | 1.50 | 40.0 min |
| gaussian_control | logistic_regression | raw (k=1) | 21.075 [18.212, 24.279] | 0.8781 | 1.1 h | 316.12 | 0.2 min |
| gaussian_control | logistic_regression | episode_fa<=1 (k=3,m=3) | 0.350 [0.175, 0.550] | 0.0146 | 68.6 h | 5.25 | 11.4 min |
| gaussian_control | logistic_regression | strict_window_fa<=1 | 0.125 [0.000, 0.338] | 0.0052 | 192.0 h | 1.88 | 32.0 min |
| gaussian_control | random_forest | raw (k=1) | 7.100 [5.149, 9.263] | 0.2958 | 3.4 h | 106.50 | 0.6 min |
| gaussian_control | random_forest | episode_fa<=1 (k=3,m=3) | 0.450 [0.225, 0.700] | 0.0187 | 53.3 h | 6.75 | 8.9 min |
| gaussian_control | random_forest | strict_window_fa<=1 | 0.225 [0.100, 0.363] | 0.0094 | 106.7 h | 3.38 | 17.8 min |
| trough_panel | threshold_rule | raw (k=1) | 6.525 [3.697, 9.988] | 0.2719 | 3.7 h | 97.88 | 0.6 min |
| trough_panel | threshold_rule | episode_fa<=1 (k=3,m=3) | 0.450 [0.175, 0.800] | 0.0187 | 53.3 h | 6.75 | 8.9 min |
| trough_panel | threshold_rule | strict_window_fa<=1 | 0.100 [0.000, 0.225] | 0.0042 | 240.0 h | 1.50 | 40.0 min |
| trough_panel | logistic_regression | raw (k=1) | 21.075 [18.212, 24.279] | 0.8781 | 1.1 h | 316.12 | 0.2 min |
| trough_panel | logistic_regression | episode_fa<=1 (k=3,m=3) | 0.350 [0.175, 0.550] | 0.0146 | 68.6 h | 5.25 | 11.4 min |
| trough_panel | logistic_regression | strict_window_fa<=1 | 0.125 [0.000, 0.338] | 0.0052 | 192.0 h | 1.88 | 32.0 min |
| trough_panel | random_forest | raw (k=1) | 7.100 [5.149, 9.263] | 0.2958 | 3.4 h | 106.50 | 0.6 min |
| trough_panel | random_forest | episode_fa<=1 (k=3,m=3) | 0.450 [0.225, 0.700] | 0.0187 | 53.3 h | 6.75 | 8.9 min |
| trough_panel | random_forest | strict_window_fa<=1 | 0.225 [0.100, 0.363] | 0.0094 | 106.7 h | 3.38 | 17.8 min |
| asymmetric | threshold_rule | raw (k=1) | 6.525 [3.697, 9.988] | 0.2719 | 3.7 h | 97.88 | 0.6 min |
| asymmetric | threshold_rule | episode_fa<=1 (k=3,m=3) | 0.450 [0.175, 0.800] | 0.0187 | 53.3 h | 6.75 | 8.9 min |
| asymmetric | threshold_rule | strict_window_fa<=1 | 0.100 [0.000, 0.225] | 0.0042 | 240.0 h | 1.50 | 40.0 min |
| asymmetric | logistic_regression | raw (k=1) | 21.075 [18.212, 24.279] | 0.8781 | 1.1 h | 316.12 | 0.2 min |
| asymmetric | logistic_regression | episode_fa<=1 (k=3,m=3) | 0.350 [0.175, 0.550] | 0.0146 | 68.6 h | 5.25 | 11.4 min |
| asymmetric | logistic_regression | strict_window_fa<=1 | 0.125 [0.000, 0.338] | 0.0052 | 192.0 h | 1.88 | 32.0 min |
| asymmetric | random_forest | raw (k=1) | 7.100 [5.149, 9.263] | 0.2958 | 3.4 h | 106.50 | 0.6 min |
| asymmetric | random_forest | episode_fa<=1 (k=3,m=3) | 0.450 [0.225, 0.700] | 0.0187 | 53.3 h | 6.75 | 8.9 min |
| asymmetric | random_forest | strict_window_fa<=1 | 0.225 [0.100, 0.363] | 0.0094 | 106.7 h | 3.38 | 17.8 min |
| two_basin | threshold_rule | raw (k=1) | 6.525 [3.697, 9.988] | 0.2719 | 3.7 h | 97.88 | 0.6 min |
| two_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | 0.450 [0.175, 0.800] | 0.0187 | 53.3 h | 6.75 | 8.9 min |
| two_basin | threshold_rule | strict_window_fa<=1 | 0.100 [0.000, 0.225] | 0.0042 | 240.0 h | 1.50 | 40.0 min |
| two_basin | logistic_regression | raw (k=1) | 21.075 [18.212, 24.279] | 0.8781 | 1.1 h | 316.12 | 0.2 min |
| two_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | 0.350 [0.175, 0.550] | 0.0146 | 68.6 h | 5.25 | 11.4 min |
| two_basin | logistic_regression | strict_window_fa<=1 | 0.125 [0.000, 0.338] | 0.0052 | 192.0 h | 1.88 | 32.0 min |
| two_basin | random_forest | raw (k=1) | 7.100 [5.149, 9.263] | 0.2958 | 3.4 h | 106.50 | 0.6 min |
| two_basin | random_forest | episode_fa<=1 (k=3,m=3) | 0.450 [0.225, 0.700] | 0.0187 | 53.3 h | 6.75 | 8.9 min |
| two_basin | random_forest | strict_window_fa<=1 | 0.225 [0.100, 0.363] | 0.0094 | 106.7 h | 3.38 | 17.8 min |
| planar_slope | threshold_rule | raw (k=1) | 6.525 [3.697, 9.988] | 0.2719 | 3.7 h | 97.88 | 0.6 min |
| planar_slope | threshold_rule | episode_fa<=1 (k=3,m=3) | 0.450 [0.175, 0.800] | 0.0187 | 53.3 h | 6.75 | 8.9 min |
| planar_slope | threshold_rule | strict_window_fa<=1 | 0.100 [0.000, 0.225] | 0.0042 | 240.0 h | 1.50 | 40.0 min |
| planar_slope | logistic_regression | raw (k=1) | 21.075 [18.212, 24.279] | 0.8781 | 1.1 h | 316.12 | 0.2 min |
| planar_slope | logistic_regression | episode_fa<=1 (k=3,m=3) | 0.350 [0.175, 0.550] | 0.0146 | 68.6 h | 5.25 | 11.4 min |
| planar_slope | logistic_regression | strict_window_fa<=1 | 0.125 [0.000, 0.338] | 0.0052 | 192.0 h | 1.88 | 32.0 min |
| planar_slope | random_forest | raw (k=1) | 7.100 [5.149, 9.263] | 0.2958 | 3.4 h | 106.50 | 0.6 min |
| planar_slope | random_forest | episode_fa<=1 (k=3,m=3) | 0.450 [0.225, 0.700] | 0.0187 | 53.3 h | 6.75 | 8.9 min |
| planar_slope | random_forest | strict_window_fa<=1 | 0.225 [0.100, 0.363] | 0.0094 | 106.7 h | 3.38 | 17.8 min |
