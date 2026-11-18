# Gradual vs Sensor_Fault Confusion Counts Across B1 & B2 Arms (SYNTHETIC / SIMULATION)

> **SYNTHETIC / SIMULATION** — Literature-basis sensitivity checks on frozen v3 models; nothing here is validated on real data.

| arm | model | regime | gradual win | win: gradual->sensor_fault [95% CI] (rate) | alarm: gradual->sensor_fault [95% CI] | win->gradual | win->rapid | win->normal |
|---|---|---|---:|---|---|---:|---:|---:|
| `gaussian_control` | threshold_rule | episode_fa<=1 (k=3,m=3) | 2008 | **80** [0.0, 187.0] (0.040) | **78** [0.0, 206.0] | 377 | 307 | 1240 |
| `gaussian_control` | threshold_rule | strict_window_fa<=1 | 2008 | **80** [0.0, 187.0] (0.040) | **74** [0.0, 196.0] | 377 | 307 | 1240 |
| `gaussian_control` | logistic_regression | episode_fa<=1 (k=3,m=3) | 2008 | **15** [2.0, 31.0] (0.007) | **0** [0.0, 0.0] | 351 | 364 | 1276 |
| `gaussian_control` | logistic_regression | strict_window_fa<=1 | 2008 | **8** [0.0, 18.0] (0.004) | **0** [0.0, 0.0] | 135 | 172 | 1691 |
| `gaussian_control` | random_forest | episode_fa<=1 (k=3,m=3) | 2008 | **40** [3.0, 103.5] (0.020) | **27** [0.0, 78.0] | 494 | 393 | 1075 |
| `gaussian_control` | random_forest | strict_window_fa<=1 | 2008 | **44** [6.0, 109.5] (0.022) | **24** [0.0, 70.0] | 298 | 229 | 1431 |
| `high_tilt_3_6` | threshold_rule | episode_fa<=1 (k=3,m=3) | 2014 | **786** [557.8, 990.5] (0.390) | **740** [546.9, 941.0] | 492 | 335 | 392 |
| `high_tilt_3_6` | threshold_rule | strict_window_fa<=1 | 2014 | **786** [557.8, 990.5] (0.390) | **687** [494.8, 879.1] | 492 | 335 | 392 |
| `high_tilt_3_6` | logistic_regression | episode_fa<=1 (k=3,m=3) | 2014 | **77** [28.4, 149.1] (0.038) | **57** [9.0, 117.0] | 618 | 597 | 715 |
| `high_tilt_3_6` | logistic_regression | strict_window_fa<=1 | 2014 | **61** [20.0, 122.2] (0.030) | **24** [2.0, 60.0] | 412 | 292 | 1242 |
| `high_tilt_3_6` | random_forest | episode_fa<=1 (k=3,m=3) | 2014 | **207** [84.0, 344.0] (0.103) | **187** [66.0, 322.0] | 575 | 748 | 480 |
| `high_tilt_3_6` | random_forest | strict_window_fa<=1 | 2014 | **241** [105.9, 393.5] (0.120) | **226** [75.4, 373.5] | 457 | 570 | 742 |
| `high_tilt_6_12` | threshold_rule | episode_fa<=1 (k=3,m=3) | 2038 | **1382** [1280.0, 1506.6] (0.678) | **1334** [1215.0, 1459.0] | 243 | 183 | 224 |
| `high_tilt_6_12` | threshold_rule | strict_window_fa<=1 | 2038 | **1382** [1280.0, 1506.6] (0.678) | **1263** [1144.0, 1385.2] | 243 | 183 | 224 |
| `high_tilt_6_12` | logistic_regression | episode_fa<=1 (k=3,m=3) | 2038 | **186** [73.5, 314.5] (0.091) | **180** [77.4, 298.6] | 1020 | 433 | 398 |
| `high_tilt_6_12` | logistic_regression | strict_window_fa<=1 | 2038 | **168** [63.4, 289.5] (0.082) | **156** [56.4, 271.0] | 942 | 286 | 641 |
| `high_tilt_6_12` | random_forest | episode_fa<=1 (k=3,m=3) | 2038 | **149** [28.4, 308.6] (0.073) | **150** [27.9, 306.0] | 450 | 1131 | 297 |
| `high_tilt_6_12` | random_forest | strict_window_fa<=1 | 2038 | **164** [39.5, 325.0] (0.081) | **153** [36.4, 300.7] | 349 | 1004 | 510 |
| `depth_all_gt_1p5` | threshold_rule | episode_fa<=1 (k=3,m=3) | 4685 | **1** [0.0, 3.5] (0.000) | **0** [0.0, 0.0] | 837 | 841 | 2997 |
| `depth_all_gt_1p5` | threshold_rule | strict_window_fa<=1 | 4685 | **1** [0.0, 3.5] (0.000) | **0** [0.0, 0.0] | 837 | 841 | 2997 |
| `depth_all_gt_1p5` | logistic_regression | episode_fa<=1 (k=3,m=3) | 4685 | **19** [3.0, 38.0] (0.004) | **9** [0.0, 23.0] | 515 | 1453 | 2684 |
| `depth_all_gt_1p5` | logistic_regression | strict_window_fa<=1 | 4685 | **13** [2.0, 26.5] (0.003) | **4** [0.0, 12.0] | 258 | 822 | 3578 |
| `depth_all_gt_1p5` | random_forest | episode_fa<=1 (k=3,m=3) | 4685 | **15** [2.0, 38.0] (0.003) | **10** [0.0, 30.0] | 1314 | 1358 | 1985 |
| `depth_all_gt_1p5` | random_forest | strict_window_fa<=1 | 4685 | **17** [3.0, 40.0] (0.004) | **9** [0.0, 27.0] | 948 | 1013 | 2694 |
| `H100_tanB1p5` | threshold_rule | episode_fa<=1 (k=3,m=3) | 683 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 136 | 121 | 426 |
| `H100_tanB1p5` | threshold_rule | strict_window_fa<=1 | 683 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 136 | 121 | 426 |
| `H100_tanB1p5` | logistic_regression | episode_fa<=1 (k=3,m=3) | 683 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 69 | 261 | 351 |
| `H100_tanB1p5` | logistic_regression | strict_window_fa<=1 | 683 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 41 | 125 | 515 |
| `H100_tanB1p5` | random_forest | episode_fa<=1 (k=3,m=3) | 683 | **2** [0.0, 8.0] (0.003) | **0** [0.0, 0.0] | 245 | 198 | 237 |
| `H100_tanB1p5` | random_forest | strict_window_fa<=1 | 683 | **2** [0.0, 8.0] (0.003) | **0** [0.0, 0.0] | 206 | 143 | 331 |
| `H200_tanB1p5` | threshold_rule | episode_fa<=1 (k=3,m=3) | 667 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 148 | 152 | 365 |
| `H200_tanB1p5` | threshold_rule | strict_window_fa<=1 | 667 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 148 | 152 | 365 |
| `H200_tanB1p5` | logistic_regression | episode_fa<=1 (k=3,m=3) | 667 | **8** [0.0, 24.0] (0.012) | **0** [0.0, 0.0] | 83 | 185 | 389 |
| `H200_tanB1p5` | logistic_regression | strict_window_fa<=1 | 667 | **4** [0.0, 12.0] (0.006) | **0** [0.0, 0.0] | 25 | 103 | 533 |
| `H200_tanB1p5` | random_forest | episode_fa<=1 (k=3,m=3) | 667 | **2** [0.0, 6.0] (0.003) | **0** [0.0, 0.0] | 217 | 146 | 301 |
| `H200_tanB1p5` | random_forest | strict_window_fa<=1 | 667 | **2** [0.0, 6.0] (0.003) | **0** [0.0, 0.0] | 142 | 100 | 422 |
| `H200_tanB2p0` | threshold_rule | episode_fa<=1 (k=3,m=3) | 655 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 92 | 161 | 402 |
| `H200_tanB2p0` | threshold_rule | strict_window_fa<=1 | 655 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 92 | 161 | 402 |
| `H200_tanB2p0` | logistic_regression | episode_fa<=1 (k=3,m=3) | 655 | **1** [0.0, 4.0] (0.002) | **0** [0.0, 0.0] | 121 | 185 | 348 |
| `H200_tanB2p0` | logistic_regression | strict_window_fa<=1 | 655 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 60 | 108 | 487 |
| `H200_tanB2p0` | random_forest | episode_fa<=1 (k=3,m=3) | 655 | **1** [0.0, 3.0] (0.002) | **0** [0.0, 0.0] | 201 | 185 | 268 |
| `H200_tanB2p0` | random_forest | strict_window_fa<=1 | 655 | **1** [0.0, 3.0] (0.002) | **0** [0.0, 0.0] | 132 | 142 | 380 |
| `H200_tanB2p5` | threshold_rule | episode_fa<=1 (k=3,m=3) | 683 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 140 | 127 | 413 |
| `H200_tanB2p5` | threshold_rule | strict_window_fa<=1 | 683 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 140 | 127 | 413 |
| `H200_tanB2p5` | logistic_regression | episode_fa<=1 (k=3,m=3) | 683 | **3** [0.0, 7.0] (0.004) | **4** [0.0, 12.0] | 84 | 219 | 373 |
| `H200_tanB2p5` | logistic_regression | strict_window_fa<=1 | 683 | **2** [0.0, 5.0] (0.003) | **0** [0.0, 0.0] | 56 | 151 | 470 |
| `H200_tanB2p5` | random_forest | episode_fa<=1 (k=3,m=3) | 683 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 165 | 235 | 278 |
| `H200_tanB2p5` | random_forest | strict_window_fa<=1 | 683 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 134 | 188 | 356 |
| `H300_tanB1p5` | threshold_rule | episode_fa<=1 (k=3,m=3) | 678 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 99 | 79 | 500 |
| `H300_tanB1p5` | threshold_rule | strict_window_fa<=1 | 678 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 99 | 79 | 500 |
| `H300_tanB1p5` | logistic_regression | episode_fa<=1 (k=3,m=3) | 678 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 15 | 242 | 420 |
| `H300_tanB1p5` | logistic_regression | strict_window_fa<=1 | 678 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 0 | 138 | 539 |
| `H300_tanB1p5` | random_forest | episode_fa<=1 (k=3,m=3) | 678 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 159 | 196 | 321 |
| `H300_tanB1p5` | random_forest | strict_window_fa<=1 | 678 | **1** [0.0, 3.0] (0.002) | **0** [0.0, 0.0] | 120 | 171 | 384 |
| `H300_tanB2p0` | threshold_rule | episode_fa<=1 (k=3,m=3) | 652 | **1** [0.0, 3.0] (0.002) | **0** [0.0, 0.0] | 95 | 88 | 468 |
| `H300_tanB2p0` | threshold_rule | strict_window_fa<=1 | 652 | **1** [0.0, 3.0] (0.002) | **0** [0.0, 0.0] | 95 | 88 | 468 |
| `H300_tanB2p0` | logistic_regression | episode_fa<=1 (k=3,m=3) | 652 | **6** [0.0, 16.0] (0.009) | **5** [0.0, 15.0] | 60 | 146 | 439 |
| `H300_tanB2p0` | logistic_regression | strict_window_fa<=1 | 652 | **6** [0.0, 16.0] (0.009) | **4** [0.0, 12.0] | 26 | 64 | 555 |
| `H300_tanB2p0` | random_forest | episode_fa<=1 (k=3,m=3) | 652 | **10** [0.0, 29.0] (0.015) | **10** [0.0, 30.0] | 150 | 177 | 314 |
| `H300_tanB2p0` | random_forest | strict_window_fa<=1 | 652 | **11** [0.0, 31.0] (0.017) | **9** [0.0, 27.0] | 86 | 108 | 446 |
| `H300_tanB2p5` | threshold_rule | episode_fa<=1 (k=3,m=3) | 667 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 127 | 113 | 423 |
| `H300_tanB2p5` | threshold_rule | strict_window_fa<=1 | 667 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 127 | 113 | 423 |
| `H300_tanB2p5` | logistic_regression | episode_fa<=1 (k=3,m=3) | 667 | **1** [0.0, 3.0] (0.002) | **0** [0.0, 0.0] | 83 | 215 | 364 |
| `H300_tanB2p5` | logistic_regression | strict_window_fa<=1 | 667 | **1** [0.0, 3.0] (0.002) | **0** [0.0, 0.0] | 50 | 133 | 479 |
| `H300_tanB2p5` | random_forest | episode_fa<=1 (k=3,m=3) | 667 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 177 | 221 | 266 |
| `H300_tanB2p5` | random_forest | strict_window_fa<=1 | 667 | **0** [0.0, 0.0] (0.000) | **0** [0.0, 0.0] | 128 | 161 | 375 |
