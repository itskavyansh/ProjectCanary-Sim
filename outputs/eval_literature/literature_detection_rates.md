# Run-Level Exact Detection & Missed-Event Rates Across B1 and B2 Arms (SYNTHETIC / SIMULATION)

> **SYNTHETIC / SIMULATION** — Literature-basis sensitivity checks on frozen v3 models; nothing here is validated on real data.

| arm | subset | runs | model | regime | exact detect rate [95% CI] | missed-event rate [95% CI] |
|---|---|---:|---|---|---|---|
| `gaussian_control` | all_events | 60 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.483 [0.350, 0.592]** | 0.517 [0.383, 0.633] |
| `gaussian_control` | gradual | 30 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.500 [0.333, 0.700]** | 0.500 [0.333, 0.684] |
| `gaussian_control` | rapid | 30 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.467 [0.300, 0.667]** | 0.533 [0.367, 0.700] |
| `gaussian_control` | all_events | 60 | threshold_rule | strict_window_fa<=1 | **0.283 [0.167, 0.392]** | 0.717 [0.600, 0.817] |
| `gaussian_control` | gradual | 30 | threshold_rule | strict_window_fa<=1 | **0.233 [0.067, 0.400]** | 0.767 [0.600, 0.900] |
| `gaussian_control` | rapid | 30 | threshold_rule | strict_window_fa<=1 | **0.333 [0.167, 0.500]** | 0.667 [0.500, 0.833] |
| `gaussian_control` | all_events | 60 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.467 [0.325, 0.583]** | 0.533 [0.400, 0.659] |
| `gaussian_control` | gradual | 30 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.400 [0.267, 0.567]** | 0.600 [0.433, 0.767] |
| `gaussian_control` | rapid | 30 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.533 [0.333, 0.700]** | 0.467 [0.267, 0.633] |
| `gaussian_control` | all_events | 60 | logistic_regression | strict_window_fa<=1 | **0.267 [0.167, 0.383]** | 0.733 [0.617, 0.833] |
| `gaussian_control` | gradual | 30 | logistic_regression | strict_window_fa<=1 | **0.233 [0.100, 0.400]** | 0.767 [0.600, 0.900] |
| `gaussian_control` | rapid | 30 | logistic_regression | strict_window_fa<=1 | **0.300 [0.167, 0.467]** | 0.700 [0.533, 0.867] |
| `gaussian_control` | all_events | 60 | random_forest | episode_fa<=1 (k=3,m=3) | **0.617 [0.491, 0.742]** | 0.383 [0.250, 0.500] |
| `gaussian_control` | gradual | 30 | random_forest | episode_fa<=1 (k=3,m=3) | **0.600 [0.433, 0.767]** | 0.400 [0.233, 0.600] |
| `gaussian_control` | rapid | 30 | random_forest | episode_fa<=1 (k=3,m=3) | **0.633 [0.467, 0.800]** | 0.367 [0.200, 0.517] |
| `gaussian_control` | all_events | 60 | random_forest | strict_window_fa<=1 | **0.400 [0.267, 0.517]** | 0.600 [0.483, 0.717] |
| `gaussian_control` | gradual | 30 | random_forest | strict_window_fa<=1 | **0.367 [0.233, 0.551]** | 0.633 [0.500, 0.800] |
| `gaussian_control` | rapid | 30 | random_forest | strict_window_fa<=1 | **0.433 [0.267, 0.600]** | 0.567 [0.383, 0.733] |
| `high_tilt_3_6` | all_events | 60 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.650 [0.533, 0.783]** | 0.350 [0.217, 0.475] |
| `high_tilt_3_6` | gradual | 30 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.633 [0.467, 0.800]** | 0.367 [0.200, 0.533] |
| `high_tilt_3_6` | rapid | 30 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.667 [0.500, 0.818]** | 0.333 [0.167, 0.500] |
| `high_tilt_3_6` | all_events | 60 | threshold_rule | strict_window_fa<=1 | **0.517 [0.408, 0.633]** | 0.483 [0.350, 0.600] |
| `high_tilt_3_6` | gradual | 30 | threshold_rule | strict_window_fa<=1 | **0.533 [0.349, 0.733]** | 0.467 [0.267, 0.667] |
| `high_tilt_3_6` | rapid | 30 | threshold_rule | strict_window_fa<=1 | **0.500 [0.333, 0.667]** | 0.500 [0.333, 0.667] |
| `high_tilt_3_6` | all_events | 60 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.583 [0.467, 0.700]** | 0.417 [0.300, 0.542] |
| `high_tilt_3_6` | gradual | 30 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.600 [0.433, 0.800]** | 0.400 [0.233, 0.567] |
| `high_tilt_3_6` | rapid | 30 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.567 [0.400, 0.751]** | 0.433 [0.267, 0.600] |
| `high_tilt_3_6` | all_events | 60 | logistic_regression | strict_window_fa<=1 | **0.400 [0.267, 0.525]** | 0.600 [0.483, 0.717] |
| `high_tilt_3_6` | gradual | 30 | logistic_regression | strict_window_fa<=1 | **0.467 [0.282, 0.651]** | 0.533 [0.367, 0.718] |
| `high_tilt_3_6` | rapid | 30 | logistic_regression | strict_window_fa<=1 | **0.333 [0.167, 0.484]** | 0.667 [0.500, 0.833] |
| `high_tilt_3_6` | all_events | 60 | random_forest | episode_fa<=1 (k=3,m=3) | **0.767 [0.667, 0.867]** | 0.233 [0.133, 0.350] |
| `high_tilt_3_6` | gradual | 30 | random_forest | episode_fa<=1 (k=3,m=3) | **0.633 [0.449, 0.800]** | 0.367 [0.233, 0.567] |
| `high_tilt_3_6` | rapid | 30 | random_forest | episode_fa<=1 (k=3,m=3) | **0.900 [0.782, 1.000]** | 0.100 [0.000, 0.217] |
| `high_tilt_3_6` | all_events | 60 | random_forest | strict_window_fa<=1 | **0.733 [0.633, 0.850]** | 0.267 [0.167, 0.375] |
| `high_tilt_3_6` | gradual | 30 | random_forest | strict_window_fa<=1 | **0.633 [0.449, 0.800]** | 0.367 [0.233, 0.567] |
| `high_tilt_3_6` | rapid | 30 | random_forest | strict_window_fa<=1 | **0.833 [0.700, 0.967]** | 0.167 [0.067, 0.300] |
| `high_tilt_6_12` | all_events | 60 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.367 [0.250, 0.483]** | 0.633 [0.517, 0.750] |
| `high_tilt_6_12` | gradual | 30 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.667 [0.500, 0.800]** | 0.333 [0.167, 0.500] |
| `high_tilt_6_12` | rapid | 30 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.067 [0.000, 0.167]** | 0.933 [0.833, 1.000] |
| `high_tilt_6_12` | all_events | 60 | threshold_rule | strict_window_fa<=1 | **0.100 [0.033, 0.183]** | 0.900 [0.817, 0.967] |
| `high_tilt_6_12` | gradual | 30 | threshold_rule | strict_window_fa<=1 | **0.200 [0.067, 0.333]** | 0.800 [0.649, 0.933] |
| `high_tilt_6_12` | rapid | 30 | threshold_rule | strict_window_fa<=1 | **0.000 [0.000, 0.000]** | 1.000 [1.000, 1.000] |
| `high_tilt_6_12` | all_events | 60 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.500 [0.383, 0.633]** | 0.500 [0.383, 0.617] |
| `high_tilt_6_12` | gradual | 30 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.700 [0.533, 0.833]** | 0.300 [0.133, 0.467] |
| `high_tilt_6_12` | rapid | 30 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.300 [0.149, 0.467]** | 0.700 [0.533, 0.867] |
| `high_tilt_6_12` | all_events | 60 | logistic_regression | strict_window_fa<=1 | **0.417 [0.300, 0.550]** | 0.583 [0.467, 0.700] |
| `high_tilt_6_12` | gradual | 30 | logistic_regression | strict_window_fa<=1 | **0.667 [0.500, 0.818]** | 0.333 [0.167, 0.500] |
| `high_tilt_6_12` | rapid | 30 | logistic_regression | strict_window_fa<=1 | **0.167 [0.049, 0.300]** | 0.833 [0.700, 0.933] |
| `high_tilt_6_12` | all_events | 60 | random_forest | episode_fa<=1 (k=3,m=3) | **0.767 [0.667, 0.875]** | 0.233 [0.133, 0.342] |
| `high_tilt_6_12` | gradual | 30 | random_forest | episode_fa<=1 (k=3,m=3) | **0.633 [0.467, 0.767]** | 0.367 [0.200, 0.567] |
| `high_tilt_6_12` | rapid | 30 | random_forest | episode_fa<=1 (k=3,m=3) | **0.900 [0.800, 1.000]** | 0.100 [0.000, 0.200] |
| `high_tilt_6_12` | all_events | 60 | random_forest | strict_window_fa<=1 | **0.667 [0.550, 0.783]** | 0.333 [0.217, 0.450] |
| `high_tilt_6_12` | gradual | 30 | random_forest | strict_window_fa<=1 | **0.467 [0.300, 0.633]** | 0.533 [0.349, 0.733] |
| `high_tilt_6_12` | rapid | 30 | random_forest | strict_window_fa<=1 | **0.867 [0.767, 0.967]** | 0.133 [0.033, 0.267] |
| `depth_all_gt_1p5` | all_events | 140 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.486 [0.396, 0.564]** | 0.514 [0.436, 0.604] |
| `depth_all_gt_1p5` | gradual | 70 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.514 [0.400, 0.629]** | 0.486 [0.357, 0.600] |
| `depth_all_gt_1p5` | rapid | 70 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.457 [0.357, 0.571]** | 0.543 [0.414, 0.657] |
| `depth_all_gt_1p5` | all_events | 140 | threshold_rule | strict_window_fa<=1 | **0.343 [0.264, 0.432]** | 0.657 [0.586, 0.743] |
| `depth_all_gt_1p5` | gradual | 70 | threshold_rule | strict_window_fa<=1 | **0.314 [0.214, 0.414]** | 0.686 [0.586, 0.800] |
| `depth_all_gt_1p5` | rapid | 70 | threshold_rule | strict_window_fa<=1 | **0.371 [0.271, 0.479]** | 0.629 [0.514, 0.729] |
| `depth_all_gt_1p5` | all_events | 140 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.464 [0.379, 0.550]** | 0.536 [0.450, 0.614] |
| `depth_all_gt_1p5` | gradual | 70 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.257 [0.157, 0.357]** | 0.743 [0.650, 0.843] |
| `depth_all_gt_1p5` | rapid | 70 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.671 [0.571, 0.771]** | 0.329 [0.229, 0.443] |
| `depth_all_gt_1p5` | all_events | 140 | logistic_regression | strict_window_fa<=1 | **0.279 [0.203, 0.364]** | 0.721 [0.639, 0.793] |
| `depth_all_gt_1p5` | gradual | 70 | logistic_regression | strict_window_fa<=1 | **0.143 [0.071, 0.229]** | 0.857 [0.771, 0.943] |
| `depth_all_gt_1p5` | rapid | 70 | logistic_regression | strict_window_fa<=1 | **0.414 [0.314, 0.536]** | 0.586 [0.471, 0.700] |
| `depth_all_gt_1p5` | all_events | 140 | random_forest | episode_fa<=1 (k=3,m=3) | **0.629 [0.550, 0.700]** | 0.371 [0.293, 0.443] |
| `depth_all_gt_1p5` | gradual | 70 | random_forest | episode_fa<=1 (k=3,m=3) | **0.571 [0.450, 0.686]** | 0.429 [0.300, 0.543] |
| `depth_all_gt_1p5` | rapid | 70 | random_forest | episode_fa<=1 (k=3,m=3) | **0.686 [0.571, 0.771]** | 0.314 [0.214, 0.429] |
| `depth_all_gt_1p5` | all_events | 140 | random_forest | strict_window_fa<=1 | **0.521 [0.439, 0.611]** | 0.479 [0.393, 0.564] |
| `depth_all_gt_1p5` | gradual | 70 | random_forest | strict_window_fa<=1 | **0.471 [0.350, 0.579]** | 0.529 [0.400, 0.643] |
| `depth_all_gt_1p5` | rapid | 70 | random_forest | strict_window_fa<=1 | **0.571 [0.471, 0.686]** | 0.429 [0.307, 0.536] |
| `H100_tanB1p5` | all_events | 20 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.500 [0.250, 0.700]** | 0.500 [0.274, 0.700] |
| `H100_tanB1p5` | gradual | 10 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.600 [0.300, 0.900]** | 0.400 [0.100, 0.700] |
| `H100_tanB1p5` | rapid | 10 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.400 [0.100, 0.700]** | 0.600 [0.300, 0.900] |
| `H100_tanB1p5` | all_events | 20 | threshold_rule | strict_window_fa<=1 | **0.400 [0.200, 0.600]** | 0.600 [0.350, 0.800] |
| `H100_tanB1p5` | gradual | 10 | threshold_rule | strict_window_fa<=1 | **0.400 [0.100, 0.700]** | 0.600 [0.300, 0.900] |
| `H100_tanB1p5` | rapid | 10 | threshold_rule | strict_window_fa<=1 | **0.400 [0.100, 0.700]** | 0.600 [0.300, 0.900] |
| `H100_tanB1p5` | all_events | 20 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.500 [0.300, 0.726]** | 0.500 [0.250, 0.726] |
| `H100_tanB1p5` | gradual | 10 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.300 [0.000, 0.600]** | 0.700 [0.400, 0.953] |
| `H100_tanB1p5` | rapid | 10 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.700 [0.400, 0.900]** | 0.300 [0.000, 0.600] |
| `H100_tanB1p5` | all_events | 20 | logistic_regression | strict_window_fa<=1 | **0.300 [0.100, 0.500]** | 0.700 [0.500, 0.900] |
| `H100_tanB1p5` | gradual | 10 | logistic_regression | strict_window_fa<=1 | **0.100 [0.000, 0.300]** | 0.900 [0.700, 1.000] |
| `H100_tanB1p5` | rapid | 10 | logistic_regression | strict_window_fa<=1 | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H100_tanB1p5` | all_events | 20 | random_forest | episode_fa<=1 (k=3,m=3) | **0.700 [0.450, 0.900]** | 0.300 [0.100, 0.500] |
| `H100_tanB1p5` | gradual | 10 | random_forest | episode_fa<=1 (k=3,m=3) | **0.600 [0.300, 0.900]** | 0.400 [0.100, 0.700] |
| `H100_tanB1p5` | rapid | 10 | random_forest | episode_fa<=1 (k=3,m=3) | **0.800 [0.500, 1.000]** | 0.200 [0.000, 0.500] |
| `H100_tanB1p5` | all_events | 20 | random_forest | strict_window_fa<=1 | **0.650 [0.450, 0.850]** | 0.350 [0.100, 0.550] |
| `H100_tanB1p5` | gradual | 10 | random_forest | strict_window_fa<=1 | **0.600 [0.300, 0.900]** | 0.400 [0.100, 0.700] |
| `H100_tanB1p5` | rapid | 10 | random_forest | strict_window_fa<=1 | **0.700 [0.400, 0.900]** | 0.300 [0.000, 0.600] |
| `H200_tanB1p5` | all_events | 20 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.650 [0.500, 0.800]** | 0.350 [0.150, 0.500] |
| `H200_tanB1p5` | gradual | 10 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.700 [0.400, 1.000]** | 0.300 [0.100, 0.600] |
| `H200_tanB1p5` | rapid | 10 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.600 [0.300, 0.900]** | 0.400 [0.100, 0.700] |
| `H200_tanB1p5` | all_events | 20 | threshold_rule | strict_window_fa<=1 | **0.350 [0.150, 0.550]** | 0.650 [0.450, 0.850] |
| `H200_tanB1p5` | gradual | 10 | threshold_rule | strict_window_fa<=1 | **0.300 [0.000, 0.600]** | 0.700 [0.400, 0.953] |
| `H200_tanB1p5` | rapid | 10 | threshold_rule | strict_window_fa<=1 | **0.400 [0.100, 0.800]** | 0.600 [0.300, 0.900] |
| `H200_tanB1p5` | all_events | 20 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.500 [0.300, 0.750]** | 0.500 [0.300, 0.700] |
| `H200_tanB1p5` | gradual | 10 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.400 [0.100, 0.700]** | 0.600 [0.300, 0.900] |
| `H200_tanB1p5` | rapid | 10 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.600 [0.300, 0.900]** | 0.400 [0.100, 0.700] |
| `H200_tanB1p5` | all_events | 20 | logistic_regression | strict_window_fa<=1 | **0.250 [0.100, 0.450]** | 0.750 [0.550, 0.900] |
| `H200_tanB1p5` | gradual | 10 | logistic_regression | strict_window_fa<=1 | **0.100 [0.000, 0.300]** | 0.900 [0.700, 1.000] |
| `H200_tanB1p5` | rapid | 10 | logistic_regression | strict_window_fa<=1 | **0.400 [0.100, 0.752]** | 0.600 [0.347, 0.900] |
| `H200_tanB1p5` | all_events | 20 | random_forest | episode_fa<=1 (k=3,m=3) | **0.650 [0.450, 0.850]** | 0.350 [0.150, 0.550] |
| `H200_tanB1p5` | gradual | 10 | random_forest | episode_fa<=1 (k=3,m=3) | **0.600 [0.300, 0.900]** | 0.400 [0.100, 0.700] |
| `H200_tanB1p5` | rapid | 10 | random_forest | episode_fa<=1 (k=3,m=3) | **0.700 [0.400, 0.953]** | 0.300 [0.100, 0.600] |
| `H200_tanB1p5` | all_events | 20 | random_forest | strict_window_fa<=1 | **0.600 [0.400, 0.800]** | 0.400 [0.174, 0.600] |
| `H200_tanB1p5` | gradual | 10 | random_forest | strict_window_fa<=1 | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H200_tanB1p5` | rapid | 10 | random_forest | strict_window_fa<=1 | **0.700 [0.400, 0.953]** | 0.300 [0.100, 0.600] |
| `H200_tanB2p0` | all_events | 20 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.500 [0.300, 0.700]** | 0.500 [0.350, 0.700] |
| `H200_tanB2p0` | gradual | 10 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H200_tanB2p0` | rapid | 10 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H200_tanB2p0` | all_events | 20 | threshold_rule | strict_window_fa<=1 | **0.250 [0.100, 0.450]** | 0.750 [0.574, 0.900] |
| `H200_tanB2p0` | gradual | 10 | threshold_rule | strict_window_fa<=1 | **0.200 [0.000, 0.400]** | 0.800 [0.500, 1.000] |
| `H200_tanB2p0` | rapid | 10 | threshold_rule | strict_window_fa<=1 | **0.300 [0.000, 0.600]** | 0.700 [0.400, 1.000] |
| `H200_tanB2p0` | all_events | 20 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.550 [0.300, 0.750]** | 0.450 [0.250, 0.676] |
| `H200_tanB2p0` | gradual | 10 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.400 [0.100, 0.700]** | 0.600 [0.300, 0.900] |
| `H200_tanB2p0` | rapid | 10 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.700 [0.400, 0.953]** | 0.300 [0.000, 0.600] |
| `H200_tanB2p0` | all_events | 20 | logistic_regression | strict_window_fa<=1 | **0.350 [0.100, 0.550]** | 0.650 [0.450, 0.850] |
| `H200_tanB2p0` | gradual | 10 | logistic_regression | strict_window_fa<=1 | **0.300 [0.048, 0.600]** | 0.700 [0.400, 1.000] |
| `H200_tanB2p0` | rapid | 10 | logistic_regression | strict_window_fa<=1 | **0.400 [0.100, 0.700]** | 0.600 [0.300, 0.900] |
| `H200_tanB2p0` | all_events | 20 | random_forest | episode_fa<=1 (k=3,m=3) | **0.600 [0.350, 0.800]** | 0.400 [0.200, 0.650] |
| `H200_tanB2p0` | gradual | 10 | random_forest | episode_fa<=1 (k=3,m=3) | **0.700 [0.400, 0.900]** | 0.300 [0.000, 0.600] |
| `H200_tanB2p0` | rapid | 10 | random_forest | episode_fa<=1 (k=3,m=3) | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H200_tanB2p0` | all_events | 20 | random_forest | strict_window_fa<=1 | **0.500 [0.300, 0.700]** | 0.500 [0.300, 0.726] |
| `H200_tanB2p0` | gradual | 10 | random_forest | strict_window_fa<=1 | **0.500 [0.147, 0.800]** | 0.500 [0.200, 0.800] |
| `H200_tanB2p0` | rapid | 10 | random_forest | strict_window_fa<=1 | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H200_tanB2p5` | all_events | 20 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.450 [0.250, 0.700]** | 0.550 [0.324, 0.750] |
| `H200_tanB2p5` | gradual | 10 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H200_tanB2p5` | rapid | 10 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.400 [0.100, 0.752]** | 0.600 [0.300, 0.900] |
| `H200_tanB2p5` | all_events | 20 | threshold_rule | strict_window_fa<=1 | **0.450 [0.250, 0.700]** | 0.550 [0.324, 0.750] |
| `H200_tanB2p5` | gradual | 10 | threshold_rule | strict_window_fa<=1 | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H200_tanB2p5` | rapid | 10 | threshold_rule | strict_window_fa<=1 | **0.400 [0.100, 0.752]** | 0.600 [0.300, 0.900] |
| `H200_tanB2p5` | all_events | 20 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.500 [0.300, 0.700]** | 0.500 [0.300, 0.700] |
| `H200_tanB2p5` | gradual | 10 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.300 [0.000, 0.600]** | 0.700 [0.400, 1.000] |
| `H200_tanB2p5` | rapid | 10 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.700 [0.400, 1.000]** | 0.300 [0.100, 0.600] |
| `H200_tanB2p5` | all_events | 20 | logistic_regression | strict_window_fa<=1 | **0.350 [0.124, 0.550]** | 0.650 [0.450, 0.850] |
| `H200_tanB2p5` | gradual | 10 | logistic_regression | strict_window_fa<=1 | **0.200 [0.000, 0.500]** | 0.800 [0.600, 1.000] |
| `H200_tanB2p5` | rapid | 10 | logistic_regression | strict_window_fa<=1 | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H200_tanB2p5` | all_events | 20 | random_forest | episode_fa<=1 (k=3,m=3) | **0.650 [0.450, 0.850]** | 0.350 [0.150, 0.576] |
| `H200_tanB2p5` | gradual | 10 | random_forest | episode_fa<=1 (k=3,m=3) | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H200_tanB2p5` | rapid | 10 | random_forest | episode_fa<=1 (k=3,m=3) | **0.800 [0.500, 1.000]** | 0.200 [0.000, 0.500] |
| `H200_tanB2p5` | all_events | 20 | random_forest | strict_window_fa<=1 | **0.550 [0.324, 0.750]** | 0.450 [0.200, 0.700] |
| `H200_tanB2p5` | gradual | 10 | random_forest | strict_window_fa<=1 | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H200_tanB2p5` | rapid | 10 | random_forest | strict_window_fa<=1 | **0.600 [0.300, 0.900]** | 0.400 [0.100, 0.700] |
| `H300_tanB1p5` | all_events | 20 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.350 [0.150, 0.550]** | 0.650 [0.450, 0.850] |
| `H300_tanB1p5` | gradual | 10 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.400 [0.100, 0.700]** | 0.600 [0.300, 0.900] |
| `H300_tanB1p5` | rapid | 10 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.300 [0.100, 0.600]** | 0.700 [0.400, 0.953] |
| `H300_tanB1p5` | all_events | 20 | threshold_rule | strict_window_fa<=1 | **0.300 [0.100, 0.500]** | 0.700 [0.500, 0.900] |
| `H300_tanB1p5` | gradual | 10 | threshold_rule | strict_window_fa<=1 | **0.300 [0.000, 0.600]** | 0.700 [0.400, 1.000] |
| `H300_tanB1p5` | rapid | 10 | threshold_rule | strict_window_fa<=1 | **0.300 [0.100, 0.600]** | 0.700 [0.400, 0.953] |
| `H300_tanB1p5` | all_events | 20 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.200 [0.050, 0.350]** | 0.800 [0.624, 0.950] |
| `H300_tanB1p5` | gradual | 10 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.000 [0.000, 0.000]** | 1.000 [1.000, 1.000] |
| `H300_tanB1p5` | rapid | 10 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.400 [0.100, 0.700]** | 0.600 [0.300, 0.900] |
| `H300_tanB1p5` | all_events | 20 | logistic_regression | strict_window_fa<=1 | **0.150 [0.000, 0.350]** | 0.850 [0.700, 0.950] |
| `H300_tanB1p5` | gradual | 10 | logistic_regression | strict_window_fa<=1 | **0.000 [0.000, 0.000]** | 1.000 [1.000, 1.000] |
| `H300_tanB1p5` | rapid | 10 | logistic_regression | strict_window_fa<=1 | **0.300 [0.048, 0.600]** | 0.700 [0.400, 0.900] |
| `H300_tanB1p5` | all_events | 20 | random_forest | episode_fa<=1 (k=3,m=3) | **0.500 [0.250, 0.700]** | 0.500 [0.300, 0.750] |
| `H300_tanB1p5` | gradual | 10 | random_forest | episode_fa<=1 (k=3,m=3) | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H300_tanB1p5` | rapid | 10 | random_forest | episode_fa<=1 (k=3,m=3) | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H300_tanB1p5` | all_events | 20 | random_forest | strict_window_fa<=1 | **0.400 [0.200, 0.600]** | 0.600 [0.400, 0.800] |
| `H300_tanB1p5` | gradual | 10 | random_forest | strict_window_fa<=1 | **0.400 [0.100, 0.700]** | 0.600 [0.300, 0.900] |
| `H300_tanB1p5` | rapid | 10 | random_forest | strict_window_fa<=1 | **0.400 [0.100, 0.700]** | 0.600 [0.300, 0.900] |
| `H300_tanB2p0` | all_events | 20 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.450 [0.200, 0.650]** | 0.550 [0.300, 0.750] |
| `H300_tanB2p0` | gradual | 10 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.400 [0.100, 0.800]** | 0.600 [0.300, 0.900] |
| `H300_tanB2p0` | rapid | 10 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H300_tanB2p0` | all_events | 20 | threshold_rule | strict_window_fa<=1 | **0.300 [0.100, 0.500]** | 0.700 [0.474, 0.850] |
| `H300_tanB2p0` | gradual | 10 | threshold_rule | strict_window_fa<=1 | **0.200 [0.000, 0.500]** | 0.800 [0.500, 1.000] |
| `H300_tanB2p0` | rapid | 10 | threshold_rule | strict_window_fa<=1 | **0.400 [0.100, 0.700]** | 0.600 [0.300, 0.900] |
| `H300_tanB2p0` | all_events | 20 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.500 [0.250, 0.700]** | 0.500 [0.274, 0.700] |
| `H300_tanB2p0` | gradual | 10 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.200 [0.000, 0.500]** | 0.800 [0.600, 1.000] |
| `H300_tanB2p0` | rapid | 10 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.800 [0.500, 1.000]** | 0.200 [0.000, 0.500] |
| `H300_tanB2p0` | all_events | 20 | logistic_regression | strict_window_fa<=1 | **0.250 [0.100, 0.450]** | 0.750 [0.550, 0.900] |
| `H300_tanB2p0` | gradual | 10 | logistic_regression | strict_window_fa<=1 | **0.100 [0.000, 0.300]** | 0.900 [0.700, 1.000] |
| `H300_tanB2p0` | rapid | 10 | logistic_regression | strict_window_fa<=1 | **0.400 [0.100, 0.700]** | 0.600 [0.300, 0.900] |
| `H300_tanB2p0` | all_events | 20 | random_forest | episode_fa<=1 (k=3,m=3) | **0.650 [0.450, 0.826]** | 0.350 [0.150, 0.550] |
| `H300_tanB2p0` | gradual | 10 | random_forest | episode_fa<=1 (k=3,m=3) | **0.600 [0.300, 0.900]** | 0.400 [0.100, 0.700] |
| `H300_tanB2p0` | rapid | 10 | random_forest | episode_fa<=1 (k=3,m=3) | **0.700 [0.400, 0.900]** | 0.300 [0.000, 0.600] |
| `H300_tanB2p0` | all_events | 20 | random_forest | strict_window_fa<=1 | **0.400 [0.200, 0.600]** | 0.600 [0.400, 0.800] |
| `H300_tanB2p0` | gradual | 10 | random_forest | strict_window_fa<=1 | **0.300 [0.000, 0.600]** | 0.700 [0.400, 1.000] |
| `H300_tanB2p0` | rapid | 10 | random_forest | strict_window_fa<=1 | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H300_tanB2p5` | all_events | 20 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.500 [0.300, 0.700]** | 0.500 [0.250, 0.700] |
| `H300_tanB2p5` | gradual | 10 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H300_tanB2p5` | rapid | 10 | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H300_tanB2p5` | all_events | 20 | threshold_rule | strict_window_fa<=1 | **0.350 [0.200, 0.550]** | 0.650 [0.400, 0.850] |
| `H300_tanB2p5` | gradual | 10 | threshold_rule | strict_window_fa<=1 | **0.300 [0.000, 0.600]** | 0.700 [0.400, 0.900] |
| `H300_tanB2p5` | rapid | 10 | threshold_rule | strict_window_fa<=1 | **0.400 [0.100, 0.700]** | 0.600 [0.300, 0.900] |
| `H300_tanB2p5` | all_events | 20 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.500 [0.300, 0.700]** | 0.500 [0.250, 0.700] |
| `H300_tanB2p5` | gradual | 10 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.200 [0.000, 0.400]** | 0.800 [0.600, 1.000] |
| `H300_tanB2p5` | rapid | 10 | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.800 [0.500, 1.000]** | 0.200 [0.000, 0.500] |
| `H300_tanB2p5` | all_events | 20 | logistic_regression | strict_window_fa<=1 | **0.300 [0.100, 0.500]** | 0.700 [0.500, 0.900] |
| `H300_tanB2p5` | gradual | 10 | logistic_regression | strict_window_fa<=1 | **0.200 [0.000, 0.400]** | 0.800 [0.600, 1.000] |
| `H300_tanB2p5` | rapid | 10 | logistic_regression | strict_window_fa<=1 | **0.400 [0.100, 0.752]** | 0.600 [0.300, 0.900] |
| `H300_tanB2p5` | all_events | 20 | random_forest | episode_fa<=1 (k=3,m=3) | **0.650 [0.400, 0.850]** | 0.350 [0.150, 0.576] |
| `H300_tanB2p5` | gradual | 10 | random_forest | episode_fa<=1 (k=3,m=3) | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H300_tanB2p5` | rapid | 10 | random_forest | episode_fa<=1 (k=3,m=3) | **0.800 [0.500, 1.000]** | 0.200 [0.000, 0.453] |
| `H300_tanB2p5` | all_events | 20 | random_forest | strict_window_fa<=1 | **0.550 [0.350, 0.750]** | 0.450 [0.250, 0.676] |
| `H300_tanB2p5` | gradual | 10 | random_forest | strict_window_fa<=1 | **0.500 [0.200, 0.800]** | 0.500 [0.200, 0.800] |
| `H300_tanB2p5` | rapid | 10 | random_forest | strict_window_fa<=1 | **0.600 [0.200, 0.900]** | 0.400 [0.100, 0.700] |
