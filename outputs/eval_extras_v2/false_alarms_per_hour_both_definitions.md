# False alarms per hour - two time definitions (SYNTHETIC / SIMULATION)

> **SYNTHETIC / SIMULATION** - all data are simulated; nothing here is validated on real data or field-ready.

* **Definition A - slow-process time (ground-movement timescale)**: false alarms per normal run / 24 h (240 s x compression factor 360 / 3600).
* **Definition B - sensor time (noise, vibration and window timescale)**: false alarms per normal run / 0.0667 h (240 s of actual sensor time / 3600). Definition B is the stricter figure (15x higher than A with these numbers) and the more defensible one for false alarms caused by sensor noise and benign vibration. Neither is a validated field rate.
* All normal runs of every listed split use compression factor 360, so the factors are never mixed. Rows are false-alarm *episodes* (after persistence); CIs are run-bootstrap 95%; missed-event rate = event runs with no correct alarm.

| split | model | regime | FA eps / run | A: FA / h (slow) | A: one FA every | B: FA / h (sensor) | B: one FA every | missed-event rate | exact detect |
|---|---|---|---|---|---|---|---|---|---|
| test | threshold_rule | raw (k=1) | 6.750 [2.295, 11.850] | 0.2812 [0.0956, 0.4938] | 3.6 h | 101.25 [34.42, 177.75] | 0.6 min | 0.200 [0.130, 0.290] | 0.800 |
| test | threshold_rule | episode_fa<=1 (k=3,m=3) | 0.600 [0.050, 1.326] | 0.0250 [0.0021, 0.0553] | 40.0 h | 9.00 [0.75, 19.89] | 6.7 min | 0.300 [0.210, 0.390] | 0.700 |
| test | threshold_rule | strict_window_fa<=1 | 0.050 [0.000, 0.150] | 0.0021 [0.0000, 0.0063] | 480.0 h | 0.75 [0.00, 2.25] | 1.3 h | 0.350 [0.265, 0.445] | 0.650 |
| test | logistic_regression | raw (k=1) | 21.100 [16.442, 25.626] | 0.8792 [0.6851, 1.0678] | 1.1 h | 316.50 [246.64, 384.39] | 0.2 min | 0.060 [0.020, 0.120] | 0.940 |
| test | logistic_regression | episode_fa<=1 (k=3,m=3) | 0.100 [0.000, 0.200] | 0.0042 [0.0000, 0.0083] | 240.0 h | 1.50 [0.00, 3.00] | 40.0 min | 0.390 [0.290, 0.480] | 0.610 |
| test | logistic_regression | strict_window_fa<=1 | 0.000 [0.000, 0.000] | 0.0000 [0.0000, 0.0000] | none observed | 0.00 [0.00, 0.00] | none observed | 0.450 [0.360, 0.545] | 0.550 |
| test | random_forest | raw (k=1) | 5.650 [3.450, 8.100] | 0.2354 [0.1437, 0.3375] | 4.2 h | 84.75 [51.75, 121.50] | 0.7 min | 0.170 [0.105, 0.250] | 0.830 |
| test | random_forest | episode_fa<=1 (k=3,m=3) | 0.650 [0.200, 1.176] | 0.0271 [0.0083, 0.0490] | 36.9 h | 9.75 [3.00, 17.64] | 6.2 min | 0.310 [0.230, 0.410] | 0.690 |
| test | random_forest | strict_window_fa<=1 | 0.250 [0.050, 0.500] | 0.0104 [0.0021, 0.0208] | 96.0 h | 3.75 [0.75, 7.50] | 16.0 min | 0.360 [0.280, 0.460] | 0.640 |
| shifted_test | threshold_rule | raw (k=1) | 29.800 [23.958, 37.108] | 1.2417 [0.9983, 1.5462] | 48.3 min | 447.00 [359.38, 556.62] | 0.1 min | 0.053 [0.013, 0.107] | 0.947 |
| shifted_test | threshold_rule | episode_fa<=1 (k=3,m=3) | 2.467 [1.463, 3.502] | 0.1028 [0.0610, 0.1459] | 9.7 h | 37.00 [21.95, 52.52] | 1.6 min | 0.173 [0.093, 0.267] | 0.827 |
| shifted_test | threshold_rule | strict_window_fa<=1 | 0.200 [0.000, 0.400] | 0.0083 [0.0000, 0.0167] | 120.0 h | 3.00 [0.00, 6.00] | 20.0 min | 0.333 [0.240, 0.427] | 0.667 |
| shifted_test | logistic_regression | raw (k=1) | 29.467 [27.298, 31.400] | 1.2278 [1.1374, 1.3083] | 48.9 min | 442.00 [409.48, 471.00] | 0.1 min | 0.013 [0.000, 0.040] | 0.987 |
| shifted_test | logistic_regression | episode_fa<=1 (k=3,m=3) | 1.267 [0.667, 1.968] | 0.0528 [0.0278, 0.0820] | 18.9 h | 19.00 [10.00, 29.52] | 3.2 min | 0.307 [0.213, 0.413] | 0.693 |
| shifted_test | logistic_regression | strict_window_fa<=1 | 0.600 [0.200, 1.067] | 0.0250 [0.0083, 0.0444] | 40.0 h | 9.00 [3.00, 16.00] | 6.7 min | 0.467 [0.347, 0.573] | 0.533 |
| shifted_test | random_forest | raw (k=1) | 14.333 [12.133, 16.768] | 0.5972 [0.5056, 0.6987] | 1.7 h | 215.00 [182.00, 251.53] | 0.3 min | 0.107 [0.053, 0.187] | 0.893 |
| shifted_test | random_forest | episode_fa<=1 (k=3,m=3) | 1.400 [0.698, 2.333] | 0.0583 [0.0291, 0.0972] | 17.1 h | 21.00 [10.47, 35.00] | 2.9 min | 0.227 [0.147, 0.320] | 0.773 |
| shifted_test | random_forest | strict_window_fa<=1 | 0.200 [0.000, 0.400] | 0.0083 [0.0000, 0.0167] | 120.0 h | 3.00 [0.00, 6.00] | 20.0 min | 0.280 [0.187, 0.400] | 0.720 |
| val | threshold_rule | raw (k=1) | 11.450 [6.674, 17.453] | 0.4771 [0.2781, 0.7272] | 2.1 h | 171.75 [100.11, 261.79] | 0.3 min | 0.250 [0.170, 0.335] | 0.750 |
| val | threshold_rule | episode_fa<=1 (k=3,m=3) | 1.000 [0.450, 1.750] | 0.0417 [0.0187, 0.0729] | 24.0 h | 15.00 [6.75, 26.25] | 4.0 min | 0.280 [0.200, 0.370] | 0.720 |
| val | threshold_rule | strict_window_fa<=1 | 0.200 [0.050, 0.400] | 0.0083 [0.0021, 0.0167] | 120.0 h | 3.00 [0.75, 6.00] | 20.0 min | 0.350 [0.260, 0.450] | 0.650 |
| val | logistic_regression | raw (k=1) | 23.400 [19.074, 27.376] | 0.9750 [0.7947, 1.1407] | 1.0 h | 351.00 [286.11, 410.64] | 0.2 min | 0.050 [0.010, 0.090] | 0.950 |
| val | logistic_regression | episode_fa<=1 (k=3,m=3) | 0.850 [0.450, 1.350] | 0.0354 [0.0187, 0.0563] | 28.2 h | 12.75 [6.75, 20.25] | 4.7 min | 0.340 [0.250, 0.420] | 0.660 |
| val | logistic_regression | strict_window_fa<=1 | 0.300 [0.100, 0.600] | 0.0125 [0.0042, 0.0250] | 80.0 h | 4.50 [1.50, 9.00] | 13.3 min | 0.390 [0.300, 0.480] | 0.610 |
| val | random_forest | raw (k=1) | 8.350 [4.971, 11.479] | 0.3479 [0.2071, 0.4783] | 2.9 h | 125.25 [74.57, 172.18] | 0.5 min | 0.170 [0.100, 0.240] | 0.830 |
| val | random_forest | episode_fa<=1 (k=3,m=3) | 1.000 [0.450, 1.700] | 0.0417 [0.0187, 0.0708] | 24.0 h | 15.00 [6.75, 25.50] | 4.0 min | 0.240 [0.160, 0.320] | 0.760 |
| val | random_forest | strict_window_fa<=1 | 0.400 [0.150, 0.750] | 0.0167 [0.0063, 0.0312] | 60.0 h | 6.00 [2.25, 11.25] | 10.0 min | 0.300 [0.230, 0.385] | 0.700 |
| train | threshold_rule | raw (k=1) | 4.533 [1.857, 7.402] | 0.1889 [0.0774, 0.3084] | 5.3 h | 68.00 [27.86, 111.04] | 0.9 min | 0.207 [0.160, 0.252] | 0.793 |
| train | threshold_rule | episode_fa<=1 (k=3,m=3) | 0.350 [0.075, 0.692] | 0.0146 [0.0031, 0.0288] | 68.6 h | 5.25 [1.12, 10.38] | 11.4 min | 0.293 [0.245, 0.350] | 0.707 |
| train | threshold_rule | strict_window_fa<=1 | 0.050 [0.000, 0.142] | 0.0021 [0.0000, 0.0059] | 480.0 h | 0.75 [0.00, 2.13] | 1.3 h | 0.377 [0.323, 0.433] | 0.623 |
| train | logistic_regression | raw (k=1) | 18.567 [15.865, 21.003] | 0.7736 [0.6610, 0.8751] | 1.3 h | 278.50 [237.97, 315.05] | 0.2 min | 0.027 [0.010, 0.047] | 0.973 |
| train | logistic_regression | episode_fa<=1 (k=3,m=3) | 0.250 [0.133, 0.392] | 0.0104 [0.0056, 0.0163] | 96.0 h | 3.75 [2.00, 5.88] | 16.0 min | 0.300 [0.248, 0.350] | 0.700 |
| train | logistic_regression | strict_window_fa<=1 | 0.150 [0.067, 0.267] | 0.0063 [0.0028, 0.0111] | 160.0 h | 2.25 [1.00, 4.00] | 26.7 min | 0.393 [0.340, 0.447] | 0.607 |
| train | random_forest | raw (k=1) | 2.683 [1.799, 3.592] | 0.1118 [0.0750, 0.1497] | 8.9 h | 40.25 [26.99, 53.88] | 1.5 min | 0.007 [0.000, 0.017] | 0.993 |
| train | random_forest | episode_fa<=1 (k=3,m=3) | 0.250 [0.100, 0.417] | 0.0104 [0.0042, 0.0174] | 96.0 h | 3.75 [1.50, 6.25] | 16.0 min | 0.037 [0.017, 0.057] | 0.963 |
| train | random_forest | strict_window_fa<=1 | 0.000 [0.000, 0.000] | 0.0000 [0.0000, 0.0000] | none observed | 0.00 [0.00, 0.00] | none observed | 0.077 [0.050, 0.103] | 0.923 |
