# Gradual & Rapid Window Recall and Run Detection by SNR Bin (SYNTHETIC / SIMULATION)

> **SYNTHETIC / SIMULATION** — Model-mismatch stress test on synthetic mathematical surfaces; NOT field data and NOT validated on real data.

| shape | model | regime | class | SNR bin | runs | windows | window recall (95% CI) | run detect rate (95% CI) |
|---|---|---|---|---|---|---|---|---|
| gaussian_control | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | ALL | 30 | 2008 | 0.188 [0.121, 0.260] | 0.500 [0.367, 0.667] |
| gaussian_control | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.124 [0.053, 0.212] | 0.400 [0.100, 0.600] |
| gaussian_control | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 339 | 0.012 [0.000, 0.034] | 0.000 [0.000, 0.000] |
| gaussian_control | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 387 | 0.129 [0.020, 0.251] | 0.667 [0.333, 1.000] |
| gaussian_control | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 614 | 0.391 [0.258, 0.517] | 0.778 [0.444, 1.000] |
| gaussian_control | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | ALL | 30 | 1816 | 0.276 [0.168, 0.385] | 0.467 [0.282, 0.633] |
| gaussian_control | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | <1 | 9 | 556 | 0.059 [0.000, 0.160] | 0.111 [0.000, 0.333] |
| gaussian_control | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 8 | 442 | 0.176 [0.048, 0.321] | 0.500 [0.125, 0.875] |
| gaussian_control | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 218 | 0.188 [0.009, 0.527] | 0.250 [0.000, 0.750] |
| gaussian_control | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | >5 | 9 | 600 | 0.583 [0.407, 0.719] | 0.889 [0.667, 1.000] |
| gaussian_control | threshold_rule | strict_window_fa<=1 | gradual | ALL | 30 | 2008 | 0.188 [0.121, 0.260] | 0.233 [0.100, 0.384] |
| gaussian_control | threshold_rule | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.124 [0.053, 0.212] | 0.000 [0.000, 0.000] |
| gaussian_control | threshold_rule | strict_window_fa<=1 | gradual | 1-2 | 5 | 339 | 0.012 [0.000, 0.034] | 0.000 [0.000, 0.000] |
| gaussian_control | threshold_rule | strict_window_fa<=1 | gradual | 2-5 | 6 | 387 | 0.129 [0.020, 0.251] | 0.000 [0.000, 0.000] |
| gaussian_control | threshold_rule | strict_window_fa<=1 | gradual | >5 | 9 | 614 | 0.391 [0.258, 0.517] | 0.778 [0.444, 1.000] |
| gaussian_control | threshold_rule | strict_window_fa<=1 | rapid | ALL | 30 | 1816 | 0.276 [0.168, 0.385] | 0.333 [0.167, 0.500] |
| gaussian_control | threshold_rule | strict_window_fa<=1 | rapid | <1 | 9 | 556 | 0.059 [0.000, 0.160] | 0.111 [0.000, 0.333] |
| gaussian_control | threshold_rule | strict_window_fa<=1 | rapid | 1-2 | 8 | 442 | 0.176 [0.048, 0.321] | 0.250 [0.000, 0.625] |
| gaussian_control | threshold_rule | strict_window_fa<=1 | rapid | 2-5 | 4 | 218 | 0.188 [0.009, 0.527] | 0.250 [0.000, 0.750] |
| gaussian_control | threshold_rule | strict_window_fa<=1 | rapid | >5 | 9 | 600 | 0.583 [0.407, 0.719] | 0.667 [0.333, 1.000] |
| gaussian_control | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | ALL | 30 | 2008 | 0.175 [0.105, 0.258] | 0.400 [0.233, 0.600] |
| gaussian_control | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.076 [0.021, 0.161] | 0.300 [0.100, 0.600] |
| gaussian_control | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 339 | 0.003 [0.000, 0.008] | 0.000 [0.000, 0.000] |
| gaussian_control | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 387 | 0.158 [0.000, 0.345] | 0.333 [0.000, 0.667] |
| gaussian_control | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 614 | 0.388 [0.240, 0.545] | 0.778 [0.444, 1.000] |
| gaussian_control | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | ALL | 30 | 1816 | 0.346 [0.214, 0.482] | 0.533 [0.333, 0.733] |
| gaussian_control | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | <1 | 9 | 556 | 0.049 [0.003, 0.100] | 0.222 [0.000, 0.556] |
| gaussian_control | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 8 | 442 | 0.145 [0.021, 0.271] | 0.375 [0.059, 0.750] |
| gaussian_control | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 218 | 0.298 [0.037, 0.671] | 0.500 [0.000, 1.000] |
| gaussian_control | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | >5 | 9 | 600 | 0.788 [0.596, 0.938] | 1.000 [1.000, 1.000] |
| gaussian_control | logistic_regression | strict_window_fa<=1 | gradual | ALL | 30 | 2008 | 0.067 [0.027, 0.117] | 0.233 [0.100, 0.400] |
| gaussian_control | logistic_regression | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.013 [0.000, 0.032] | 0.000 [0.000, 0.000] |
| gaussian_control | logistic_regression | strict_window_fa<=1 | gradual | 1-2 | 5 | 339 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| gaussian_control | logistic_regression | strict_window_fa<=1 | gradual | 2-5 | 6 | 387 | 0.062 [0.000, 0.131] | 0.333 [0.000, 0.667] |
| gaussian_control | logistic_regression | strict_window_fa<=1 | gradual | >5 | 9 | 614 | 0.166 [0.072, 0.287] | 0.556 [0.222, 0.889] |
| gaussian_control | logistic_regression | strict_window_fa<=1 | rapid | ALL | 30 | 1816 | 0.213 [0.107, 0.319] | 0.300 [0.133, 0.467] |
| gaussian_control | logistic_regression | strict_window_fa<=1 | rapid | <1 | 9 | 556 | 0.013 [0.000, 0.035] | 0.111 [0.000, 0.333] |
| gaussian_control | logistic_regression | strict_window_fa<=1 | rapid | 1-2 | 8 | 442 | 0.038 [0.002, 0.072] | 0.000 [0.000, 0.000] |
| gaussian_control | logistic_regression | strict_window_fa<=1 | rapid | 2-5 | 4 | 218 | 0.096 [0.000, 0.247] | 0.250 [0.000, 0.750] |
| gaussian_control | logistic_regression | strict_window_fa<=1 | rapid | >5 | 9 | 600 | 0.570 [0.339, 0.790] | 0.778 [0.556, 1.000] |
| gaussian_control | random_forest | episode_fa<=1 (k=3,m=3) | gradual | ALL | 30 | 2008 | 0.246 [0.160, 0.329] | 0.600 [0.433, 0.767] |
| gaussian_control | random_forest | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.186 [0.093, 0.291] | 0.600 [0.300, 0.853] |
| gaussian_control | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 339 | 0.083 [0.025, 0.147] | 0.400 [0.000, 0.800] |
| gaussian_control | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 387 | 0.300 [0.106, 0.512] | 0.667 [0.167, 1.000] |
| gaussian_control | random_forest | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 614 | 0.368 [0.190, 0.555] | 0.667 [0.333, 0.889] |
| gaussian_control | random_forest | episode_fa<=1 (k=3,m=3) | rapid | ALL | 30 | 1816 | 0.383 [0.241, 0.500] | 0.633 [0.467, 0.800] |
| gaussian_control | random_forest | episode_fa<=1 (k=3,m=3) | rapid | <1 | 9 | 556 | 0.097 [0.016, 0.199] | 0.444 [0.111, 0.778] |
| gaussian_control | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 8 | 442 | 0.197 [0.035, 0.379] | 0.500 [0.125, 0.875] |
| gaussian_control | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 218 | 0.211 [0.000, 0.466] | 0.500 [0.000, 1.000] |
| gaussian_control | random_forest | episode_fa<=1 (k=3,m=3) | rapid | >5 | 9 | 600 | 0.848 [0.765, 0.923] | 1.000 [1.000, 1.000] |
| gaussian_control | random_forest | strict_window_fa<=1 | gradual | ALL | 30 | 2008 | 0.148 [0.065, 0.231] | 0.367 [0.200, 0.567] |
| gaussian_control | random_forest | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.037 [0.013, 0.063] | 0.300 [0.048, 0.552] |
| gaussian_control | random_forest | strict_window_fa<=1 | gradual | 1-2 | 5 | 339 | 0.029 [0.000, 0.060] | 0.000 [0.000, 0.000] |
| gaussian_control | random_forest | strict_window_fa<=1 | gradual | 2-5 | 6 | 387 | 0.209 [0.040, 0.439] | 0.500 [0.079, 0.833] |
| gaussian_control | random_forest | strict_window_fa<=1 | gradual | >5 | 9 | 614 | 0.296 [0.114, 0.477] | 0.556 [0.222, 0.889] |
| gaussian_control | random_forest | strict_window_fa<=1 | rapid | ALL | 30 | 1816 | 0.300 [0.166, 0.420] | 0.433 [0.233, 0.600] |
| gaussian_control | random_forest | strict_window_fa<=1 | rapid | <1 | 9 | 556 | 0.045 [0.007, 0.106] | 0.222 [0.000, 0.556] |
| gaussian_control | random_forest | strict_window_fa<=1 | rapid | 1-2 | 8 | 442 | 0.079 [0.011, 0.198] | 0.125 [0.000, 0.375] |
| gaussian_control | random_forest | strict_window_fa<=1 | rapid | 2-5 | 4 | 218 | 0.142 [0.000, 0.419] | 0.250 [0.000, 0.750] |
| gaussian_control | random_forest | strict_window_fa<=1 | rapid | >5 | 9 | 600 | 0.755 [0.548, 0.891] | 1.000 [1.000, 1.000] |
| trough_panel | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | ALL | 30 | 2008 | 0.156 [0.102, 0.213] | 0.433 [0.267, 0.600] |
| trough_panel | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.121 [0.053, 0.205] | 0.400 [0.100, 0.600] |
| trough_panel | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 339 | 0.012 [0.000, 0.034] | 0.000 [0.000, 0.000] |
| trough_panel | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 387 | 0.152 [0.029, 0.289] | 0.333 [0.000, 0.667] |
| trough_panel | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 614 | 0.277 [0.165, 0.396] | 0.778 [0.444, 1.000] |
| trough_panel | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | ALL | 30 | 1816 | 0.252 [0.142, 0.357] | 0.467 [0.300, 0.633] |
| trough_panel | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | <1 | 9 | 556 | 0.061 [0.000, 0.167] | 0.111 [0.000, 0.333] |
| trough_panel | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 8 | 442 | 0.185 [0.049, 0.351] | 0.500 [0.125, 0.875] |
| trough_panel | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 218 | 0.257 [0.044, 0.541] | 0.500 [0.000, 1.000] |
| trough_panel | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | >5 | 9 | 600 | 0.475 [0.291, 0.650] | 0.778 [0.444, 1.000] |
| trough_panel | threshold_rule | strict_window_fa<=1 | gradual | ALL | 30 | 2008 | 0.156 [0.102, 0.213] | 0.333 [0.200, 0.500] |
| trough_panel | threshold_rule | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.121 [0.053, 0.205] | 0.100 [0.000, 0.300] |
| trough_panel | threshold_rule | strict_window_fa<=1 | gradual | 1-2 | 5 | 339 | 0.012 [0.000, 0.034] | 0.000 [0.000, 0.000] |
| trough_panel | threshold_rule | strict_window_fa<=1 | gradual | 2-5 | 6 | 387 | 0.152 [0.029, 0.289] | 0.333 [0.000, 0.667] |
| trough_panel | threshold_rule | strict_window_fa<=1 | gradual | >5 | 9 | 614 | 0.277 [0.165, 0.396] | 0.778 [0.444, 1.000] |
| trough_panel | threshold_rule | strict_window_fa<=1 | rapid | ALL | 30 | 1816 | 0.252 [0.142, 0.357] | 0.400 [0.267, 0.567] |
| trough_panel | threshold_rule | strict_window_fa<=1 | rapid | <1 | 9 | 556 | 0.061 [0.000, 0.167] | 0.111 [0.000, 0.333] |
| trough_panel | threshold_rule | strict_window_fa<=1 | rapid | 1-2 | 8 | 442 | 0.185 [0.049, 0.351] | 0.250 [0.000, 0.625] |
| trough_panel | threshold_rule | strict_window_fa<=1 | rapid | 2-5 | 4 | 218 | 0.257 [0.044, 0.541] | 0.500 [0.000, 1.000] |
| trough_panel | threshold_rule | strict_window_fa<=1 | rapid | >5 | 9 | 600 | 0.475 [0.291, 0.650] | 0.778 [0.444, 1.000] |
| trough_panel | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | ALL | 30 | 2008 | 0.100 [0.046, 0.154] | 0.333 [0.200, 0.500] |
| trough_panel | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.063 [0.018, 0.119] | 0.300 [0.100, 0.600] |
| trough_panel | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 339 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| trough_panel | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 387 | 0.119 [0.007, 0.238] | 0.333 [0.000, 0.667] |
| trough_panel | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 614 | 0.182 [0.072, 0.313] | 0.556 [0.222, 0.889] |
| trough_panel | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | ALL | 30 | 1816 | 0.290 [0.161, 0.419] | 0.433 [0.267, 0.600] |
| trough_panel | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | <1 | 9 | 556 | 0.023 [0.000, 0.049] | 0.111 [0.000, 0.333] |
| trough_panel | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 8 | 442 | 0.068 [0.000, 0.180] | 0.125 [0.000, 0.375] |
| trough_panel | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 218 | 0.156 [0.056, 0.255] | 0.750 [0.250, 1.000] |
| trough_panel | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | >5 | 9 | 600 | 0.748 [0.563, 0.888] | 0.889 [0.667, 1.000] |
| trough_panel | logistic_regression | strict_window_fa<=1 | gradual | ALL | 30 | 2008 | 0.021 [0.008, 0.038] | 0.067 [0.000, 0.167] |
| trough_panel | logistic_regression | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.012 [0.002, 0.028] | 0.000 [0.000, 0.000] |
| trough_panel | logistic_regression | strict_window_fa<=1 | gradual | 1-2 | 5 | 339 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| trough_panel | logistic_regression | strict_window_fa<=1 | gradual | 2-5 | 6 | 387 | 0.021 [0.000, 0.045] | 0.000 [0.000, 0.000] |
| trough_panel | logistic_regression | strict_window_fa<=1 | gradual | >5 | 9 | 614 | 0.044 [0.006, 0.092] | 0.222 [0.000, 0.556] |
| trough_panel | logistic_regression | strict_window_fa<=1 | rapid | ALL | 30 | 1816 | 0.187 [0.078, 0.291] | 0.300 [0.167, 0.467] |
| trough_panel | logistic_regression | strict_window_fa<=1 | rapid | <1 | 9 | 556 | 0.004 [0.000, 0.011] | 0.000 [0.000, 0.000] |
| trough_panel | logistic_regression | strict_window_fa<=1 | rapid | 1-2 | 8 | 442 | 0.020 [0.000, 0.055] | 0.125 [0.000, 0.375] |
| trough_panel | logistic_regression | strict_window_fa<=1 | rapid | 2-5 | 4 | 218 | 0.028 [0.005, 0.059] | 0.000 [0.000, 0.000] |
| trough_panel | logistic_regression | strict_window_fa<=1 | rapid | >5 | 9 | 600 | 0.538 [0.344, 0.732] | 0.889 [0.667, 1.000] |
| trough_panel | random_forest | episode_fa<=1 (k=3,m=3) | gradual | ALL | 30 | 2008 | 0.138 [0.094, 0.196] | 0.567 [0.400, 0.733] |
| trough_panel | random_forest | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.130 [0.062, 0.207] | 0.600 [0.300, 0.853] |
| trough_panel | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 339 | 0.080 [0.031, 0.127] | 0.600 [0.200, 1.000] |
| trough_panel | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 387 | 0.168 [0.088, 0.227] | 0.667 [0.333, 1.000] |
| trough_panel | random_forest | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 614 | 0.160 [0.045, 0.338] | 0.444 [0.222, 0.778] |
| trough_panel | random_forest | episode_fa<=1 (k=3,m=3) | rapid | ALL | 30 | 1816 | 0.299 [0.169, 0.431] | 0.500 [0.333, 0.700] |
| trough_panel | random_forest | episode_fa<=1 (k=3,m=3) | rapid | <1 | 9 | 556 | 0.036 [0.001, 0.073] | 0.333 [0.111, 0.667] |
| trough_panel | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 8 | 442 | 0.138 [0.004, 0.338] | 0.250 [0.000, 0.500] |
| trough_panel | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 218 | 0.105 [0.009, 0.198] | 0.500 [0.000, 1.000] |
| trough_panel | random_forest | episode_fa<=1 (k=3,m=3) | rapid | >5 | 9 | 600 | 0.732 [0.487, 0.942] | 0.889 [0.667, 1.000] |
| trough_panel | random_forest | strict_window_fa<=1 | gradual | ALL | 30 | 2008 | 0.048 [0.015, 0.098] | 0.167 [0.033, 0.300] |
| trough_panel | random_forest | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.021 [0.003, 0.041] | 0.100 [0.000, 0.300] |
| trough_panel | random_forest | strict_window_fa<=1 | gradual | 1-2 | 5 | 339 | 0.015 [0.003, 0.029] | 0.000 [0.000, 0.000] |
| trough_panel | random_forest | strict_window_fa<=1 | gradual | 2-5 | 6 | 387 | 0.052 [0.019, 0.084] | 0.333 [0.000, 0.754] |
| trough_panel | random_forest | strict_window_fa<=1 | gradual | >5 | 9 | 614 | 0.093 [0.005, 0.263] | 0.222 [0.000, 0.556] |
| trough_panel | random_forest | strict_window_fa<=1 | rapid | ALL | 30 | 1816 | 0.233 [0.105, 0.355] | 0.333 [0.182, 0.533] |
| trough_panel | random_forest | strict_window_fa<=1 | rapid | <1 | 9 | 556 | 0.013 [0.001, 0.028] | 0.111 [0.000, 0.333] |
| trough_panel | random_forest | strict_window_fa<=1 | rapid | 1-2 | 8 | 442 | 0.048 [0.000, 0.117] | 0.250 [0.000, 0.500] |
| trough_panel | random_forest | strict_window_fa<=1 | rapid | 2-5 | 4 | 218 | 0.009 [0.000, 0.018] | 0.000 [0.000, 0.000] |
| trough_panel | random_forest | strict_window_fa<=1 | rapid | >5 | 9 | 600 | 0.655 [0.405, 0.892] | 0.778 [0.444, 1.000] |
| asymmetric | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | ALL | 30 | 2008 | 0.202 [0.136, 0.280] | 0.467 [0.300, 0.651] |
| asymmetric | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.123 [0.053, 0.208] | 0.400 [0.100, 0.600] |
| asymmetric | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 339 | 0.012 [0.000, 0.034] | 0.000 [0.000, 0.000] |
| asymmetric | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 387 | 0.127 [0.003, 0.270] | 0.333 [0.000, 0.667] |
| asymmetric | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 614 | 0.441 [0.343, 0.539] | 0.889 [0.667, 1.000] |
| asymmetric | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | ALL | 30 | 1816 | 0.259 [0.167, 0.370] | 0.400 [0.233, 0.551] |
| asymmetric | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | <1 | 9 | 556 | 0.058 [0.000, 0.157] | 0.111 [0.000, 0.333] |
| asymmetric | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 8 | 442 | 0.176 [0.048, 0.324] | 0.375 [0.000, 0.750] |
| asymmetric | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 218 | 0.238 [0.044, 0.536] | 0.250 [0.000, 0.750] |
| asymmetric | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | >5 | 9 | 600 | 0.513 [0.327, 0.673] | 0.778 [0.556, 1.000] |
| asymmetric | threshold_rule | strict_window_fa<=1 | gradual | ALL | 30 | 2008 | 0.202 [0.136, 0.280] | 0.300 [0.133, 0.467] |
| asymmetric | threshold_rule | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.123 [0.053, 0.208] | 0.000 [0.000, 0.000] |
| asymmetric | threshold_rule | strict_window_fa<=1 | gradual | 1-2 | 5 | 339 | 0.012 [0.000, 0.034] | 0.000 [0.000, 0.000] |
| asymmetric | threshold_rule | strict_window_fa<=1 | gradual | 2-5 | 6 | 387 | 0.127 [0.003, 0.270] | 0.167 [0.000, 0.500] |
| asymmetric | threshold_rule | strict_window_fa<=1 | gradual | >5 | 9 | 614 | 0.441 [0.343, 0.539] | 0.889 [0.667, 1.000] |
| asymmetric | threshold_rule | strict_window_fa<=1 | rapid | ALL | 30 | 1816 | 0.259 [0.167, 0.370] | 0.333 [0.182, 0.500] |
| asymmetric | threshold_rule | strict_window_fa<=1 | rapid | <1 | 9 | 556 | 0.058 [0.000, 0.157] | 0.111 [0.000, 0.333] |
| asymmetric | threshold_rule | strict_window_fa<=1 | rapid | 1-2 | 8 | 442 | 0.176 [0.048, 0.324] | 0.250 [0.000, 0.625] |
| asymmetric | threshold_rule | strict_window_fa<=1 | rapid | 2-5 | 4 | 218 | 0.238 [0.044, 0.536] | 0.250 [0.000, 0.750] |
| asymmetric | threshold_rule | strict_window_fa<=1 | rapid | >5 | 9 | 600 | 0.513 [0.327, 0.673] | 0.667 [0.333, 0.889] |
| asymmetric | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | ALL | 30 | 2008 | 0.139 [0.076, 0.216] | 0.367 [0.200, 0.533] |
| asymmetric | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.066 [0.020, 0.131] | 0.300 [0.100, 0.600] |
| asymmetric | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 339 | 0.006 [0.000, 0.012] | 0.000 [0.000, 0.000] |
| asymmetric | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 387 | 0.194 [0.000, 0.404] | 0.333 [0.000, 0.667] |
| asymmetric | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 614 | 0.257 [0.139, 0.406] | 0.667 [0.333, 0.889] |
| asymmetric | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | ALL | 30 | 1816 | 0.357 [0.231, 0.484] | 0.533 [0.333, 0.733] |
| asymmetric | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | <1 | 9 | 556 | 0.056 [0.006, 0.116] | 0.222 [0.000, 0.556] |
| asymmetric | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 8 | 442 | 0.138 [0.024, 0.254] | 0.375 [0.059, 0.750] |
| asymmetric | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 218 | 0.339 [0.037, 0.636] | 0.500 [0.000, 1.000] |
| asymmetric | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | >5 | 9 | 600 | 0.805 [0.665, 0.926] | 1.000 [1.000, 1.000] |
| asymmetric | logistic_regression | strict_window_fa<=1 | gradual | ALL | 30 | 2008 | 0.047 [0.011, 0.106] | 0.133 [0.033, 0.267] |
| asymmetric | logistic_regression | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.012 [0.002, 0.026] | 0.000 [0.000, 0.000] |
| asymmetric | logistic_regression | strict_window_fa<=1 | gradual | 1-2 | 5 | 339 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| asymmetric | logistic_regression | strict_window_fa<=1 | gradual | 2-5 | 6 | 387 | 0.075 [0.000, 0.172] | 0.333 [0.000, 0.667] |
| asymmetric | logistic_regression | strict_window_fa<=1 | gradual | >5 | 9 | 614 | 0.093 [0.015, 0.230] | 0.222 [0.000, 0.503] |
| asymmetric | logistic_regression | strict_window_fa<=1 | rapid | ALL | 30 | 1816 | 0.211 [0.104, 0.319] | 0.400 [0.233, 0.567] |
| asymmetric | logistic_regression | strict_window_fa<=1 | rapid | <1 | 9 | 556 | 0.020 [0.001, 0.053] | 0.111 [0.000, 0.333] |
| asymmetric | logistic_regression | strict_window_fa<=1 | rapid | 1-2 | 8 | 442 | 0.041 [0.002, 0.079] | 0.125 [0.000, 0.375] |
| asymmetric | logistic_regression | strict_window_fa<=1 | rapid | 2-5 | 4 | 218 | 0.096 [0.000, 0.191] | 0.500 [0.000, 1.000] |
| asymmetric | logistic_regression | strict_window_fa<=1 | rapid | >5 | 9 | 600 | 0.555 [0.330, 0.762] | 0.889 [0.667, 1.000] |
| asymmetric | random_forest | episode_fa<=1 (k=3,m=3) | gradual | ALL | 30 | 2008 | 0.241 [0.160, 0.337] | 0.600 [0.400, 0.767] |
| asymmetric | random_forest | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.184 [0.097, 0.282] | 0.600 [0.300, 0.853] |
| asymmetric | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 339 | 0.077 [0.015, 0.132] | 0.400 [0.000, 0.800] |
| asymmetric | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 387 | 0.333 [0.100, 0.560] | 0.667 [0.246, 1.000] |
| asymmetric | random_forest | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 614 | 0.337 [0.145, 0.552] | 0.667 [0.333, 0.889] |
| asymmetric | random_forest | episode_fa<=1 (k=3,m=3) | rapid | ALL | 30 | 1816 | 0.353 [0.217, 0.478] | 0.600 [0.433, 0.800] |
| asymmetric | random_forest | episode_fa<=1 (k=3,m=3) | rapid | <1 | 9 | 556 | 0.106 [0.018, 0.221] | 0.556 [0.222, 0.889] |
| asymmetric | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 8 | 442 | 0.215 [0.035, 0.421] | 0.500 [0.125, 0.875] |
| asymmetric | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 218 | 0.110 [0.009, 0.203] | 0.250 [0.000, 0.750] |
| asymmetric | random_forest | episode_fa<=1 (k=3,m=3) | rapid | >5 | 9 | 600 | 0.772 [0.580, 0.902] | 0.889 [0.667, 1.000] |
| asymmetric | random_forest | strict_window_fa<=1 | gradual | ALL | 30 | 2008 | 0.159 [0.078, 0.249] | 0.433 [0.267, 0.633] |
| asymmetric | random_forest | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.046 [0.015, 0.079] | 0.300 [0.048, 0.552] |
| asymmetric | random_forest | strict_window_fa<=1 | gradual | 1-2 | 5 | 339 | 0.026 [0.000, 0.054] | 0.200 [0.000, 0.600] |
| asymmetric | random_forest | strict_window_fa<=1 | gradual | 2-5 | 6 | 387 | 0.222 [0.028, 0.433] | 0.500 [0.079, 0.833] |
| asymmetric | random_forest | strict_window_fa<=1 | gradual | >5 | 9 | 614 | 0.314 [0.130, 0.528] | 0.667 [0.333, 0.889] |
| asymmetric | random_forest | strict_window_fa<=1 | rapid | ALL | 30 | 1816 | 0.281 [0.149, 0.407] | 0.367 [0.216, 0.551] |
| asymmetric | random_forest | strict_window_fa<=1 | rapid | <1 | 9 | 556 | 0.036 [0.001, 0.095] | 0.111 [0.000, 0.333] |
| asymmetric | random_forest | strict_window_fa<=1 | rapid | 1-2 | 8 | 442 | 0.079 [0.013, 0.185] | 0.250 [0.000, 0.500] |
| asymmetric | random_forest | strict_window_fa<=1 | rapid | 2-5 | 4 | 218 | 0.041 [0.000, 0.122] | 0.000 [0.000, 0.000] |
| asymmetric | random_forest | strict_window_fa<=1 | rapid | >5 | 9 | 600 | 0.745 [0.526, 0.895] | 0.889 [0.667, 1.000] |
| two_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | ALL | 30 | 2008 | 0.187 [0.125, 0.256] | 0.467 [0.300, 0.618] |
| two_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.129 [0.055, 0.220] | 0.400 [0.100, 0.600] |
| two_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 339 | 0.012 [0.000, 0.034] | 0.000 [0.000, 0.000] |
| two_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 387 | 0.168 [0.052, 0.295] | 0.500 [0.167, 0.833] |
| two_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 614 | 0.358 [0.231, 0.498] | 0.778 [0.444, 1.000] |
| two_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | ALL | 30 | 1816 | 0.268 [0.160, 0.380] | 0.467 [0.300, 0.633] |
| two_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | <1 | 9 | 556 | 0.061 [0.000, 0.164] | 0.222 [0.000, 0.556] |
| two_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 8 | 442 | 0.181 [0.052, 0.334] | 0.500 [0.125, 0.875] |
| two_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 218 | 0.193 [0.009, 0.555] | 0.250 [0.000, 0.750] |
| two_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | >5 | 9 | 600 | 0.552 [0.349, 0.707] | 0.778 [0.444, 1.000] |
| two_basin | threshold_rule | strict_window_fa<=1 | gradual | ALL | 30 | 2008 | 0.187 [0.125, 0.256] | 0.300 [0.133, 0.467] |
| two_basin | threshold_rule | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.129 [0.055, 0.220] | 0.000 [0.000, 0.000] |
| two_basin | threshold_rule | strict_window_fa<=1 | gradual | 1-2 | 5 | 339 | 0.012 [0.000, 0.034] | 0.000 [0.000, 0.000] |
| two_basin | threshold_rule | strict_window_fa<=1 | gradual | 2-5 | 6 | 387 | 0.168 [0.052, 0.295] | 0.333 [0.000, 0.667] |
| two_basin | threshold_rule | strict_window_fa<=1 | gradual | >5 | 9 | 614 | 0.358 [0.231, 0.498] | 0.778 [0.444, 1.000] |
| two_basin | threshold_rule | strict_window_fa<=1 | rapid | ALL | 30 | 1816 | 0.268 [0.160, 0.380] | 0.367 [0.200, 0.533] |
| two_basin | threshold_rule | strict_window_fa<=1 | rapid | <1 | 9 | 556 | 0.061 [0.000, 0.164] | 0.111 [0.000, 0.333] |
| two_basin | threshold_rule | strict_window_fa<=1 | rapid | 1-2 | 8 | 442 | 0.181 [0.052, 0.334] | 0.250 [0.000, 0.566] |
| two_basin | threshold_rule | strict_window_fa<=1 | rapid | 2-5 | 4 | 218 | 0.193 [0.009, 0.555] | 0.250 [0.000, 0.750] |
| two_basin | threshold_rule | strict_window_fa<=1 | rapid | >5 | 9 | 600 | 0.552 [0.349, 0.707] | 0.778 [0.444, 1.000] |
| two_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | ALL | 30 | 2008 | 0.144 [0.069, 0.226] | 0.333 [0.200, 0.500] |
| two_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.073 [0.022, 0.150] | 0.300 [0.100, 0.600] |
| two_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 339 | 0.006 [0.000, 0.017] | 0.000 [0.000, 0.000] |
| two_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 387 | 0.194 [0.003, 0.409] | 0.333 [0.000, 0.667] |
| two_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 614 | 0.266 [0.090, 0.451] | 0.556 [0.222, 0.889] |
| two_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | ALL | 30 | 1816 | 0.287 [0.155, 0.407] | 0.400 [0.216, 0.567] |
| two_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | <1 | 9 | 556 | 0.054 [0.007, 0.104] | 0.222 [0.000, 0.556] |
| two_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 8 | 442 | 0.100 [0.022, 0.225] | 0.125 [0.000, 0.375] |
| two_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 218 | 0.170 [0.033, 0.404] | 0.250 [0.000, 0.750] |
| two_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | >5 | 9 | 600 | 0.685 [0.462, 0.920] | 0.889 [0.667, 1.000] |
| two_basin | logistic_regression | strict_window_fa<=1 | gradual | ALL | 30 | 2008 | 0.058 [0.019, 0.106] | 0.133 [0.033, 0.267] |
| two_basin | logistic_regression | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.013 [0.003, 0.029] | 0.000 [0.000, 0.000] |
| two_basin | logistic_regression | strict_window_fa<=1 | gradual | 1-2 | 5 | 339 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| two_basin | logistic_regression | strict_window_fa<=1 | gradual | 2-5 | 6 | 387 | 0.067 [0.000, 0.168] | 0.167 [0.000, 0.500] |
| two_basin | logistic_regression | strict_window_fa<=1 | gradual | >5 | 9 | 614 | 0.134 [0.035, 0.253] | 0.333 [0.111, 0.667] |
| two_basin | logistic_regression | strict_window_fa<=1 | rapid | ALL | 30 | 1816 | 0.169 [0.061, 0.281] | 0.267 [0.100, 0.417] |
| two_basin | logistic_regression | strict_window_fa<=1 | rapid | <1 | 9 | 556 | 0.005 [0.002, 0.010] | 0.000 [0.000, 0.000] |
| two_basin | logistic_regression | strict_window_fa<=1 | rapid | 1-2 | 8 | 442 | 0.016 [0.000, 0.039] | 0.000 [0.000, 0.000] |
| two_basin | logistic_regression | strict_window_fa<=1 | rapid | 2-5 | 4 | 218 | 0.041 [0.000, 0.096] | 0.250 [0.000, 0.750] |
| two_basin | logistic_regression | strict_window_fa<=1 | rapid | >5 | 9 | 600 | 0.480 [0.269, 0.763] | 0.778 [0.556, 1.000] |
| two_basin | random_forest | episode_fa<=1 (k=3,m=3) | gradual | ALL | 30 | 2008 | 0.278 [0.168, 0.385] | 0.567 [0.400, 0.767] |
| two_basin | random_forest | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.199 [0.101, 0.322] | 0.600 [0.300, 0.853] |
| two_basin | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 339 | 0.094 [0.034, 0.159] | 0.400 [0.000, 0.800] |
| two_basin | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 387 | 0.313 [0.066, 0.555] | 0.500 [0.079, 0.833] |
| two_basin | random_forest | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 614 | 0.443 [0.254, 0.651] | 0.667 [0.333, 0.889] |
| two_basin | random_forest | episode_fa<=1 (k=3,m=3) | rapid | ALL | 30 | 1816 | 0.325 [0.187, 0.440] | 0.600 [0.416, 0.800] |
| two_basin | random_forest | episode_fa<=1 (k=3,m=3) | rapid | <1 | 9 | 556 | 0.090 [0.018, 0.175] | 0.444 [0.111, 0.778] |
| two_basin | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 8 | 442 | 0.131 [0.022, 0.273] | 0.250 [0.000, 0.500] |
| two_basin | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 218 | 0.216 [0.055, 0.415] | 0.750 [0.250, 1.000] |
| two_basin | random_forest | episode_fa<=1 (k=3,m=3) | rapid | >5 | 9 | 600 | 0.727 [0.549, 0.897] | 1.000 [1.000, 1.000] |
| two_basin | random_forest | strict_window_fa<=1 | gradual | ALL | 30 | 2008 | 0.190 [0.099, 0.289] | 0.400 [0.249, 0.600] |
| two_basin | random_forest | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.048 [0.015, 0.083] | 0.300 [0.048, 0.552] |
| two_basin | random_forest | strict_window_fa<=1 | gradual | 1-2 | 5 | 339 | 0.029 [0.000, 0.061] | 0.000 [0.000, 0.000] |
| two_basin | random_forest | strict_window_fa<=1 | gradual | 2-5 | 6 | 387 | 0.258 [0.032, 0.482] | 0.500 [0.079, 0.833] |
| two_basin | random_forest | strict_window_fa<=1 | gradual | >5 | 9 | 614 | 0.389 [0.219, 0.596] | 0.667 [0.333, 0.889] |
| two_basin | random_forest | strict_window_fa<=1 | rapid | ALL | 30 | 1816 | 0.230 [0.097, 0.354] | 0.400 [0.233, 0.584] |
| two_basin | random_forest | strict_window_fa<=1 | rapid | <1 | 9 | 556 | 0.036 [0.008, 0.068] | 0.222 [0.000, 0.556] |
| two_basin | random_forest | strict_window_fa<=1 | rapid | 1-2 | 8 | 442 | 0.036 [0.000, 0.087] | 0.250 [0.000, 0.500] |
| two_basin | random_forest | strict_window_fa<=1 | rapid | 2-5 | 4 | 218 | 0.055 [0.000, 0.135] | 0.250 [0.000, 0.750] |
| two_basin | random_forest | strict_window_fa<=1 | rapid | >5 | 9 | 600 | 0.615 [0.376, 0.861] | 0.778 [0.556, 1.000] |
| planar_slope | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | ALL | 30 | 2008 | 0.260 [0.191, 0.335] | 0.700 [0.533, 0.833] |
| planar_slope | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.127 [0.054, 0.216] | 0.500 [0.200, 0.800] |
| planar_slope | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 339 | 0.026 [0.000, 0.075] | 0.200 [0.000, 0.600] |
| planar_slope | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 387 | 0.336 [0.282, 0.393] | 1.000 [1.000, 1.000] |
| planar_slope | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 614 | 0.485 [0.422, 0.567] | 1.000 [1.000, 1.000] |
| planar_slope | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | ALL | 30 | 1816 | 0.374 [0.262, 0.494] | 0.567 [0.400, 0.733] |
| planar_slope | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | <1 | 9 | 556 | 0.068 [0.002, 0.178] | 0.111 [0.000, 0.333] |
| planar_slope | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 8 | 442 | 0.317 [0.089, 0.553] | 0.500 [0.125, 0.875] |
| planar_slope | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 218 | 0.404 [0.111, 0.694] | 0.750 [0.250, 1.000] |
| planar_slope | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | >5 | 9 | 600 | 0.690 [0.622, 0.749] | 1.000 [1.000, 1.000] |
| planar_slope | threshold_rule | strict_window_fa<=1 | gradual | ALL | 30 | 2008 | 0.260 [0.191, 0.335] | 0.500 [0.333, 0.700] |
| planar_slope | threshold_rule | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.127 [0.054, 0.216] | 0.000 [0.000, 0.000] |
| planar_slope | threshold_rule | strict_window_fa<=1 | gradual | 1-2 | 5 | 339 | 0.026 [0.000, 0.075] | 0.000 [0.000, 0.000] |
| planar_slope | threshold_rule | strict_window_fa<=1 | gradual | 2-5 | 6 | 387 | 0.336 [0.282, 0.393] | 1.000 [1.000, 1.000] |
| planar_slope | threshold_rule | strict_window_fa<=1 | gradual | >5 | 9 | 614 | 0.485 [0.422, 0.567] | 1.000 [1.000, 1.000] |
| planar_slope | threshold_rule | strict_window_fa<=1 | rapid | ALL | 30 | 1816 | 0.374 [0.262, 0.494] | 0.533 [0.367, 0.700] |
| planar_slope | threshold_rule | strict_window_fa<=1 | rapid | <1 | 9 | 556 | 0.068 [0.002, 0.178] | 0.111 [0.000, 0.333] |
| planar_slope | threshold_rule | strict_window_fa<=1 | rapid | 1-2 | 8 | 442 | 0.317 [0.089, 0.553] | 0.500 [0.125, 0.875] |
| planar_slope | threshold_rule | strict_window_fa<=1 | rapid | 2-5 | 4 | 218 | 0.404 [0.111, 0.694] | 0.500 [0.000, 1.000] |
| planar_slope | threshold_rule | strict_window_fa<=1 | rapid | >5 | 9 | 600 | 0.690 [0.622, 0.749] | 1.000 [1.000, 1.000] |
| planar_slope | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | ALL | 30 | 2008 | 0.141 [0.067, 0.226] | 0.400 [0.233, 0.600] |
| planar_slope | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.046 [0.004, 0.099] | 0.200 [0.000, 0.453] |
| planar_slope | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 339 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| planar_slope | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 387 | 0.072 [0.010, 0.166] | 0.333 [0.000, 0.667] |
| planar_slope | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 614 | 0.365 [0.233, 0.514] | 0.889 [0.667, 1.000] |
| planar_slope | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | ALL | 30 | 1816 | 0.242 [0.150, 0.334] | 0.600 [0.433, 0.767] |
| planar_slope | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | <1 | 9 | 556 | 0.077 [0.019, 0.163] | 0.333 [0.000, 0.556] |
| planar_slope | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 8 | 442 | 0.265 [0.099, 0.436] | 0.625 [0.250, 1.000] |
| planar_slope | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 218 | 0.197 [0.026, 0.468] | 0.500 [0.000, 1.000] |
| planar_slope | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | >5 | 9 | 600 | 0.393 [0.227, 0.578] | 0.889 [0.667, 1.000] |
| planar_slope | logistic_regression | strict_window_fa<=1 | gradual | ALL | 30 | 2008 | 0.085 [0.033, 0.145] | 0.233 [0.100, 0.384] |
| planar_slope | logistic_regression | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.009 [0.000, 0.027] | 0.000 [0.000, 0.000] |
| planar_slope | logistic_regression | strict_window_fa<=1 | gradual | 1-2 | 5 | 339 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| planar_slope | logistic_regression | strict_window_fa<=1 | gradual | 2-5 | 6 | 387 | 0.023 [0.003, 0.056] | 0.167 [0.000, 0.500] |
| planar_slope | logistic_regression | strict_window_fa<=1 | gradual | >5 | 9 | 614 | 0.252 [0.136, 0.397] | 0.667 [0.333, 0.889] |
| planar_slope | logistic_regression | strict_window_fa<=1 | rapid | ALL | 30 | 1816 | 0.151 [0.076, 0.231] | 0.367 [0.200, 0.567] |
| planar_slope | logistic_regression | strict_window_fa<=1 | rapid | <1 | 9 | 556 | 0.036 [0.005, 0.092] | 0.111 [0.000, 0.333] |
| planar_slope | logistic_regression | strict_window_fa<=1 | rapid | 1-2 | 8 | 442 | 0.156 [0.040, 0.288] | 0.375 [0.125, 0.750] |
| planar_slope | logistic_regression | strict_window_fa<=1 | rapid | 2-5 | 4 | 218 | 0.119 [0.009, 0.315] | 0.250 [0.000, 0.750] |
| planar_slope | logistic_regression | strict_window_fa<=1 | rapid | >5 | 9 | 600 | 0.265 [0.083, 0.466] | 0.667 [0.333, 0.947] |
| planar_slope | random_forest | episode_fa<=1 (k=3,m=3) | gradual | ALL | 30 | 2008 | 0.157 [0.096, 0.225] | 0.467 [0.282, 0.651] |
| planar_slope | random_forest | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.193 [0.095, 0.312] | 0.500 [0.200, 0.800] |
| planar_slope | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 339 | 0.038 [0.003, 0.096] | 0.200 [0.000, 0.600] |
| planar_slope | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 387 | 0.124 [0.016, 0.312] | 0.167 [0.000, 0.500] |
| planar_slope | random_forest | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 614 | 0.204 [0.119, 0.301] | 0.778 [0.444, 1.000] |
| planar_slope | random_forest | episode_fa<=1 (k=3,m=3) | rapid | ALL | 30 | 1816 | 0.236 [0.151, 0.337] | 0.633 [0.433, 0.800] |
| planar_slope | random_forest | episode_fa<=1 (k=3,m=3) | rapid | <1 | 9 | 556 | 0.101 [0.032, 0.188] | 0.444 [0.111, 0.778] |
| planar_slope | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 8 | 442 | 0.242 [0.084, 0.420] | 0.500 [0.184, 0.875] |
| planar_slope | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 218 | 0.101 [0.032, 0.161] | 0.750 [0.250, 1.000] |
| planar_slope | random_forest | episode_fa<=1 (k=3,m=3) | rapid | >5 | 9 | 600 | 0.405 [0.223, 0.558] | 0.889 [0.667, 1.000] |
| planar_slope | random_forest | strict_window_fa<=1 | gradual | ALL | 30 | 2008 | 0.044 [0.017, 0.082] | 0.200 [0.067, 0.333] |
| planar_slope | random_forest | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.025 [0.004, 0.052] | 0.100 [0.000, 0.300] |
| planar_slope | random_forest | strict_window_fa<=1 | gradual | 1-2 | 5 | 339 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| planar_slope | random_forest | strict_window_fa<=1 | gradual | 2-5 | 6 | 387 | 0.034 [0.000, 0.094] | 0.000 [0.000, 0.000] |
| planar_slope | random_forest | strict_window_fa<=1 | gradual | >5 | 9 | 614 | 0.095 [0.026, 0.169] | 0.556 [0.222, 0.889] |
| planar_slope | random_forest | strict_window_fa<=1 | rapid | ALL | 30 | 1816 | 0.121 [0.070, 0.173] | 0.433 [0.249, 0.600] |
| planar_slope | random_forest | strict_window_fa<=1 | rapid | <1 | 9 | 556 | 0.034 [0.005, 0.074] | 0.222 [0.000, 0.503] |
| planar_slope | random_forest | strict_window_fa<=1 | rapid | 1-2 | 8 | 442 | 0.113 [0.034, 0.206] | 0.375 [0.125, 0.750] |
| planar_slope | random_forest | strict_window_fa<=1 | rapid | 2-5 | 4 | 218 | 0.060 [0.013, 0.119] | 0.250 [0.000, 0.750] |
| planar_slope | random_forest | strict_window_fa<=1 | rapid | >5 | 9 | 600 | 0.228 [0.104, 0.341] | 0.778 [0.497, 1.000] |
