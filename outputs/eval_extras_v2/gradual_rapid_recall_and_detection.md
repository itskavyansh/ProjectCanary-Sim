# Gradual / rapid: window recall and run-level detection together (SYNTHETIC / SIMULATION)

> **SYNTHETIC / SIMULATION** - all data are simulated; nothing here is validated on real data or field-ready.

Window recall = share of true gradual (rapid) windows predicted as that class by the model/operating point (before persistence). Run-level detection = share of gradual (rapid) runs with at least one alarm of that class after the regime's (k, m) persistence; it counts ANY correct alarm in the run, so it is always shown next to window recall and is never a substitute for it. Own-class rule: in the stress set an alarm of a co-occurring other class does not count. snr_vs_imu_noise = run's peak tilt / IMU noise (manifest).

| split | model | regime | class | runs | windows | window recall | run-level detection |
|---|---|---|---|---|---|---|---|
| test | threshold_rule | raw (k=1) | gradual | 20 | 1333 | 0.158 [0.094, 0.217] | 0.600 [0.400, 0.800] |
| test | threshold_rule | raw (k=1) | rapid | 20 | 1167 | 0.274 [0.159, 0.402] | 0.650 [0.450, 0.850] |
| test | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 20 | 1333 | 0.158 [0.094, 0.217] | 0.450 [0.224, 0.650] |
| test | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 20 | 1167 | 0.274 [0.159, 0.402] | 0.450 [0.250, 0.650] |
| test | threshold_rule | strict_window_fa<=1 | gradual | 20 | 1333 | 0.158 [0.094, 0.217] | 0.300 [0.100, 0.500] |
| test | threshold_rule | strict_window_fa<=1 | rapid | 20 | 1167 | 0.274 [0.159, 0.402] | 0.400 [0.200, 0.600] |
| test | logistic_regression | raw (k=1) | gradual | 20 | 1333 | 0.242 [0.142, 0.343] | 0.800 [0.600, 0.950] |
| test | logistic_regression | raw (k=1) | rapid | 20 | 1167 | 0.343 [0.204, 0.483] | 1.000 [1.000, 1.000] |
| test | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 20 | 1333 | 0.085 [0.026, 0.164] | 0.300 [0.100, 0.500] |
| test | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 20 | 1167 | 0.209 [0.083, 0.353] | 0.350 [0.150, 0.550] |
| test | logistic_regression | strict_window_fa<=1 | gradual | 20 | 1333 | 0.036 [0.001, 0.099] | 0.100 [0.000, 0.226] |
| test | logistic_regression | strict_window_fa<=1 | rapid | 20 | 1167 | 0.141 [0.031, 0.270] | 0.250 [0.074, 0.450] |
| test | random_forest | raw (k=1) | gradual | 20 | 1333 | 0.205 [0.120, 0.302] | 0.750 [0.600, 0.926] |
| test | random_forest | raw (k=1) | rapid | 20 | 1167 | 0.291 [0.138, 0.442] | 0.650 [0.450, 0.850] |
| test | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 20 | 1333 | 0.158 [0.076, 0.248] | 0.400 [0.200, 0.600] |
| test | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 20 | 1167 | 0.284 [0.135, 0.437] | 0.400 [0.200, 0.600] |
| test | random_forest | strict_window_fa<=1 | gradual | 20 | 1333 | 0.112 [0.040, 0.189] | 0.300 [0.150, 0.500] |
| test | random_forest | strict_window_fa<=1 | rapid | 20 | 1167 | 0.220 [0.073, 0.369] | 0.250 [0.074, 0.450] |
| shifted_test | threshold_rule | raw (k=1) | gradual | 15 | 1035 | 0.293 [0.256, 0.335] | 1.000 [1.000, 1.000] |
| shifted_test | threshold_rule | raw (k=1) | rapid | 15 | 916 | 0.416 [0.288, 0.564] | 1.000 [1.000, 1.000] |
| shifted_test | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 15 | 1035 | 0.293 [0.256, 0.335] | 0.867 [0.667, 1.000] |
| shifted_test | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 15 | 916 | 0.416 [0.288, 0.564] | 0.667 [0.432, 0.867] |
| shifted_test | threshold_rule | strict_window_fa<=1 | gradual | 15 | 1035 | 0.293 [0.256, 0.335] | 0.400 [0.200, 0.600] |
| shifted_test | threshold_rule | strict_window_fa<=1 | rapid | 15 | 916 | 0.416 [0.288, 0.564] | 0.467 [0.200, 0.733] |
| shifted_test | logistic_regression | raw (k=1) | gradual | 15 | 1035 | 0.449 [0.337, 0.558] | 1.000 [1.000, 1.000] |
| shifted_test | logistic_regression | raw (k=1) | rapid | 15 | 916 | 0.234 [0.135, 0.326] | 0.933 [0.800, 1.000] |
| shifted_test | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 15 | 1035 | 0.149 [0.081, 0.253] | 0.400 [0.133, 0.667] |
| shifted_test | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 15 | 916 | 0.129 [0.059, 0.206] | 0.467 [0.200, 0.733] |
| shifted_test | logistic_regression | strict_window_fa<=1 | gradual | 15 | 1035 | 0.044 [0.011, 0.099] | 0.067 [0.000, 0.200] |
| shifted_test | logistic_regression | strict_window_fa<=1 | rapid | 15 | 916 | 0.037 [0.018, 0.059] | 0.067 [0.000, 0.200] |
| shifted_test | random_forest | raw (k=1) | gradual | 15 | 1035 | 0.431 [0.326, 0.539] | 1.000 [1.000, 1.000] |
| shifted_test | random_forest | raw (k=1) | rapid | 15 | 916 | 0.141 [0.047, 0.251] | 0.600 [0.365, 0.800] |
| shifted_test | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 15 | 1035 | 0.271 [0.166, 0.403] | 0.733 [0.467, 0.933] |
| shifted_test | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 15 | 916 | 0.128 [0.036, 0.234] | 0.400 [0.200, 0.667] |
| shifted_test | random_forest | strict_window_fa<=1 | gradual | 15 | 1035 | 0.155 [0.057, 0.300] | 0.533 [0.267, 0.768] |
| shifted_test | random_forest | strict_window_fa<=1 | rapid | 15 | 916 | 0.100 [0.014, 0.202] | 0.267 [0.067, 0.533] |
| stress | threshold_rule | raw (k=1) | gradual | 30 | 1991 | 0.163 [0.106, 0.213] | 0.733 [0.583, 0.900] |
| stress | threshold_rule | raw (k=1) | rapid | 28 | 1784 | 0.198 [0.122, 0.280] | 0.607 [0.429, 0.769] |
| stress | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 30 | 1991 | 0.163 [0.106, 0.213] | 0.433 [0.267, 0.600] |
| stress | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 28 | 1784 | 0.198 [0.122, 0.280] | 0.429 [0.250, 0.607] |
| stress | threshold_rule | strict_window_fa<=1 | gradual | 30 | 1991 | 0.163 [0.106, 0.213] | 0.200 [0.067, 0.333] |
| stress | threshold_rule | strict_window_fa<=1 | rapid | 28 | 1784 | 0.198 [0.122, 0.280] | 0.357 [0.214, 0.536] |
| stress | logistic_regression | raw (k=1) | gradual | 30 | 1991 | 0.265 [0.193, 0.341] | 0.900 [0.800, 1.000] |
| stress | logistic_regression | raw (k=1) | rapid | 28 | 1784 | 0.433 [0.333, 0.529] | 0.893 [0.786, 1.000] |
| stress | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 30 | 1991 | 0.109 [0.052, 0.171] | 0.267 [0.133, 0.400] |
| stress | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 28 | 1784 | 0.313 [0.219, 0.408] | 0.679 [0.500, 0.857] |
| stress | logistic_regression | strict_window_fa<=1 | gradual | 30 | 1991 | 0.041 [0.008, 0.080] | 0.067 [0.000, 0.167] |
| stress | logistic_regression | strict_window_fa<=1 | rapid | 28 | 1784 | 0.160 [0.089, 0.247] | 0.357 [0.179, 0.536] |
| stress | random_forest | raw (k=1) | gradual | 30 | 1991 | 0.188 [0.138, 0.252] | 0.800 [0.667, 0.900] |
| stress | random_forest | raw (k=1) | rapid | 28 | 1784 | 0.394 [0.304, 0.482] | 0.893 [0.786, 1.000] |
| stress | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 30 | 1991 | 0.139 [0.091, 0.201] | 0.467 [0.300, 0.651] |
| stress | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 28 | 1784 | 0.381 [0.293, 0.469] | 0.786 [0.643, 0.929] |
| stress | random_forest | strict_window_fa<=1 | gradual | 30 | 1991 | 0.074 [0.035, 0.116] | 0.233 [0.100, 0.400] |
| stress | random_forest | strict_window_fa<=1 | rapid | 28 | 1784 | 0.284 [0.199, 0.384] | 0.714 [0.536, 0.893] |
| broad_basin | threshold_rule | raw (k=1) | gradual | 20 | 1344 | 0.204 [0.140, 0.294] | 0.750 [0.524, 0.900] |
| broad_basin | threshold_rule | raw (k=1) | rapid | 20 | 1221 | 0.243 [0.124, 0.357] | 0.700 [0.500, 0.900] |
| broad_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 20 | 1344 | 0.204 [0.140, 0.294] | 0.500 [0.300, 0.700] |
| broad_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 20 | 1221 | 0.243 [0.124, 0.357] | 0.400 [0.200, 0.650] |
| broad_basin | threshold_rule | strict_window_fa<=1 | gradual | 20 | 1344 | 0.204 [0.140, 0.294] | 0.350 [0.150, 0.600] |
| broad_basin | threshold_rule | strict_window_fa<=1 | rapid | 20 | 1221 | 0.243 [0.124, 0.357] | 0.300 [0.124, 0.500] |
| broad_basin | logistic_regression | raw (k=1) | gradual | 20 | 1344 | 0.225 [0.123, 0.335] | 0.850 [0.650, 1.000] |
| broad_basin | logistic_regression | raw (k=1) | rapid | 20 | 1221 | 0.545 [0.420, 0.675] | 1.000 [1.000, 1.000] |
| broad_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 20 | 1344 | 0.075 [0.024, 0.161] | 0.200 [0.050, 0.350] |
| broad_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 20 | 1221 | 0.353 [0.239, 0.492] | 0.650 [0.424, 0.850] |
| broad_basin | logistic_regression | strict_window_fa<=1 | gradual | 20 | 1344 | 0.025 [0.003, 0.067] | 0.100 [0.000, 0.250] |
| broad_basin | logistic_regression | strict_window_fa<=1 | rapid | 20 | 1221 | 0.129 [0.063, 0.223] | 0.450 [0.250, 0.700] |
| broad_basin | random_forest | raw (k=1) | gradual | 20 | 1344 | 0.272 [0.190, 0.391] | 0.900 [0.750, 1.000] |
| broad_basin | random_forest | raw (k=1) | rapid | 20 | 1221 | 0.378 [0.263, 0.526] | 0.900 [0.750, 1.000] |
| broad_basin | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 20 | 1344 | 0.225 [0.143, 0.348] | 0.650 [0.450, 0.850] |
| broad_basin | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 20 | 1221 | 0.377 [0.257, 0.530] | 0.800 [0.600, 0.950] |
| broad_basin | random_forest | strict_window_fa<=1 | gradual | 20 | 1344 | 0.136 [0.069, 0.253] | 0.350 [0.150, 0.550] |
| broad_basin | random_forest | strict_window_fa<=1 | rapid | 20 | 1221 | 0.287 [0.183, 0.421] | 0.700 [0.500, 0.900] |
