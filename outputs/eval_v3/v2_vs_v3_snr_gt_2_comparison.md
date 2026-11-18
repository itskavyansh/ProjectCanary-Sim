# v2_vs_v3_snr_gt_2_comparison (SYNTHETIC / SIMULATION)

| split | version | regime | model | n_runs | window_macro_f1 | window_macro_f1_ci_lo | window_macro_f1_ci_hi | alarm_macro_f1 | alarm_macro_f1_ci_lo | alarm_macro_f1_ci_hi | gradual_window_recall | rapid_window_recall | sensor_fault_window_recall | gradual_run_alarm_detect_rate | all_events_run_alarm_detect_rate | fa_episodes_per_normal_run | fa_windows_per_normal_run | total_gradual_sf_confusions |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| test | v2 (old features) | raw (k=1) | threshold_rule | 99 | 0.702 | 0.6484 | 0.7368 | 0.702 | 0.6484 | 0.7368 | 0.276 | 0.5162 | 0.4541 | 1 | 0.8987 | 6.65 | 10.05 | 54 |
| test | v2 (old features) | episode_fa<=1 (k=3,m=3) | threshold_rule | 99 | 0.702 | 0.6484 | 0.7368 | 0.6891 | 0.633 | 0.7255 | 0.276 | 0.5162 | 0.4541 | 0.8 | 0.8354 | 0.6 | 5.6 | 54 |
| test | v2 (old features) | strict_window_fa<=1 | threshold_rule | 99 | 0.702 | 0.6484 | 0.7368 | 0.6749 | 0.6135 | 0.7204 | 0.276 | 0.5162 | 0.4541 | 0.6 | 0.8101 | 0.05 | 0.1 | 54 |
| test | v3 (new features) | raw (k=1) | threshold_rule | 99 | 0.7022 | 0.6511 | 0.7342 | 0.7022 | 0.6511 | 0.7342 | 0.2745 | 0.5086 | 0.4685 | 1 | 0.9114 | 6.75 | 10.05 | 47 |
| test | v3 (new features) | episode_fa<=1 (k=3,m=3) | threshold_rule | 99 | 0.7022 | 0.6511 | 0.7342 | 0.6908 | 0.6349 | 0.7263 | 0.2745 | 0.5086 | 0.4685 | 0.8 | 0.8481 | 0.6 | 5.6 | 47 |
| test | v3 (new features) | strict_window_fa<=1 | threshold_rule | 99 | 0.7022 | 0.6511 | 0.7342 | 0.6756 | 0.614 | 0.721 | 0.2745 | 0.5086 | 0.4685 | 0.6 | 0.8101 | 0.05 | 0.1 | 47 |
| test | v2 (old features) | raw (k=1) | logistic_regression | 99 | 0.5514 | 0.511 | 0.5835 | 0.5514 | 0.511 | 0.5835 | 0.3665 | 0.5352 | 0.2613 | 0.9 | 0.962 | 22.65 | 42.45 | 132 |
| test | v2 (old features) | episode_fa<=1 (k=3,m=3) | logistic_regression | 99 | 0.6054 | 0.54 | 0.6515 | 0.5937 | 0.5175 | 0.6547 | 0.1448 | 0.3086 | 0.2108 | 0.4 | 0.6962 | 0.15 | 0.45 | 25 |
| test | v2 (old features) | strict_window_fa<=1 | logistic_regression | 99 | 0.5557 | 0.5029 | 0.6062 | 0.5329 | 0.4845 | 0.5844 | 0.0211 | 0.141 | 0.2036 | 0 | 0.6329 | 0 | 0 | 11 |
| test | v3 (new features) | raw (k=1) | logistic_regression | 99 | 0.5368 | 0.4939 | 0.5753 | 0.5368 | 0.4939 | 0.5753 | 0.2685 | 0.5219 | 0.3243 | 0.9 | 0.962 | 21.1 | 44.95 | 94 |
| test | v3 (new features) | episode_fa<=1 (k=3,m=3) | logistic_regression | 99 | 0.6164 | 0.5574 | 0.6775 | 0.6108 | 0.5455 | 0.6831 | 0.1403 | 0.4343 | 0.2306 | 0.5 | 0.7468 | 0.1 | 1 | 13 |
| test | v3 (new features) | strict_window_fa<=1 | logistic_regression | 99 | 0.5983 | 0.534 | 0.6674 | 0.5854 | 0.521 | 0.6508 | 0.0709 | 0.3105 | 0.218 | 0.2 | 0.6962 | 0 | 0 | 6 |
| test | v2 (old features) | raw (k=1) | random_forest | 99 | 0.6736 | 0.6145 | 0.7252 | 0.6736 | 0.6145 | 0.7252 | 0.4615 | 0.5257 | 0.4216 | 0.9 | 0.8987 | 10.95 | 30.05 | 92 |
| test | v2 (old features) | episode_fa<=1 (k=3,m=3) | random_forest | 99 | 0.691 | 0.623 | 0.7493 | 0.6795 | 0.6078 | 0.7446 | 0.2489 | 0.4057 | 0.4847 | 0.6 | 0.8228 | 0.6 | 3.95 | 25 |
| test | v2 (old features) | strict_window_fa<=1 | random_forest | 99 | 0.6872 | 0.6086 | 0.754 | 0.6714 | 0.5878 | 0.7449 | 0.1916 | 0.3752 | 0.436 | 0.3 | 0.7595 | 0.2 | 1.35 | 5 |
| test | v3 (new features) | raw (k=1) | random_forest | 99 | 0.6722 | 0.6153 | 0.7298 | 0.6722 | 0.6153 | 0.7298 | 0.279 | 0.5429 | 0.3856 | 0.8 | 0.8861 | 5.65 | 11.45 | 39 |
| test | v3 (new features) | episode_fa<=1 (k=3,m=3) | random_forest | 99 | 0.6725 | 0.6133 | 0.7265 | 0.6703 | 0.601 | 0.7302 | 0.2504 | 0.5371 | 0.4162 | 0.6 | 0.8228 | 0.65 | 5.2 | 30 |
| test | v3 (new features) | strict_window_fa<=1 | random_forest | 99 | 0.6825 | 0.6189 | 0.743 | 0.6663 | 0.6006 | 0.7307 | 0.2006 | 0.4724 | 0.4342 | 0.5 | 0.7975 | 0.25 | 1.9 | 8 |
| shifted_test | v2 (old features) | raw (k=1) | threshold_rule | 71 | 0.6029 | 0.5411 | 0.6492 | 0.6029 | 0.5411 | 0.6492 | 0.3736 | 0.677 | 0.4335 | 1 | 0.8929 | 29.667 | 43.667 | 67 |
| shifted_test | v2 (old features) | episode_fa<=1 (k=3,m=3) | threshold_rule | 71 | 0.6029 | 0.5411 | 0.6492 | 0.6068 | 0.5373 | 0.6597 | 0.3736 | 0.677 | 0.4335 | 1 | 0.875 | 2.467 | 21.467 | 67 |
| shifted_test | v2 (old features) | strict_window_fa<=1 | threshold_rule | 71 | 0.6029 | 0.5411 | 0.6492 | 0.6481 | 0.5721 | 0.7002 | 0.3736 | 0.677 | 0.4335 | 0.8 | 0.8393 | 0.2 | 1.667 | 67 |
| shifted_test | v3 (new features) | raw (k=1) | threshold_rule | 71 | 0.608 | 0.5545 | 0.6497 | 0.608 | 0.5545 | 0.6497 | 0.3621 | 0.6938 | 0.4787 | 1 | 0.9286 | 29.8 | 43.667 | 75 |
| shifted_test | v3 (new features) | episode_fa<=1 (k=3,m=3) | threshold_rule | 71 | 0.608 | 0.5545 | 0.6497 | 0.6218 | 0.5592 | 0.6806 | 0.3621 | 0.6938 | 0.4787 | 1 | 0.8929 | 2.467 | 21.467 | 75 |
| shifted_test | v3 (new features) | strict_window_fa<=1 | threshold_rule | 71 | 0.608 | 0.5545 | 0.6497 | 0.6529 | 0.5793 | 0.7069 | 0.3621 | 0.6938 | 0.4787 | 0.8 | 0.8393 | 0.2 | 1.667 | 75 |
| shifted_test | v2 (old features) | raw (k=1) | logistic_regression | 71 | 0.439 | 0.4144 | 0.4636 | 0.439 | 0.4144 | 0.4636 | 0.681 | 0.1236 | 0.3138 | 1 | 0.9643 | 33.133 | 77.467 | 186 |
| shifted_test | v2 (old features) | episode_fa<=1 (k=3,m=3) | logistic_regression | 71 | 0.553 | 0.5135 | 0.5897 | 0.5473 | 0.4995 | 0.5921 | 0.3764 | 0.0815 | 0.1888 | 0.8 | 0.8393 | 0.733 | 3.6 | 74 |
| shifted_test | v2 (old features) | strict_window_fa<=1 | logistic_regression | 71 | 0.5315 | 0.4942 | 0.5681 | 0.5065 | 0.4598 | 0.5505 | 0.1207 | 0.0112 | 0.1622 | 0.2 | 0.7321 | 0.133 | 0.333 | 40 |
| shifted_test | v3 (new features) | raw (k=1) | logistic_regression | 71 | 0.4509 | 0.4256 | 0.4732 | 0.4509 | 0.4256 | 0.4732 | 0.3362 | 0.2669 | 0.4654 | 1 | 1 | 29.467 | 76.667 | 167 |
| shifted_test | v3 (new features) | episode_fa<=1 (k=3,m=3) | logistic_regression | 71 | 0.5551 | 0.5119 | 0.5938 | 0.5365 | 0.4804 | 0.5903 | 0.1724 | 0.2022 | 0.2234 | 0.4 | 0.7857 | 1.267 | 7.867 | 68 |
| shifted_test | v3 (new features) | strict_window_fa<=1 | logistic_regression | 71 | 0.5328 | 0.5 | 0.5721 | 0.4951 | 0.4612 | 0.5318 | 0.069 | 0.0534 | 0.1995 | 0.2 | 0.7143 | 0.6 | 1.667 | 41 |
| shifted_test | v2 (old features) | raw (k=1) | random_forest | 71 | 0.5242 | 0.4774 | 0.5721 | 0.5242 | 0.4774 | 0.5721 | 0.7011 | 0.2949 | 0.3431 | 1 | 0.9286 | 14.333 | 77.333 | 172 |
| shifted_test | v2 (old features) | episode_fa<=1 (k=3,m=3) | random_forest | 71 | 0.6218 | 0.5673 | 0.6722 | 0.6149 | 0.5406 | 0.6857 | 0.5287 | 0.264 | 0.4521 | 1 | 0.875 | 2.133 | 12.2 | 102 |
| shifted_test | v2 (old features) | strict_window_fa<=1 | random_forest | 71 | 0.6439 | 0.5842 | 0.7035 | 0.6392 | 0.5676 | 0.7119 | 0.4828 | 0.2444 | 0.3777 | 0.8 | 0.8393 | 0.467 | 1.4 | 71 |
| shifted_test | v3 (new features) | raw (k=1) | random_forest | 71 | 0.613 | 0.5584 | 0.6596 | 0.613 | 0.5584 | 0.6596 | 0.4224 | 0.2388 | 0.4309 | 1 | 0.9286 | 14.333 | 32.067 | 108 |
| shifted_test | v3 (new features) | episode_fa<=1 (k=3,m=3) | random_forest | 71 | 0.6249 | 0.567 | 0.6717 | 0.6082 | 0.5407 | 0.661 | 0.2816 | 0.2331 | 0.4707 | 0.8 | 0.8571 | 1.4 | 8.6 | 51 |
| shifted_test | v3 (new features) | strict_window_fa<=1 | random_forest | 71 | 0.6444 | 0.5837 | 0.6993 | 0.6265 | 0.5594 | 0.6838 | 0.227 | 0.2079 | 0.4973 | 0.8 | 0.875 | 0.2 | 0.6 | 11 |
| broad_basin | v2 (old features) | raw (k=1) | threshold_rule | 20 | 0.5628 | 0.4853 | 0.6365 | 0.5628 | 0.4853 | 0.6365 | 0.3592 | 0.4101 | 0 | 1 | 0.9 | 0 | 0 | 32 |
| broad_basin | v2 (old features) | episode_fa<=1 (k=3,m=3) | threshold_rule | 20 | 0.5628 | 0.4853 | 0.6365 | 0.5532 | 0.4432 | 0.6516 | 0.3592 | 0.4101 | 0 | 0.8889 | 0.75 | 0 | 0 | 32 |
| broad_basin | v2 (old features) | strict_window_fa<=1 | threshold_rule | 20 | 0.5628 | 0.4853 | 0.6365 | 0.5197 | 0.4124 | 0.6075 | 0.3592 | 0.4101 | 0 | 0.7778 | 0.7 | 0 | 0 | 32 |
| broad_basin | v3 (new features) | raw (k=1) | threshold_rule | 20 | 0.557 | 0.4748 | 0.6308 | 0.557 | 0.4748 | 0.6308 | 0.3592 | 0.3848 | 0 | 1 | 0.9 | 0 | 0 | 32 |
| broad_basin | v3 (new features) | episode_fa<=1 (k=3,m=3) | threshold_rule | 20 | 0.557 | 0.4748 | 0.6308 | 0.5478 | 0.4402 | 0.6497 | 0.3592 | 0.3848 | 0 | 0.8889 | 0.7 | 0 | 0 | 32 |
| broad_basin | v3 (new features) | strict_window_fa<=1 | threshold_rule | 20 | 0.557 | 0.4748 | 0.6308 | 0.5158 | 0.4069 | 0.6063 | 0.3592 | 0.3848 | 0 | 0.7778 | 0.65 | 0 | 0 | 32 |
| broad_basin | v2 (old features) | raw (k=1) | logistic_regression | 20 | 0.5021 | 0.4044 | 0.5731 | 0.5021 | 0.4044 | 0.5731 | 0.1939 | 0.5349 | 0 | 0.8889 | 0.95 | 0 | 0 | 19 |
| broad_basin | v2 (old features) | episode_fa<=1 (k=3,m=3) | logistic_regression | 20 | 0.3948 | 0.2941 | 0.4857 | 0.3721 | 0.2666 | 0.4663 | 0.0556 | 0.37 | 0 | 0.2222 | 0.4 | 0 | 0 | 1 |
| broad_basin | v2 (old features) | strict_window_fa<=1 | logistic_regression | 20 | 0.2847 | 0.1998 | 0.3572 | 0.2621 | 0.188 | 0.3252 | 0.0034 | 0.1947 | 0 | 0 | 0.2 | 0 | 0 | 0 |
| broad_basin | v3 (new features) | raw (k=1) | logistic_regression | 20 | 0.5075 | 0.4028 | 0.5908 | 0.5075 | 0.4028 | 0.5908 | 0.1703 | 0.6434 | 0 | 0.7778 | 0.9 | 0 | 0 | 9 |
| broad_basin | v3 (new features) | episode_fa<=1 (k=3,m=3) | logistic_regression | 20 | 0.4759 | 0.3742 | 0.5674 | 0.4671 | 0.3676 | 0.5569 | 0.1113 | 0.5215 | 0 | 0.2222 | 0.6 | 0 | 0 | 0 |
| broad_basin | v3 (new features) | strict_window_fa<=1 | logistic_regression | 20 | 0.3155 | 0.2385 | 0.3841 | 0.2706 | 0.2046 | 0.3389 | 0.0489 | 0.2065 | 0 | 0.2222 | 0.45 | 0 | 0 | 0 |
| broad_basin | v2 (old features) | raw (k=1) | random_forest | 20 | 0.6188 | 0.4973 | 0.7079 | 0.6188 | 0.4973 | 0.7079 | 0.5565 | 0.4666 | 0 | 1 | 1 | 0 | 0 | 1 |
| broad_basin | v2 (old features) | episode_fa<=1 (k=3,m=3) | random_forest | 20 | 0.5684 | 0.4436 | 0.6589 | 0.5673 | 0.4443 | 0.6637 | 0.398 | 0.3982 | 0 | 0.7778 | 0.65 | 0 | 0 | 4 |
| broad_basin | v2 (old features) | strict_window_fa<=1 | random_forest | 20 | 0.5462 | 0.4187 | 0.6405 | 0.53 | 0.4023 | 0.6208 | 0.3508 | 0.3893 | 0 | 0.7778 | 0.65 | 0 | 0 | 0 |
| broad_basin | v3 (new features) | raw (k=1) | random_forest | 20 | 0.5888 | 0.5046 | 0.6678 | 0.5888 | 0.5046 | 0.6678 | 0.3676 | 0.5141 | 0 | 1 | 0.95 | 0 | 0 | 3 |
| broad_basin | v3 (new features) | episode_fa<=1 (k=3,m=3) | random_forest | 20 | 0.5827 | 0.4974 | 0.6602 | 0.5723 | 0.4715 | 0.6625 | 0.3541 | 0.5126 | 0 | 0.8889 | 0.9 | 0 | 0 | 5 |
| broad_basin | v3 (new features) | strict_window_fa<=1 | random_forest | 20 | 0.5263 | 0.4367 | 0.6062 | 0.4913 | 0.3789 | 0.5796 | 0.2648 | 0.4368 | 0 | 0.6667 | 0.8 | 0 | 0 | 7 |
