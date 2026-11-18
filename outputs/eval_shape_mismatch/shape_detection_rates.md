# Run-Level Exact Detection & Missed-Event Rate by Shape (SYNTHETIC / SIMULATION)

> **SYNTHETIC / SIMULATION** — Model-mismatch stress test on synthetic mathematical surfaces; NOT field data and NOT validated on real data.

| shape | subset | model | regime | exact detect rate (95% CI) | missed-event rate (95% CI) |
|---|---|---|---|---|---|
| gaussian_control | all_events (60 runs) | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.483 [0.350, 0.617]** | 0.517 [0.383, 0.650] |
| gaussian_control | gradual (30 runs) | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.500 [0.333, 0.667]** | 0.500 [0.333, 0.684] |
| gaussian_control | rapid (30 runs) | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.467 [0.300, 0.633]** | 0.533 [0.367, 0.700] |
| gaussian_control | all_events (60 runs) | threshold_rule | strict_window_fa<=1 | **0.283 [0.183, 0.400]** | 0.717 [0.600, 0.833] |
| gaussian_control | gradual (30 runs) | threshold_rule | strict_window_fa<=1 | **0.233 [0.100, 0.384]** | 0.767 [0.633, 0.933] |
| gaussian_control | rapid (30 runs) | threshold_rule | strict_window_fa<=1 | **0.333 [0.149, 0.500]** | 0.667 [0.500, 0.833] |
| gaussian_control | all_events (60 runs) | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.467 [0.333, 0.600]** | 0.533 [0.417, 0.667] |
| gaussian_control | gradual (30 runs) | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.400 [0.233, 0.567]** | 0.600 [0.433, 0.767] |
| gaussian_control | rapid (30 runs) | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.533 [0.333, 0.700]** | 0.467 [0.300, 0.633] |
| gaussian_control | all_events (60 runs) | logistic_regression | strict_window_fa<=1 | **0.267 [0.167, 0.392]** | 0.733 [0.617, 0.850] |
| gaussian_control | gradual (30 runs) | logistic_regression | strict_window_fa<=1 | **0.233 [0.100, 0.367]** | 0.767 [0.633, 0.917] |
| gaussian_control | rapid (30 runs) | logistic_regression | strict_window_fa<=1 | **0.300 [0.149, 0.433]** | 0.700 [0.516, 0.867] |
| gaussian_control | all_events (60 runs) | random_forest | episode_fa<=1 (k=3,m=3) | **0.617 [0.500, 0.733]** | 0.383 [0.250, 0.500] |
| gaussian_control | gradual (30 runs) | random_forest | episode_fa<=1 (k=3,m=3) | **0.600 [0.433, 0.767]** | 0.400 [0.233, 0.600] |
| gaussian_control | rapid (30 runs) | random_forest | episode_fa<=1 (k=3,m=3) | **0.633 [0.449, 0.800]** | 0.367 [0.200, 0.551] |
| gaussian_control | all_events (60 runs) | random_forest | strict_window_fa<=1 | **0.400 [0.275, 0.533]** | 0.600 [0.500, 0.750] |
| gaussian_control | gradual (30 runs) | random_forest | strict_window_fa<=1 | **0.367 [0.200, 0.533]** | 0.633 [0.467, 0.818] |
| gaussian_control | rapid (30 runs) | random_forest | strict_window_fa<=1 | **0.433 [0.267, 0.600]** | 0.567 [0.400, 0.733] |
| trough_panel | all_events (60 runs) | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.450 [0.333, 0.583]** | 0.550 [0.433, 0.659] |
| trough_panel | gradual (30 runs) | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.433 [0.249, 0.600]** | 0.567 [0.400, 0.767] |
| trough_panel | rapid (30 runs) | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.467 [0.267, 0.651]** | 0.533 [0.367, 0.700] |
| trough_panel | all_events (60 runs) | threshold_rule | strict_window_fa<=1 | **0.367 [0.250, 0.500]** | 0.633 [0.517, 0.750] |
| trough_panel | gradual (30 runs) | threshold_rule | strict_window_fa<=1 | **0.333 [0.167, 0.500]** | 0.667 [0.500, 0.833] |
| trough_panel | rapid (30 runs) | threshold_rule | strict_window_fa<=1 | **0.400 [0.233, 0.584]** | 0.600 [0.400, 0.767] |
| trough_panel | all_events (60 runs) | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.383 [0.267, 0.533]** | 0.617 [0.500, 0.733] |
| trough_panel | gradual (30 runs) | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.333 [0.167, 0.500]** | 0.667 [0.500, 0.833] |
| trough_panel | rapid (30 runs) | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.433 [0.267, 0.600]** | 0.567 [0.400, 0.733] |
| trough_panel | all_events (60 runs) | logistic_regression | strict_window_fa<=1 | **0.183 [0.091, 0.283]** | 0.817 [0.725, 0.917] |
| trough_panel | gradual (30 runs) | logistic_regression | strict_window_fa<=1 | **0.067 [0.000, 0.167]** | 0.933 [0.833, 1.000] |
| trough_panel | rapid (30 runs) | logistic_regression | strict_window_fa<=1 | **0.300 [0.133, 0.433]** | 0.700 [0.533, 0.851] |
| trough_panel | all_events (60 runs) | random_forest | episode_fa<=1 (k=3,m=3) | **0.533 [0.417, 0.659]** | 0.467 [0.325, 0.600] |
| trough_panel | gradual (30 runs) | random_forest | episode_fa<=1 (k=3,m=3) | **0.567 [0.400, 0.733]** | 0.433 [0.267, 0.633] |
| trough_panel | rapid (30 runs) | random_forest | episode_fa<=1 (k=3,m=3) | **0.500 [0.333, 0.667]** | 0.500 [0.333, 0.667] |
| trough_panel | all_events (60 runs) | random_forest | strict_window_fa<=1 | **0.250 [0.141, 0.367]** | 0.750 [0.650, 0.859] |
| trough_panel | gradual (30 runs) | random_forest | strict_window_fa<=1 | **0.167 [0.049, 0.300]** | 0.833 [0.700, 0.967] |
| trough_panel | rapid (30 runs) | random_forest | strict_window_fa<=1 | **0.333 [0.167, 0.500]** | 0.667 [0.500, 0.833] |
| asymmetric | all_events (60 runs) | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.433 [0.300, 0.567]** | 0.567 [0.441, 0.717] |
| asymmetric | gradual (30 runs) | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.467 [0.282, 0.633]** | 0.533 [0.367, 0.718] |
| asymmetric | rapid (30 runs) | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.400 [0.216, 0.600]** | 0.600 [0.433, 0.767] |
| asymmetric | all_events (60 runs) | threshold_rule | strict_window_fa<=1 | **0.317 [0.200, 0.433]** | 0.683 [0.567, 0.817] |
| asymmetric | gradual (30 runs) | threshold_rule | strict_window_fa<=1 | **0.300 [0.167, 0.467]** | 0.700 [0.549, 0.867] |
| asymmetric | rapid (30 runs) | threshold_rule | strict_window_fa<=1 | **0.333 [0.167, 0.500]** | 0.667 [0.500, 0.800] |
| asymmetric | all_events (60 runs) | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.450 [0.308, 0.575]** | 0.550 [0.417, 0.667] |
| asymmetric | gradual (30 runs) | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.367 [0.200, 0.533]** | 0.633 [0.467, 0.800] |
| asymmetric | rapid (30 runs) | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.533 [0.333, 0.700]** | 0.467 [0.300, 0.633] |
| asymmetric | all_events (60 runs) | logistic_regression | strict_window_fa<=1 | **0.267 [0.158, 0.383]** | 0.733 [0.633, 0.850] |
| asymmetric | gradual (30 runs) | logistic_regression | strict_window_fa<=1 | **0.133 [0.033, 0.267]** | 0.867 [0.767, 0.984] |
| asymmetric | rapid (30 runs) | logistic_regression | strict_window_fa<=1 | **0.400 [0.233, 0.551]** | 0.600 [0.433, 0.767] |
| asymmetric | all_events (60 runs) | random_forest | episode_fa<=1 (k=3,m=3) | **0.600 [0.483, 0.717]** | 0.400 [0.283, 0.517] |
| asymmetric | gradual (30 runs) | random_forest | episode_fa<=1 (k=3,m=3) | **0.600 [0.467, 0.767]** | 0.400 [0.233, 0.600] |
| asymmetric | rapid (30 runs) | random_forest | episode_fa<=1 (k=3,m=3) | **0.600 [0.433, 0.767]** | 0.400 [0.233, 0.533] |
| asymmetric | all_events (60 runs) | random_forest | strict_window_fa<=1 | **0.400 [0.275, 0.517]** | 0.600 [0.483, 0.733] |
| asymmetric | gradual (30 runs) | random_forest | strict_window_fa<=1 | **0.433 [0.249, 0.633]** | 0.567 [0.400, 0.751] |
| asymmetric | rapid (30 runs) | random_forest | strict_window_fa<=1 | **0.367 [0.200, 0.517]** | 0.633 [0.467, 0.800] |
| two_basin | all_events (60 runs) | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.467 [0.317, 0.609]** | 0.533 [0.400, 0.667] |
| two_basin | gradual (30 runs) | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.467 [0.300, 0.633]** | 0.533 [0.383, 0.733] |
| two_basin | rapid (30 runs) | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.467 [0.300, 0.667]** | 0.533 [0.367, 0.700] |
| two_basin | all_events (60 runs) | threshold_rule | strict_window_fa<=1 | **0.333 [0.208, 0.467]** | 0.667 [0.550, 0.783] |
| two_basin | gradual (30 runs) | threshold_rule | strict_window_fa<=1 | **0.300 [0.167, 0.467]** | 0.700 [0.567, 0.867] |
| two_basin | rapid (30 runs) | threshold_rule | strict_window_fa<=1 | **0.367 [0.200, 0.533]** | 0.633 [0.467, 0.800] |
| two_basin | all_events (60 runs) | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.367 [0.233, 0.483]** | 0.633 [0.508, 0.750] |
| two_basin | gradual (30 runs) | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.333 [0.167, 0.500]** | 0.667 [0.533, 0.800] |
| two_basin | rapid (30 runs) | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.400 [0.233, 0.551]** | 0.600 [0.433, 0.733] |
| two_basin | all_events (60 runs) | logistic_regression | strict_window_fa<=1 | **0.200 [0.100, 0.300]** | 0.800 [0.700, 0.900] |
| two_basin | gradual (30 runs) | logistic_regression | strict_window_fa<=1 | **0.133 [0.033, 0.267]** | 0.867 [0.767, 0.967] |
| two_basin | rapid (30 runs) | logistic_regression | strict_window_fa<=1 | **0.267 [0.133, 0.400]** | 0.733 [0.567, 0.867] |
| two_basin | all_events (60 runs) | random_forest | episode_fa<=1 (k=3,m=3) | **0.583 [0.450, 0.709]** | 0.417 [0.283, 0.550] |
| two_basin | gradual (30 runs) | random_forest | episode_fa<=1 (k=3,m=3) | **0.567 [0.400, 0.751]** | 0.433 [0.267, 0.633] |
| two_basin | rapid (30 runs) | random_forest | episode_fa<=1 (k=3,m=3) | **0.600 [0.400, 0.800]** | 0.400 [0.233, 0.584] |
| two_basin | all_events (60 runs) | random_forest | strict_window_fa<=1 | **0.400 [0.283, 0.525]** | 0.600 [0.483, 0.733] |
| two_basin | gradual (30 runs) | random_forest | strict_window_fa<=1 | **0.400 [0.233, 0.600]** | 0.600 [0.449, 0.800] |
| two_basin | rapid (30 runs) | random_forest | strict_window_fa<=1 | **0.400 [0.233, 0.567]** | 0.600 [0.400, 0.733] |
| planar_slope | all_events (60 runs) | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.633 [0.525, 0.750]** | 0.367 [0.250, 0.492] |
| planar_slope | gradual (30 runs) | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.700 [0.533, 0.833]** | 0.300 [0.149, 0.484] |
| planar_slope | rapid (30 runs) | threshold_rule | episode_fa<=1 (k=3,m=3) | **0.567 [0.400, 0.733]** | 0.433 [0.267, 0.600] |
| planar_slope | all_events (60 runs) | threshold_rule | strict_window_fa<=1 | **0.517 [0.391, 0.650]** | 0.483 [0.350, 0.617] |
| planar_slope | gradual (30 runs) | threshold_rule | strict_window_fa<=1 | **0.500 [0.367, 0.667]** | 0.500 [0.367, 0.667] |
| planar_slope | rapid (30 runs) | threshold_rule | strict_window_fa<=1 | **0.533 [0.367, 0.700]** | 0.467 [0.300, 0.633] |
| planar_slope | all_events (60 runs) | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.500 [0.367, 0.617]** | 0.500 [0.383, 0.633] |
| planar_slope | gradual (30 runs) | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.400 [0.249, 0.567]** | 0.600 [0.433, 0.767] |
| planar_slope | rapid (30 runs) | logistic_regression | episode_fa<=1 (k=3,m=3) | **0.600 [0.400, 0.767]** | 0.400 [0.233, 0.533] |
| planar_slope | all_events (60 runs) | logistic_regression | strict_window_fa<=1 | **0.300 [0.183, 0.417]** | 0.700 [0.600, 0.817] |
| planar_slope | gradual (30 runs) | logistic_regression | strict_window_fa<=1 | **0.233 [0.100, 0.400]** | 0.767 [0.600, 0.900] |
| planar_slope | rapid (30 runs) | logistic_regression | strict_window_fa<=1 | **0.367 [0.200, 0.533]** | 0.633 [0.467, 0.800] |
| planar_slope | all_events (60 runs) | random_forest | episode_fa<=1 (k=3,m=3) | **0.550 [0.417, 0.683]** | 0.450 [0.341, 0.567] |
| planar_slope | gradual (30 runs) | random_forest | episode_fa<=1 (k=3,m=3) | **0.467 [0.282, 0.651]** | 0.533 [0.367, 0.700] |
| planar_slope | rapid (30 runs) | random_forest | episode_fa<=1 (k=3,m=3) | **0.633 [0.433, 0.800]** | 0.367 [0.200, 0.517] |
| planar_slope | all_events (60 runs) | random_forest | strict_window_fa<=1 | **0.317 [0.200, 0.417]** | 0.683 [0.575, 0.809] |
| planar_slope | gradual (30 runs) | random_forest | strict_window_fa<=1 | **0.200 [0.067, 0.351]** | 0.800 [0.667, 0.933] |
| planar_slope | rapid (30 runs) | random_forest | strict_window_fa<=1 | **0.433 [0.233, 0.618]** | 0.567 [0.400, 0.733] |
