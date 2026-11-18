# Gradual / rapid recall by snr_vs_imu_noise bin at the v3 operating points (SYNTHETIC / SIMULATION)

> **SYNTHETIC / SIMULATION** - all data are simulated; nothing here is validated on real data or field-ready.

Window recall = share of true gradual (rapid) windows predicted as that class by the model/operating point (before persistence). Run-level detection = share of gradual (rapid) runs with at least one alarm of that class after the regime's (k, m) persistence; it counts ANY correct alarm in the run, so it is always shown next to window recall and is never a substitute for it. Own-class rule: in the stress set an alarm of a co-occurring other class does not count. snr_vs_imu_noise = run's peak tilt / IMU noise (manifest).

Small cells (few runs) have wide intervals; N/A = no run in that bin. Operating-point regimes only (episode_fa<=1 and strict_window_fa<=1) plus raw for reference.

| split | model | regime | class | SNR bin | runs | windows | window recall | run-level detection |
|---|---|---|---|---|---|---|---|---|
| test | threshold_rule | raw (k=1) | gradual | <1 | 5 | 338 | 0.086 [0.000, 0.184] | 0.400 [0.000, 0.800] |
| test | threshold_rule | raw (k=1) | gradual | 1-2 | 5 | 332 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| test | threshold_rule | raw (k=1) | gradual | 2-5 | 2 | 143 | 0.049 [0.014, 0.085] | 1.000 [1.000, 1.000] |
| test | threshold_rule | raw (k=1) | gradual | >5 | 8 | 520 | 0.337 [0.312, 0.360] | 1.000 [1.000, 1.000] |
| test | threshold_rule | raw (k=1) | rapid | <1 | 7 | 405 | 0.030 [0.005, 0.061] | 0.571 [0.211, 0.932] |
| test | threshold_rule | raw (k=1) | rapid | 1-2 | 4 | 237 | 0.173 [0.000, 0.360] | 0.500 [0.000, 1.000] |
| test | threshold_rule | raw (k=1) | rapid | 2-5 | 4 | 234 | 0.316 [0.000, 0.602] | 0.500 [0.000, 1.000] |
| test | threshold_rule | raw (k=1) | rapid | >5 | 5 | 291 | 0.663 [0.586, 0.749] | 1.000 [1.000, 1.000] |
| test | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | <1 | 5 | 338 | 0.086 [0.000, 0.184] | 0.200 [0.000, 0.600] |
| test | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 332 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| test | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 2 | 143 | 0.049 [0.014, 0.085] | 0.000 [0.000, 0.000] |
| test | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | >5 | 8 | 520 | 0.337 [0.312, 0.360] | 1.000 [1.000, 1.000] |
| test | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | <1 | 7 | 405 | 0.030 [0.005, 0.061] | 0.000 [0.000, 0.000] |
| test | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 4 | 237 | 0.173 [0.000, 0.360] | 0.500 [0.000, 1.000] |
| test | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 234 | 0.316 [0.000, 0.602] | 0.500 [0.000, 1.000] |
| test | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | >5 | 5 | 291 | 0.663 [0.586, 0.749] | 1.000 [1.000, 1.000] |
| test | threshold_rule | strict_window_fa<=1 | gradual | <1 | 5 | 338 | 0.086 [0.000, 0.184] | 0.000 [0.000, 0.000] |
| test | threshold_rule | strict_window_fa<=1 | gradual | 1-2 | 5 | 332 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| test | threshold_rule | strict_window_fa<=1 | gradual | 2-5 | 2 | 143 | 0.049 [0.014, 0.085] | 0.000 [0.000, 0.000] |
| test | threshold_rule | strict_window_fa<=1 | gradual | >5 | 8 | 520 | 0.337 [0.312, 0.360] | 0.750 [0.375, 1.000] |
| test | threshold_rule | strict_window_fa<=1 | rapid | <1 | 7 | 405 | 0.030 [0.005, 0.061] | 0.000 [0.000, 0.000] |
| test | threshold_rule | strict_window_fa<=1 | rapid | 1-2 | 4 | 237 | 0.173 [0.000, 0.360] | 0.250 [0.000, 0.750] |
| test | threshold_rule | strict_window_fa<=1 | rapid | 2-5 | 4 | 234 | 0.316 [0.000, 0.602] | 0.500 [0.000, 1.000] |
| test | threshold_rule | strict_window_fa<=1 | rapid | >5 | 5 | 291 | 0.663 [0.586, 0.749] | 1.000 [1.000, 1.000] |
| test | logistic_regression | raw (k=1) | gradual | <1 | 5 | 338 | 0.346 [0.088, 0.603] | 0.800 [0.400, 1.000] |
| test | logistic_regression | raw (k=1) | gradual | 1-2 | 5 | 332 | 0.081 [0.009, 0.147] | 0.600 [0.200, 1.000] |
| test | logistic_regression | raw (k=1) | gradual | 2-5 | 2 | 143 | 0.147 [0.056, 0.236] | 1.000 [1.000, 1.000] |
| test | logistic_regression | raw (k=1) | gradual | >5 | 8 | 520 | 0.302 [0.124, 0.517] | 0.875 [0.625, 1.000] |
| test | logistic_regression | raw (k=1) | rapid | <1 | 7 | 405 | 0.136 [0.065, 0.200] | 1.000 [1.000, 1.000] |
| test | logistic_regression | raw (k=1) | rapid | 1-2 | 4 | 237 | 0.300 [0.062, 0.599] | 1.000 [1.000, 1.000] |
| test | logistic_regression | raw (k=1) | rapid | 2-5 | 4 | 234 | 0.500 [0.187, 0.847] | 1.000 [1.000, 1.000] |
| test | logistic_regression | raw (k=1) | rapid | >5 | 5 | 291 | 0.540 [0.221, 0.845] | 1.000 [1.000, 1.000] |
| test | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | <1 | 5 | 338 | 0.056 [0.003, 0.112] | 0.200 [0.000, 0.600] |
| test | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 332 | 0.003 [0.000, 0.007] | 0.000 [0.000, 0.000] |
| test | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 2 | 143 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| test | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | >5 | 8 | 520 | 0.179 [0.045, 0.361] | 0.625 [0.250, 0.875] |
| test | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | <1 | 7 | 405 | 0.002 [0.000, 0.008] | 0.000 [0.000, 0.000] |
| test | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 4 | 237 | 0.063 [0.000, 0.143] | 0.250 [0.000, 0.750] |
| test | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 234 | 0.325 [0.049, 0.631] | 0.500 [0.000, 1.000] |
| test | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | >5 | 5 | 291 | 0.522 [0.196, 0.828] | 0.800 [0.400, 1.000] |
| test | logistic_regression | strict_window_fa<=1 | gradual | <1 | 5 | 338 | 0.003 [0.000, 0.009] | 0.000 [0.000, 0.000] |
| test | logistic_regression | strict_window_fa<=1 | gradual | 1-2 | 5 | 332 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| test | logistic_regression | strict_window_fa<=1 | gradual | 2-5 | 2 | 143 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| test | logistic_regression | strict_window_fa<=1 | gradual | >5 | 8 | 520 | 0.090 [0.002, 0.236] | 0.250 [0.000, 0.625] |
| test | logistic_regression | strict_window_fa<=1 | rapid | <1 | 7 | 405 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| test | logistic_regression | strict_window_fa<=1 | rapid | 1-2 | 4 | 237 | 0.008 [0.000, 0.015] | 0.000 [0.000, 0.000] |
| test | logistic_regression | strict_window_fa<=1 | rapid | 2-5 | 4 | 234 | 0.175 [0.000, 0.495] | 0.500 [0.000, 1.000] |
| test | logistic_regression | strict_window_fa<=1 | rapid | >5 | 5 | 291 | 0.419 [0.058, 0.788] | 0.600 [0.200, 1.000] |
| test | random_forest | raw (k=1) | gradual | <1 | 5 | 338 | 0.151 [0.052, 0.254] | 0.800 [0.400, 1.000] |
| test | random_forest | raw (k=1) | gradual | 1-2 | 5 | 332 | 0.111 [0.006, 0.258] | 0.600 [0.200, 1.000] |
| test | random_forest | raw (k=1) | gradual | 2-5 | 2 | 143 | 0.014 [0.000, 0.028] | 0.500 [0.000, 1.000] |
| test | random_forest | raw (k=1) | gradual | >5 | 8 | 520 | 0.352 [0.175, 0.548] | 0.875 [0.625, 1.000] |
| test | random_forest | raw (k=1) | rapid | <1 | 7 | 405 | 0.020 [0.002, 0.046] | 0.429 [0.143, 0.714] |
| test | random_forest | raw (k=1) | rapid | 1-2 | 4 | 237 | 0.198 [0.010, 0.465] | 0.750 [0.250, 1.000] |
| test | random_forest | raw (k=1) | rapid | 2-5 | 4 | 234 | 0.397 [0.008, 0.829] | 0.750 [0.250, 1.000] |
| test | random_forest | raw (k=1) | rapid | >5 | 5 | 291 | 0.660 [0.281, 0.929] | 0.800 [0.400, 1.000] |
| test | random_forest | episode_fa<=1 (k=3,m=3) | gradual | <1 | 5 | 338 | 0.041 [0.014, 0.072] | 0.000 [0.000, 0.000] |
| test | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 332 | 0.093 [0.003, 0.244] | 0.400 [0.000, 0.800] |
| test | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 2 | 143 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| test | random_forest | episode_fa<=1 (k=3,m=3) | gradual | >5 | 8 | 520 | 0.319 [0.163, 0.498] | 0.750 [0.434, 1.000] |
| test | random_forest | episode_fa<=1 (k=3,m=3) | rapid | <1 | 7 | 405 | 0.017 [0.002, 0.043] | 0.143 [0.000, 0.429] |
| test | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 4 | 237 | 0.177 [0.009, 0.419] | 0.250 [0.000, 0.750] |
| test | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 234 | 0.397 [0.008, 0.829] | 0.500 [0.000, 1.000] |
| test | random_forest | episode_fa<=1 (k=3,m=3) | rapid | >5 | 5 | 291 | 0.649 [0.270, 0.929] | 0.800 [0.400, 1.000] |
| test | random_forest | strict_window_fa<=1 | gradual | <1 | 5 | 338 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| test | random_forest | strict_window_fa<=1 | gradual | 1-2 | 5 | 332 | 0.048 [0.000, 0.149] | 0.200 [0.000, 0.600] |
| test | random_forest | strict_window_fa<=1 | gradual | 2-5 | 2 | 143 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| test | random_forest | strict_window_fa<=1 | gradual | >5 | 8 | 520 | 0.256 [0.123, 0.409] | 0.625 [0.250, 1.000] |
| test | random_forest | strict_window_fa<=1 | rapid | <1 | 7 | 405 | 0.002 [0.000, 0.008] | 0.000 [0.000, 0.000] |
| test | random_forest | strict_window_fa<=1 | rapid | 1-2 | 4 | 237 | 0.034 [0.000, 0.086] | 0.000 [0.000, 0.000] |
| test | random_forest | strict_window_fa<=1 | rapid | 2-5 | 4 | 234 | 0.350 [0.008, 0.730] | 0.500 [0.000, 1.000] |
| test | random_forest | strict_window_fa<=1 | rapid | >5 | 5 | 291 | 0.570 [0.200, 0.912] | 0.600 [0.200, 1.000] |
| shifted_test | threshold_rule | raw (k=1) | gradual | <1 | 7 | 494 | 0.247 [0.198, 0.302] | 1.000 [1.000, 1.000] |
| shifted_test | threshold_rule | raw (k=1) | gradual | 1-2 | 3 | 193 | 0.285 [0.226, 0.322] | 1.000 [1.000, 1.000] |
| shifted_test | threshold_rule | raw (k=1) | gradual | 2-5 | 2 | 145 | 0.372 [0.333, 0.414] | 1.000 [1.000, 1.000] |
| shifted_test | threshold_rule | raw (k=1) | gradual | >5 | 3 | 203 | 0.355 [0.328, 0.406] | 1.000 [1.000, 1.000] |
| shifted_test | threshold_rule | raw (k=1) | rapid | <1 | 6 | 354 | 0.299 [0.159, 0.402] | 1.000 [1.000, 1.000] |
| shifted_test | threshold_rule | raw (k=1) | rapid | 1-2 | 3 | 206 | 0.136 [0.059, 0.178] | 1.000 [1.000, 1.000] |
| shifted_test | threshold_rule | raw (k=1) | rapid | 2-5 | 4 | 255 | 0.710 [0.559, 0.826] | 1.000 [1.000, 1.000] |
| shifted_test | threshold_rule | raw (k=1) | rapid | >5 | 2 | 101 | 0.653 [0.588, 0.720] | 1.000 [1.000, 1.000] |
| shifted_test | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | <1 | 7 | 494 | 0.247 [0.198, 0.302] | 0.857 [0.571, 1.000] |
| shifted_test | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 3 | 193 | 0.285 [0.226, 0.322] | 0.667 [0.333, 1.000] |
| shifted_test | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 2 | 145 | 0.372 [0.333, 0.414] | 1.000 [1.000, 1.000] |
| shifted_test | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | >5 | 3 | 203 | 0.355 [0.328, 0.406] | 1.000 [1.000, 1.000] |
| shifted_test | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | <1 | 6 | 354 | 0.299 [0.159, 0.402] | 0.500 [0.167, 0.833] |
| shifted_test | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 3 | 206 | 0.136 [0.059, 0.178] | 0.333 [0.000, 0.667] |
| shifted_test | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 255 | 0.710 [0.559, 0.826] | 1.000 [1.000, 1.000] |
| shifted_test | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | >5 | 2 | 101 | 0.653 [0.588, 0.720] | 1.000 [1.000, 1.000] |
| shifted_test | threshold_rule | strict_window_fa<=1 | gradual | <1 | 7 | 494 | 0.247 [0.198, 0.302] | 0.143 [0.000, 0.429] |
| shifted_test | threshold_rule | strict_window_fa<=1 | gradual | 1-2 | 3 | 193 | 0.285 [0.226, 0.322] | 0.333 [0.000, 0.667] |
| shifted_test | threshold_rule | strict_window_fa<=1 | gradual | 2-5 | 2 | 145 | 0.372 [0.333, 0.414] | 0.500 [0.000, 1.000] |
| shifted_test | threshold_rule | strict_window_fa<=1 | gradual | >5 | 3 | 203 | 0.355 [0.328, 0.406] | 1.000 [1.000, 1.000] |
| shifted_test | threshold_rule | strict_window_fa<=1 | rapid | <1 | 6 | 354 | 0.299 [0.159, 0.402] | 0.167 [0.000, 0.500] |
| shifted_test | threshold_rule | strict_window_fa<=1 | rapid | 1-2 | 3 | 206 | 0.136 [0.059, 0.178] | 0.000 [0.000, 0.000] |
| shifted_test | threshold_rule | strict_window_fa<=1 | rapid | 2-5 | 4 | 255 | 0.710 [0.559, 0.826] | 1.000 [1.000, 1.000] |
| shifted_test | threshold_rule | strict_window_fa<=1 | rapid | >5 | 2 | 101 | 0.653 [0.588, 0.720] | 1.000 [1.000, 1.000] |
| shifted_test | logistic_regression | raw (k=1) | gradual | <1 | 7 | 494 | 0.488 [0.366, 0.598] | 1.000 [1.000, 1.000] |
| shifted_test | logistic_regression | raw (k=1) | gradual | 1-2 | 3 | 193 | 0.554 [0.355, 0.661] | 1.000 [1.000, 1.000] |
| shifted_test | logistic_regression | raw (k=1) | gradual | 2-5 | 2 | 145 | 0.276 [0.200, 0.347] | 1.000 [1.000, 1.000] |
| shifted_test | logistic_regression | raw (k=1) | gradual | >5 | 3 | 203 | 0.379 [0.055, 0.836] | 1.000 [1.000, 1.000] |
| shifted_test | logistic_regression | raw (k=1) | rapid | <1 | 6 | 354 | 0.136 [0.023, 0.279] | 0.833 [0.500, 1.000] |
| shifted_test | logistic_regression | raw (k=1) | rapid | 1-2 | 3 | 206 | 0.345 [0.185, 0.632] | 1.000 [1.000, 1.000] |
| shifted_test | logistic_regression | raw (k=1) | rapid | 2-5 | 4 | 255 | 0.263 [0.133, 0.465] | 1.000 [1.000, 1.000] |
| shifted_test | logistic_regression | raw (k=1) | rapid | >5 | 2 | 101 | 0.277 [0.020, 0.529] | 1.000 [1.000, 1.000] |
| shifted_test | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | <1 | 7 | 494 | 0.103 [0.045, 0.161] | 0.286 [0.000, 0.646] |
| shifted_test | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 3 | 193 | 0.223 [0.048, 0.319] | 0.667 [0.333, 1.000] |
| shifted_test | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 2 | 145 | 0.041 [0.013, 0.071] | 0.000 [0.000, 0.000] |
| shifted_test | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | >5 | 3 | 203 | 0.266 [0.014, 0.689] | 0.667 [0.333, 1.000] |
| shifted_test | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | <1 | 6 | 354 | 0.037 [0.000, 0.091] | 0.333 [0.000, 0.754] |
| shifted_test | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 3 | 206 | 0.160 [0.062, 0.324] | 0.667 [0.000, 1.000] |
| shifted_test | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 255 | 0.196 [0.060, 0.373] | 0.500 [0.000, 1.000] |
| shifted_test | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | >5 | 2 | 101 | 0.218 [0.000, 0.431] | 0.500 [0.000, 1.000] |
| shifted_test | logistic_regression | strict_window_fa<=1 | gradual | <1 | 7 | 494 | 0.018 [0.004, 0.035] | 0.000 [0.000, 0.000] |
| shifted_test | logistic_regression | strict_window_fa<=1 | gradual | 1-2 | 3 | 193 | 0.067 [0.000, 0.111] | 0.000 [0.000, 0.000] |
| shifted_test | logistic_regression | strict_window_fa<=1 | gradual | 2-5 | 2 | 145 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| shifted_test | logistic_regression | strict_window_fa<=1 | gradual | >5 | 3 | 203 | 0.118 [0.000, 0.377] | 0.333 [0.000, 0.667] |
| shifted_test | logistic_regression | strict_window_fa<=1 | rapid | <1 | 6 | 354 | 0.014 [0.000, 0.033] | 0.000 [0.000, 0.000] |
| shifted_test | logistic_regression | strict_window_fa<=1 | rapid | 1-2 | 3 | 206 | 0.049 [0.041, 0.059] | 0.000 [0.000, 0.000] |
| shifted_test | logistic_regression | strict_window_fa<=1 | rapid | 2-5 | 4 | 255 | 0.047 [0.007, 0.100] | 0.250 [0.000, 0.750] |
| shifted_test | logistic_regression | strict_window_fa<=1 | rapid | >5 | 2 | 101 | 0.069 [0.000, 0.137] | 0.000 [0.000, 0.000] |
| shifted_test | random_forest | raw (k=1) | gradual | <1 | 7 | 494 | 0.372 [0.238, 0.472] | 1.000 [1.000, 1.000] |
| shifted_test | random_forest | raw (k=1) | gradual | 1-2 | 3 | 193 | 0.596 [0.226, 0.780] | 1.000 [1.000, 1.000] |
| shifted_test | random_forest | raw (k=1) | gradual | 2-5 | 2 | 145 | 0.386 [0.286, 0.480] | 1.000 [1.000, 1.000] |
| shifted_test | random_forest | raw (k=1) | gradual | >5 | 3 | 203 | 0.448 [0.274, 0.787] | 1.000 [1.000, 1.000] |
| shifted_test | random_forest | raw (k=1) | rapid | <1 | 6 | 354 | 0.034 [0.000, 0.104] | 0.333 [0.000, 0.667] |
| shifted_test | random_forest | raw (k=1) | rapid | 1-2 | 3 | 206 | 0.155 [0.055, 0.309] | 1.000 [1.000, 1.000] |
| shifted_test | random_forest | raw (k=1) | rapid | 2-5 | 4 | 255 | 0.184 [0.000, 0.465] | 0.500 [0.000, 1.000] |
| shifted_test | random_forest | raw (k=1) | rapid | >5 | 2 | 101 | 0.376 [0.040, 0.706] | 1.000 [1.000, 1.000] |
| shifted_test | random_forest | episode_fa<=1 (k=3,m=3) | gradual | <1 | 7 | 494 | 0.164 [0.101, 0.222] | 0.714 [0.429, 1.000] |
| shifted_test | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 3 | 193 | 0.523 [0.065, 0.780] | 0.667 [0.333, 1.000] |
| shifted_test | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 2 | 145 | 0.117 [0.027, 0.214] | 0.500 [0.000, 1.000] |
| shifted_test | random_forest | episode_fa<=1 (k=3,m=3) | gradual | >5 | 3 | 203 | 0.399 [0.246, 0.754] | 1.000 [1.000, 1.000] |
| shifted_test | random_forest | episode_fa<=1 (k=3,m=3) | rapid | <1 | 6 | 354 | 0.023 [0.000, 0.075] | 0.167 [0.000, 0.500] |
| shifted_test | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 3 | 206 | 0.126 [0.027, 0.265] | 0.667 [0.333, 1.000] |
| shifted_test | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 4 | 255 | 0.184 [0.000, 0.465] | 0.500 [0.000, 1.000] |
| shifted_test | random_forest | episode_fa<=1 (k=3,m=3) | rapid | >5 | 2 | 101 | 0.356 [0.020, 0.686] | 0.500 [0.000, 1.000] |
| shifted_test | random_forest | strict_window_fa<=1 | gradual | <1 | 7 | 494 | 0.040 [0.008, 0.082] | 0.286 [0.000, 0.646] |
| shifted_test | random_forest | strict_window_fa<=1 | gradual | 1-2 | 3 | 193 | 0.316 [0.000, 0.576] | 0.667 [0.333, 1.000] |
| shifted_test | random_forest | strict_window_fa<=1 | gradual | 2-5 | 2 | 145 | 0.048 [0.000, 0.100] | 0.500 [0.000, 1.000] |
| shifted_test | random_forest | strict_window_fa<=1 | gradual | >5 | 3 | 203 | 0.355 [0.174, 0.738] | 1.000 [1.000, 1.000] |
| shifted_test | random_forest | strict_window_fa<=1 | rapid | <1 | 6 | 354 | 0.003 [0.000, 0.009] | 0.000 [0.000, 0.000] |
| shifted_test | random_forest | strict_window_fa<=1 | rapid | 1-2 | 3 | 206 | 0.083 [0.000, 0.206] | 0.333 [0.000, 0.667] |
| shifted_test | random_forest | strict_window_fa<=1 | rapid | 2-5 | 4 | 255 | 0.180 [0.000, 0.465] | 0.500 [0.000, 1.000] |
| shifted_test | random_forest | strict_window_fa<=1 | rapid | >5 | 2 | 101 | 0.277 [0.020, 0.529] | 0.500 [0.000, 1.000] |
| stress | threshold_rule | raw (k=1) | gradual | <1 | 10 | 668 | 0.060 [0.021, 0.107] | 0.600 [0.300, 0.900] |
| stress | threshold_rule | raw (k=1) | gradual | 1-2 | 5 | 334 | 0.138 [0.057, 0.220] | 0.800 [0.400, 1.000] |
| stress | threshold_rule | raw (k=1) | gradual | 2-5 | 6 | 392 | 0.145 [0.056, 0.241] | 0.667 [0.246, 1.000] |
| stress | threshold_rule | raw (k=1) | gradual | >5 | 9 | 597 | 0.303 [0.199, 0.400] | 0.889 [0.667, 1.000] |
| stress | threshold_rule | raw (k=1) | rapid | <1 | 7 | 444 | 0.086 [0.000, 0.196] | 0.286 [0.000, 0.571] |
| stress | threshold_rule | raw (k=1) | rapid | 1-2 | 5 | 320 | 0.072 [0.027, 0.107] | 0.800 [0.400, 1.000] |
| stress | threshold_rule | raw (k=1) | rapid | 2-5 | 9 | 571 | 0.189 [0.066, 0.361] | 0.556 [0.222, 0.778] |
| stress | threshold_rule | raw (k=1) | rapid | >5 | 7 | 449 | 0.410 [0.268, 0.523] | 0.857 [0.571, 1.000] |
| stress | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.060 [0.021, 0.107] | 0.100 [0.000, 0.300] |
| stress | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 334 | 0.138 [0.057, 0.220] | 0.400 [0.000, 0.800] |
| stress | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 392 | 0.145 [0.056, 0.241] | 0.333 [0.000, 0.667] |
| stress | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 597 | 0.303 [0.199, 0.400] | 0.889 [0.667, 1.000] |
| stress | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | <1 | 7 | 444 | 0.086 [0.000, 0.196] | 0.286 [0.000, 0.571] |
| stress | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 5 | 320 | 0.072 [0.027, 0.107] | 0.000 [0.000, 0.000] |
| stress | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 9 | 571 | 0.189 [0.066, 0.361] | 0.444 [0.111, 0.778] |
| stress | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | >5 | 7 | 449 | 0.410 [0.268, 0.523] | 0.857 [0.571, 1.000] |
| stress | threshold_rule | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.060 [0.021, 0.107] | 0.000 [0.000, 0.000] |
| stress | threshold_rule | strict_window_fa<=1 | gradual | 1-2 | 5 | 334 | 0.138 [0.057, 0.220] | 0.000 [0.000, 0.000] |
| stress | threshold_rule | strict_window_fa<=1 | gradual | 2-5 | 6 | 392 | 0.145 [0.056, 0.241] | 0.000 [0.000, 0.000] |
| stress | threshold_rule | strict_window_fa<=1 | gradual | >5 | 9 | 597 | 0.303 [0.199, 0.400] | 0.667 [0.333, 1.000] |
| stress | threshold_rule | strict_window_fa<=1 | rapid | <1 | 7 | 444 | 0.086 [0.000, 0.196] | 0.143 [0.000, 0.429] |
| stress | threshold_rule | strict_window_fa<=1 | rapid | 1-2 | 5 | 320 | 0.072 [0.027, 0.107] | 0.000 [0.000, 0.000] |
| stress | threshold_rule | strict_window_fa<=1 | rapid | 2-5 | 9 | 571 | 0.189 [0.066, 0.361] | 0.333 [0.000, 0.667] |
| stress | threshold_rule | strict_window_fa<=1 | rapid | >5 | 7 | 449 | 0.410 [0.268, 0.523] | 0.857 [0.571, 1.000] |
| stress | logistic_regression | raw (k=1) | gradual | <1 | 10 | 668 | 0.177 [0.127, 0.236] | 1.000 [1.000, 1.000] |
| stress | logistic_regression | raw (k=1) | gradual | 1-2 | 5 | 334 | 0.371 [0.296, 0.443] | 1.000 [1.000, 1.000] |
| stress | logistic_regression | raw (k=1) | gradual | 2-5 | 6 | 392 | 0.207 [0.080, 0.349] | 1.000 [1.000, 1.000] |
| stress | logistic_regression | raw (k=1) | gradual | >5 | 9 | 597 | 0.342 [0.151, 0.539] | 0.667 [0.333, 0.947] |
| stress | logistic_regression | raw (k=1) | rapid | <1 | 7 | 444 | 0.324 [0.134, 0.461] | 1.000 [1.000, 1.000] |
| stress | logistic_regression | raw (k=1) | rapid | 1-2 | 5 | 320 | 0.412 [0.199, 0.530] | 0.800 [0.400, 1.000] |
| stress | logistic_regression | raw (k=1) | rapid | 2-5 | 9 | 571 | 0.433 [0.218, 0.601] | 0.778 [0.556, 1.000] |
| stress | logistic_regression | raw (k=1) | rapid | >5 | 7 | 449 | 0.557 [0.286, 0.824] | 1.000 [1.000, 1.000] |
| stress | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.027 [0.013, 0.044] | 0.100 [0.000, 0.300] |
| stress | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 334 | 0.102 [0.024, 0.216] | 0.400 [0.000, 0.800] |
| stress | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 392 | 0.071 [0.008, 0.161] | 0.167 [0.000, 0.500] |
| stress | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 597 | 0.231 [0.069, 0.411] | 0.444 [0.111, 0.778] |
| stress | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | <1 | 7 | 444 | 0.153 [0.043, 0.256] | 0.429 [0.143, 0.857] |
| stress | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 5 | 320 | 0.225 [0.092, 0.301] | 0.800 [0.400, 1.000] |
| stress | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 9 | 571 | 0.306 [0.145, 0.470] | 0.778 [0.556, 1.000] |
| stress | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | >5 | 7 | 449 | 0.541 [0.273, 0.814] | 0.714 [0.429, 1.000] |
| stress | logistic_regression | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.004 [0.000, 0.012] | 0.000 [0.000, 0.000] |
| stress | logistic_regression | strict_window_fa<=1 | gradual | 1-2 | 5 | 334 | 0.021 [0.000, 0.043] | 0.000 [0.000, 0.000] |
| stress | logistic_regression | strict_window_fa<=1 | gradual | 2-5 | 6 | 392 | 0.013 [0.002, 0.028] | 0.000 [0.000, 0.000] |
| stress | logistic_regression | strict_window_fa<=1 | gradual | >5 | 9 | 597 | 0.112 [0.011, 0.253] | 0.222 [0.000, 0.556] |
| stress | logistic_regression | strict_window_fa<=1 | rapid | <1 | 7 | 444 | 0.038 [0.004, 0.087] | 0.143 [0.000, 0.429] |
| stress | logistic_regression | strict_window_fa<=1 | rapid | 1-2 | 5 | 320 | 0.075 [0.018, 0.123] | 0.200 [0.000, 0.600] |
| stress | logistic_regression | strict_window_fa<=1 | rapid | 2-5 | 9 | 571 | 0.116 [0.027, 0.228] | 0.333 [0.000, 0.667] |
| stress | logistic_regression | strict_window_fa<=1 | rapid | >5 | 7 | 449 | 0.396 [0.149, 0.651] | 0.714 [0.429, 1.000] |
| stress | random_forest | raw (k=1) | gradual | <1 | 10 | 668 | 0.123 [0.063, 0.189] | 0.800 [0.600, 1.000] |
| stress | random_forest | raw (k=1) | gradual | 1-2 | 5 | 334 | 0.362 [0.229, 0.479] | 1.000 [1.000, 1.000] |
| stress | random_forest | raw (k=1) | gradual | 2-5 | 6 | 392 | 0.176 [0.050, 0.332] | 0.833 [0.500, 1.000] |
| stress | random_forest | raw (k=1) | gradual | >5 | 9 | 597 | 0.173 [0.081, 0.267] | 0.667 [0.333, 0.947] |
| stress | random_forest | raw (k=1) | rapid | <1 | 7 | 444 | 0.264 [0.099, 0.371] | 1.000 [1.000, 1.000] |
| stress | random_forest | raw (k=1) | rapid | 1-2 | 5 | 320 | 0.228 [0.083, 0.323] | 0.800 [0.400, 1.000] |
| stress | random_forest | raw (k=1) | rapid | 2-5 | 9 | 571 | 0.345 [0.165, 0.527] | 0.778 [0.556, 1.000] |
| stress | random_forest | raw (k=1) | rapid | >5 | 7 | 449 | 0.704 [0.530, 0.844] | 1.000 [1.000, 1.000] |
| stress | random_forest | episode_fa<=1 (k=3,m=3) | gradual | <1 | 10 | 668 | 0.072 [0.025, 0.123] | 0.300 [0.000, 0.600] |
| stress | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 5 | 334 | 0.293 [0.115, 0.464] | 0.600 [0.200, 1.000] |
| stress | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 6 | 392 | 0.117 [0.028, 0.230] | 0.500 [0.167, 0.833] |
| stress | random_forest | episode_fa<=1 (k=3,m=3) | gradual | >5 | 9 | 597 | 0.142 [0.051, 0.242] | 0.556 [0.222, 0.836] |
| stress | random_forest | episode_fa<=1 (k=3,m=3) | rapid | <1 | 7 | 444 | 0.250 [0.074, 0.366] | 0.571 [0.286, 0.857] |
| stress | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 5 | 320 | 0.216 [0.078, 0.309] | 0.800 [0.400, 1.000] |
| stress | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 9 | 571 | 0.333 [0.164, 0.502] | 0.778 [0.556, 1.000] |
| stress | random_forest | episode_fa<=1 (k=3,m=3) | rapid | >5 | 7 | 449 | 0.688 [0.527, 0.836] | 1.000 [1.000, 1.000] |
| stress | random_forest | strict_window_fa<=1 | gradual | <1 | 10 | 668 | 0.009 [0.000, 0.021] | 0.000 [0.000, 0.000] |
| stress | random_forest | strict_window_fa<=1 | gradual | 1-2 | 5 | 334 | 0.144 [0.013, 0.306] | 0.400 [0.000, 0.800] |
| stress | random_forest | strict_window_fa<=1 | gradual | 2-5 | 6 | 392 | 0.054 [0.000, 0.131] | 0.333 [0.000, 0.667] |
| stress | random_forest | strict_window_fa<=1 | gradual | >5 | 9 | 597 | 0.122 [0.037, 0.220] | 0.333 [0.000, 0.614] |
| stress | random_forest | strict_window_fa<=1 | rapid | <1 | 7 | 444 | 0.164 [0.040, 0.250] | 0.571 [0.286, 0.857] |
| stress | random_forest | strict_window_fa<=1 | rapid | 1-2 | 5 | 320 | 0.134 [0.043, 0.205] | 0.600 [0.200, 1.000] |
| stress | random_forest | strict_window_fa<=1 | rapid | 2-5 | 9 | 571 | 0.215 [0.076, 0.364] | 0.667 [0.333, 0.947] |
| stress | random_forest | strict_window_fa<=1 | rapid | >5 | 7 | 449 | 0.597 [0.384, 0.762] | 1.000 [1.000, 1.000] |
| broad_basin | threshold_rule | raw (k=1) | gradual | <1 | 5 | 353 | 0.110 [0.019, 0.191] | 0.600 [0.200, 1.000] |
| broad_basin | threshold_rule | raw (k=1) | gradual | 1-2 | 6 | 398 | 0.055 [0.003, 0.134] | 0.500 [0.167, 0.833] |
| broad_basin | threshold_rule | raw (k=1) | gradual | 2-5 | 3 | 199 | 0.281 [0.145, 0.392] | 1.000 [1.000, 1.000] |
| broad_basin | threshold_rule | raw (k=1) | gradual | >5 | 6 | 394 | 0.398 [0.267, 0.489] | 1.000 [1.000, 1.000] |
| broad_basin | threshold_rule | raw (k=1) | rapid | <1 | 6 | 373 | 0.102 [0.045, 0.181] | 0.833 [0.500, 1.000] |
| broad_basin | threshold_rule | raw (k=1) | rapid | 1-2 | 3 | 175 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| broad_basin | threshold_rule | raw (k=1) | rapid | 2-5 | 5 | 296 | 0.125 [0.003, 0.246] | 0.600 [0.200, 1.000] |
| broad_basin | threshold_rule | raw (k=1) | rapid | >5 | 6 | 377 | 0.589 [0.344, 0.743] | 1.000 [1.000, 1.000] |
| broad_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | <1 | 5 | 353 | 0.110 [0.019, 0.191] | 0.200 [0.000, 0.600] |
| broad_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 6 | 398 | 0.055 [0.003, 0.134] | 0.167 [0.000, 0.500] |
| broad_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 3 | 199 | 0.281 [0.145, 0.392] | 1.000 [1.000, 1.000] |
| broad_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | >5 | 6 | 394 | 0.398 [0.267, 0.489] | 0.833 [0.500, 1.000] |
| broad_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | <1 | 6 | 373 | 0.102 [0.045, 0.181] | 0.333 [0.000, 0.667] |
| broad_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 3 | 175 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| broad_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 5 | 296 | 0.125 [0.003, 0.246] | 0.200 [0.000, 0.600] |
| broad_basin | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | >5 | 6 | 377 | 0.589 [0.344, 0.743] | 0.833 [0.500, 1.000] |
| broad_basin | threshold_rule | strict_window_fa<=1 | gradual | <1 | 5 | 353 | 0.110 [0.019, 0.191] | 0.000 [0.000, 0.000] |
| broad_basin | threshold_rule | strict_window_fa<=1 | gradual | 1-2 | 6 | 398 | 0.055 [0.003, 0.134] | 0.000 [0.000, 0.000] |
| broad_basin | threshold_rule | strict_window_fa<=1 | gradual | 2-5 | 3 | 199 | 0.281 [0.145, 0.392] | 0.667 [0.333, 1.000] |
| broad_basin | threshold_rule | strict_window_fa<=1 | gradual | >5 | 6 | 394 | 0.398 [0.267, 0.489] | 0.833 [0.500, 1.000] |
| broad_basin | threshold_rule | strict_window_fa<=1 | rapid | <1 | 6 | 373 | 0.102 [0.045, 0.181] | 0.000 [0.000, 0.000] |
| broad_basin | threshold_rule | strict_window_fa<=1 | rapid | 1-2 | 3 | 175 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| broad_basin | threshold_rule | strict_window_fa<=1 | rapid | 2-5 | 5 | 296 | 0.125 [0.003, 0.246] | 0.200 [0.000, 0.600] |
| broad_basin | threshold_rule | strict_window_fa<=1 | rapid | >5 | 6 | 377 | 0.589 [0.344, 0.743] | 0.833 [0.500, 1.000] |
| broad_basin | logistic_regression | raw (k=1) | gradual | <1 | 5 | 353 | 0.363 [0.122, 0.560] | 0.800 [0.400, 1.000] |
| broad_basin | logistic_regression | raw (k=1) | gradual | 1-2 | 6 | 398 | 0.186 [0.059, 0.316] | 1.000 [1.000, 1.000] |
| broad_basin | logistic_regression | raw (k=1) | gradual | 2-5 | 3 | 199 | 0.276 [0.014, 0.839] | 1.000 [1.000, 1.000] |
| broad_basin | logistic_regression | raw (k=1) | gradual | >5 | 6 | 394 | 0.117 [0.008, 0.306] | 0.667 [0.167, 1.000] |
| broad_basin | logistic_regression | raw (k=1) | rapid | <1 | 6 | 373 | 0.434 [0.283, 0.544] | 1.000 [1.000, 1.000] |
| broad_basin | logistic_regression | raw (k=1) | rapid | 1-2 | 3 | 175 | 0.400 [0.045, 0.915] | 1.000 [1.000, 1.000] |
| broad_basin | logistic_regression | raw (k=1) | rapid | 2-5 | 5 | 296 | 0.747 [0.611, 0.888] | 1.000 [1.000, 1.000] |
| broad_basin | logistic_regression | raw (k=1) | rapid | >5 | 6 | 377 | 0.562 [0.312, 0.816] | 1.000 [1.000, 1.000] |
| broad_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | <1 | 5 | 353 | 0.079 [0.007, 0.147] | 0.400 [0.000, 0.800] |
| broad_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 6 | 398 | 0.018 [0.003, 0.035] | 0.000 [0.000, 0.000] |
| broad_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 3 | 199 | 0.196 [0.000, 0.661] | 0.333 [0.000, 1.000] |
| broad_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | >5 | 6 | 394 | 0.069 [0.002, 0.197] | 0.167 [0.000, 0.500] |
| broad_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | <1 | 6 | 373 | 0.123 [0.063, 0.172] | 0.333 [0.000, 0.667] |
| broad_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 3 | 175 | 0.194 [0.000, 0.508] | 0.333 [0.000, 0.667] |
| broad_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 5 | 296 | 0.520 [0.309, 0.739] | 0.800 [0.400, 1.000] |
| broad_basin | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | >5 | 6 | 377 | 0.523 [0.296, 0.761] | 1.000 [1.000, 1.000] |
| broad_basin | logistic_regression | strict_window_fa<=1 | gradual | <1 | 5 | 353 | 0.014 [0.003, 0.023] | 0.000 [0.000, 0.000] |
| broad_basin | logistic_regression | strict_window_fa<=1 | gradual | 1-2 | 6 | 398 | 0.000 [0.000, 0.000] | 0.000 [0.000, 0.000] |
| broad_basin | logistic_regression | strict_window_fa<=1 | gradual | 2-5 | 3 | 199 | 0.095 [0.000, 0.339] | 0.333 [0.000, 1.000] |
| broad_basin | logistic_regression | strict_window_fa<=1 | gradual | >5 | 6 | 394 | 0.025 [0.000, 0.078] | 0.167 [0.000, 0.500] |
| broad_basin | logistic_regression | strict_window_fa<=1 | rapid | <1 | 6 | 373 | 0.021 [0.003, 0.056] | 0.167 [0.000, 0.500] |
| broad_basin | logistic_regression | strict_window_fa<=1 | rapid | 1-2 | 3 | 175 | 0.063 [0.000, 0.169] | 0.333 [0.000, 0.667] |
| broad_basin | logistic_regression | strict_window_fa<=1 | rapid | 2-5 | 5 | 296 | 0.260 [0.077, 0.539] | 0.600 [0.200, 1.000] |
| broad_basin | logistic_regression | strict_window_fa<=1 | rapid | >5 | 6 | 377 | 0.164 [0.054, 0.308] | 0.667 [0.333, 1.000] |
| broad_basin | random_forest | raw (k=1) | gradual | <1 | 5 | 353 | 0.229 [0.039, 0.391] | 0.800 [0.400, 1.000] |
| broad_basin | random_forest | raw (k=1) | gradual | 1-2 | 6 | 398 | 0.166 [0.060, 0.274] | 0.833 [0.500, 1.000] |
| broad_basin | random_forest | raw (k=1) | gradual | 2-5 | 3 | 199 | 0.357 [0.162, 0.732] | 1.000 [1.000, 1.000] |
| broad_basin | random_forest | raw (k=1) | gradual | >5 | 6 | 394 | 0.373 [0.167, 0.559] | 1.000 [1.000, 1.000] |
| broad_basin | random_forest | raw (k=1) | rapid | <1 | 6 | 373 | 0.164 [0.078, 0.249] | 1.000 [1.000, 1.000] |
| broad_basin | random_forest | raw (k=1) | rapid | 1-2 | 3 | 175 | 0.314 [0.000, 0.814] | 0.667 [0.000, 1.000] |
| broad_basin | random_forest | raw (k=1) | rapid | 2-5 | 5 | 296 | 0.530 [0.307, 0.775] | 0.800 [0.400, 1.000] |
| broad_basin | random_forest | raw (k=1) | rapid | >5 | 6 | 377 | 0.501 [0.310, 0.782] | 1.000 [1.000, 1.000] |
| broad_basin | random_forest | episode_fa<=1 (k=3,m=3) | gradual | <1 | 5 | 353 | 0.125 [0.008, 0.245] | 0.600 [0.200, 1.000] |
| broad_basin | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 6 | 398 | 0.123 [0.036, 0.214] | 0.333 [0.000, 0.667] |
| broad_basin | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 3 | 199 | 0.337 [0.162, 0.696] | 0.667 [0.333, 1.000] |
| broad_basin | random_forest | episode_fa<=1 (k=3,m=3) | gradual | >5 | 6 | 394 | 0.363 [0.159, 0.547] | 1.000 [1.000, 1.000] |
| broad_basin | random_forest | episode_fa<=1 (k=3,m=3) | rapid | <1 | 6 | 373 | 0.150 [0.073, 0.227] | 0.667 [0.333, 1.000] |
| broad_basin | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 3 | 175 | 0.337 [0.000, 0.881] | 0.667 [0.000, 1.000] |
| broad_basin | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 5 | 296 | 0.527 [0.307, 0.775] | 0.800 [0.400, 1.000] |
| broad_basin | random_forest | episode_fa<=1 (k=3,m=3) | rapid | >5 | 6 | 377 | 0.501 [0.310, 0.782] | 1.000 [1.000, 1.000] |
| broad_basin | random_forest | strict_window_fa<=1 | gradual | <1 | 5 | 353 | 0.023 [0.000, 0.057] | 0.000 [0.000, 0.000] |
| broad_basin | random_forest | strict_window_fa<=1 | gradual | 1-2 | 6 | 398 | 0.045 [0.005, 0.105] | 0.167 [0.000, 0.500] |
| broad_basin | random_forest | strict_window_fa<=1 | gradual | 2-5 | 3 | 199 | 0.156 [0.101, 0.250] | 0.667 [0.333, 1.000] |
| broad_basin | random_forest | strict_window_fa<=1 | gradual | >5 | 6 | 394 | 0.320 [0.110, 0.521] | 0.667 [0.167, 1.000] |
| broad_basin | random_forest | strict_window_fa<=1 | rapid | <1 | 6 | 373 | 0.056 [0.017, 0.099] | 0.333 [0.000, 0.667] |
| broad_basin | random_forest | strict_window_fa<=1 | rapid | 1-2 | 3 | 175 | 0.200 [0.000, 0.508] | 0.667 [0.000, 1.000] |
| broad_basin | random_forest | strict_window_fa<=1 | rapid | 2-5 | 5 | 296 | 0.412 [0.153, 0.673] | 0.800 [0.400, 1.000] |
| broad_basin | random_forest | strict_window_fa<=1 | rapid | >5 | 6 | 377 | 0.456 [0.259, 0.760] | 1.000 [1.000, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | raw (k=1) | gradual | <1 | 27 | 1853 | 0.124 [0.082, 0.170] | 0.667 [0.499, 0.815] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | raw (k=1) | gradual | 1-2 | 19 | 1257 | 0.098 [0.051, 0.149] | 0.526 [0.316, 0.737] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | raw (k=1) | gradual | 2-5 | 13 | 879 | 0.198 [0.119, 0.277] | 0.846 [0.615, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | raw (k=1) | gradual | >5 | 26 | 1714 | 0.341 [0.300, 0.386] | 0.962 [0.885, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | raw (k=1) | rapid | <1 | 26 | 1576 | 0.123 [0.069, 0.192] | 0.654 [0.500, 0.808] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | raw (k=1) | rapid | 1-2 | 15 | 938 | 0.098 [0.043, 0.159] | 0.600 [0.365, 0.800] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | raw (k=1) | rapid | 2-5 | 22 | 1356 | 0.295 [0.170, 0.433] | 0.636 [0.455, 0.818] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | raw (k=1) | rapid | >5 | 20 | 1218 | 0.546 [0.452, 0.638] | 0.950 [0.850, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | <1 | 27 | 1853 | 0.124 [0.082, 0.170] | 0.333 [0.185, 0.501] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 19 | 1257 | 0.098 [0.051, 0.149] | 0.263 [0.105, 0.474] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 13 | 879 | 0.198 [0.119, 0.277] | 0.538 [0.308, 0.769] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | episode_fa<=1 (k=3,m=3) | gradual | >5 | 26 | 1714 | 0.341 [0.300, 0.386] | 0.923 [0.808, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | <1 | 26 | 1576 | 0.123 [0.069, 0.192] | 0.269 [0.115, 0.462] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 15 | 938 | 0.098 [0.043, 0.159] | 0.200 [0.000, 0.400] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 22 | 1356 | 0.295 [0.170, 0.433] | 0.500 [0.318, 0.727] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | episode_fa<=1 (k=3,m=3) | rapid | >5 | 20 | 1218 | 0.546 [0.452, 0.638] | 0.900 [0.750, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | strict_window_fa<=1 | gradual | <1 | 27 | 1853 | 0.124 [0.082, 0.170] | 0.037 [0.000, 0.111] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | strict_window_fa<=1 | gradual | 1-2 | 19 | 1257 | 0.098 [0.051, 0.149] | 0.053 [0.000, 0.158] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | strict_window_fa<=1 | gradual | 2-5 | 13 | 879 | 0.198 [0.119, 0.277] | 0.231 [0.000, 0.462] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | strict_window_fa<=1 | gradual | >5 | 26 | 1714 | 0.341 [0.300, 0.386] | 0.769 [0.577, 0.923] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | strict_window_fa<=1 | rapid | <1 | 26 | 1576 | 0.123 [0.069, 0.192] | 0.077 [0.000, 0.231] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | strict_window_fa<=1 | rapid | 1-2 | 15 | 938 | 0.098 [0.043, 0.159] | 0.067 [0.000, 0.200] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | strict_window_fa<=1 | rapid | 2-5 | 22 | 1356 | 0.295 [0.170, 0.433] | 0.455 [0.273, 0.682] |
| pooled (test+shifted_test+stress+broad_basin) | threshold_rule | strict_window_fa<=1 | rapid | >5 | 20 | 1218 | 0.546 [0.452, 0.638] | 0.900 [0.750, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | raw (k=1) | gradual | <1 | 27 | 1853 | 0.326 [0.231, 0.412] | 0.926 [0.815, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | raw (k=1) | gradual | 1-2 | 19 | 1257 | 0.264 [0.186, 0.347] | 0.895 [0.737, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | raw (k=1) | gradual | 2-5 | 13 | 879 | 0.224 [0.116, 0.353] | 1.000 [1.000, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | raw (k=1) | gradual | >5 | 26 | 1714 | 0.282 [0.172, 0.412] | 0.769 [0.615, 0.923] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | raw (k=1) | rapid | <1 | 26 | 1576 | 0.260 [0.179, 0.336] | 0.962 [0.885, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | raw (k=1) | rapid | 1-2 | 15 | 938 | 0.367 [0.231, 0.486] | 0.933 [0.800, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | raw (k=1) | rapid | 2-5 | 22 | 1356 | 0.481 [0.347, 0.607] | 0.909 [0.773, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | raw (k=1) | rapid | >5 | 20 | 1218 | 0.531 [0.376, 0.687] | 1.000 [1.000, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | <1 | 27 | 1853 | 0.063 [0.037, 0.095] | 0.222 [0.074, 0.370] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 19 | 1257 | 0.068 [0.025, 0.113] | 0.211 [0.053, 0.421] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 13 | 879 | 0.083 [0.015, 0.180] | 0.154 [0.000, 0.385] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | episode_fa<=1 (k=3,m=3) | gradual | >5 | 26 | 1714 | 0.182 [0.093, 0.294] | 0.462 [0.269, 0.674] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | <1 | 26 | 1576 | 0.081 [0.042, 0.124] | 0.269 [0.115, 0.462] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 15 | 938 | 0.164 [0.101, 0.240] | 0.533 [0.298, 0.733] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 22 | 1356 | 0.336 [0.215, 0.450] | 0.682 [0.500, 0.864] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | episode_fa<=1 (k=3,m=3) | rapid | >5 | 20 | 1218 | 0.504 [0.354, 0.657] | 0.800 [0.600, 0.950] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | strict_window_fa<=1 | gradual | <1 | 27 | 1853 | 0.010 [0.004, 0.016] | 0.000 [0.000, 0.000] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | strict_window_fa<=1 | gradual | 1-2 | 19 | 1257 | 0.016 [0.003, 0.031] | 0.000 [0.000, 0.000] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | strict_window_fa<=1 | gradual | 2-5 | 13 | 879 | 0.027 [0.001, 0.074] | 0.077 [0.000, 0.231] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | strict_window_fa<=1 | gradual | >5 | 26 | 1714 | 0.086 [0.026, 0.162] | 0.231 [0.077, 0.423] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | strict_window_fa<=1 | rapid | <1 | 26 | 1576 | 0.019 [0.006, 0.038] | 0.077 [0.000, 0.212] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | strict_window_fa<=1 | rapid | 1-2 | 15 | 938 | 0.050 [0.025, 0.079] | 0.133 [0.000, 0.333] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | strict_window_fa<=1 | rapid | 2-5 | 22 | 1356 | 0.145 [0.058, 0.225] | 0.409 [0.182, 0.591] |
| pooled (test+shifted_test+stress+broad_basin) | logistic_regression | strict_window_fa<=1 | rapid | >5 | 20 | 1218 | 0.303 [0.146, 0.459] | 0.600 [0.374, 0.800] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | raw (k=1) | gradual | <1 | 27 | 1853 | 0.215 [0.146, 0.290] | 0.852 [0.704, 0.963] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | raw (k=1) | gradual | 1-2 | 19 | 1257 | 0.270 [0.172, 0.371] | 0.842 [0.684, 0.975] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | raw (k=1) | gradual | 2-5 | 13 | 879 | 0.225 [0.124, 0.336] | 0.846 [0.615, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | raw (k=1) | gradual | >5 | 26 | 1714 | 0.306 [0.212, 0.409] | 0.846 [0.692, 0.962] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | raw (k=1) | rapid | <1 | 26 | 1576 | 0.126 [0.062, 0.187] | 0.692 [0.518, 0.846] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | raw (k=1) | rapid | 1-2 | 15 | 938 | 0.221 [0.105, 0.323] | 0.800 [0.600, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | raw (k=1) | rapid | 2-5 | 22 | 1356 | 0.364 [0.225, 0.499] | 0.727 [0.500, 0.909] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | raw (k=1) | rapid | >5 | 20 | 1218 | 0.603 [0.458, 0.737] | 0.950 [0.850, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | episode_fa<=1 (k=3,m=3) | gradual | <1 | 27 | 1853 | 0.101 [0.063, 0.153] | 0.407 [0.259, 0.593] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 1-2 | 19 | 1257 | 0.222 [0.126, 0.327] | 0.474 [0.211, 0.684] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | episode_fa<=1 (k=3,m=3) | gradual | 2-5 | 13 | 879 | 0.148 [0.059, 0.246] | 0.462 [0.231, 0.692] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | episode_fa<=1 (k=3,m=3) | gradual | >5 | 26 | 1714 | 0.277 [0.184, 0.383] | 0.769 [0.615, 0.923] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | episode_fa<=1 (k=3,m=3) | rapid | <1 | 26 | 1576 | 0.115 [0.055, 0.178] | 0.385 [0.211, 0.577] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 1-2 | 15 | 938 | 0.209 [0.093, 0.327] | 0.600 [0.333, 0.867] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | episode_fa<=1 (k=3,m=3) | rapid | 2-5 | 22 | 1356 | 0.358 [0.224, 0.487] | 0.682 [0.476, 0.864] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | episode_fa<=1 (k=3,m=3) | rapid | >5 | 20 | 1218 | 0.594 [0.448, 0.724] | 0.900 [0.750, 1.000] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | strict_window_fa<=1 | gradual | <1 | 27 | 1853 | 0.018 [0.006, 0.037] | 0.074 [0.000, 0.185] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | strict_window_fa<=1 | gradual | 1-2 | 19 | 1257 | 0.114 [0.051, 0.188] | 0.316 [0.105, 0.526] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | strict_window_fa<=1 | gradual | 2-5 | 13 | 879 | 0.067 [0.024, 0.116] | 0.385 [0.154, 0.615] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | strict_window_fa<=1 | gradual | >5 | 26 | 1714 | 0.236 [0.148, 0.333] | 0.577 [0.364, 0.769] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | strict_window_fa<=1 | rapid | <1 | 26 | 1576 | 0.061 [0.022, 0.107] | 0.231 [0.077, 0.423] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | strict_window_fa<=1 | rapid | 1-2 | 15 | 938 | 0.110 [0.051, 0.184] | 0.400 [0.200, 0.667] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | strict_window_fa<=1 | rapid | 2-5 | 22 | 1356 | 0.275 [0.149, 0.396] | 0.636 [0.409, 0.818] |
| pooled (test+shifted_test+stress+broad_basin) | random_forest | strict_window_fa<=1 | rapid | >5 | 20 | 1218 | 0.521 [0.382, 0.663] | 0.850 [0.650, 1.000] |
