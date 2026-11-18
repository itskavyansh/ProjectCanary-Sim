# Normal-Run False Alarms Under Frozen 360x vs Alternative 30-Day Compression Factors (SYNTHETIC / SIMULATION)

> **SYNTHETIC / SIMULATION** — Literature-basis sensitivity checks on frozen v3 models; nothing here is validated on real data.

| model | regime | FA eps / run [95% CI] | B: sensor time (1x, 0.0667h/run) | A (frozen 360x, 24h/run) | A_alt (10,000x, 666.7h/run) | A_alt (10,800x = 30d/run, 720h/run) | A_alt (30,000x, 2000h/run) |
|---|---|---|---|---|---|---|---|
| threshold_rule | raw (k=1) | 6.525 [3.697, 9.988] | 97.88/h (0.6 min) | 0.2719/h (3.7 h) | 0.009788/h (102.2 h) | 0.009063/h (110.3 h) | 0.003263/h (306.5 h) |
| threshold_rule | episode_fa<=1 (k=3,m=3) | 0.450 [0.175, 0.800] | 6.75/h (8.9 min) | 0.0187/h (53.3 h) | 0.000675/h (1481.5 h) | 0.000625/h (1600.0 h) | 0.000225/h (4444.4 h) |
| threshold_rule | strict_window_fa<=1 | 0.100 [0.000, 0.225] | 1.50/h (40.0 min) | 0.0042/h (240.0 h) | 0.000150/h (6666.7 h) | 0.000139/h (7200.0 h) | 0.000050/h (20000.0 h) |
| logistic_regression | raw (k=1) | 21.075 [18.212, 24.279] | 316.12/h (0.2 min) | 0.8781/h (1.1 h) | 0.031613/h (31.6 h) | 0.029271/h (34.2 h) | 0.010537/h (94.9 h) |
| logistic_regression | episode_fa<=1 (k=3,m=3) | 0.350 [0.175, 0.550] | 5.25/h (11.4 min) | 0.0146/h (68.6 h) | 0.000525/h (1904.8 h) | 0.000486/h (2057.1 h) | 0.000175/h (5714.3 h) |
| logistic_regression | strict_window_fa<=1 | 0.125 [0.000, 0.338] | 1.88/h (32.0 min) | 0.0052/h (192.0 h) | 0.000188/h (5333.3 h) | 0.000174/h (5760.0 h) | 0.000063/h (16000.0 h) |
| random_forest | raw (k=1) | 7.100 [5.149, 9.263] | 106.50/h (0.6 min) | 0.2958/h (3.4 h) | 0.010650/h (93.9 h) | 0.009861/h (101.4 h) | 0.003550/h (281.7 h) |
| random_forest | episode_fa<=1 (k=3,m=3) | 0.450 [0.225, 0.700] | 6.75/h (8.9 min) | 0.0187/h (53.3 h) | 0.000675/h (1481.5 h) | 0.000625/h (1600.0 h) | 0.000225/h (4444.4 h) |
| random_forest | strict_window_fa<=1 | 0.225 [0.100, 0.363] | 3.38/h (17.8 min) | 0.0094/h (106.7 h) | 0.000338/h (2963.0 h) | 0.000313/h (3200.0 h) | 0.000112/h (8888.9 h) |
