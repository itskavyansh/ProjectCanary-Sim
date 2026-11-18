# Radial Convergence Feature Distributions by Shape (SYNTHETIC / SIMULATION)

> **SYNTHETIC / SIMULATION** — Model-mismatch stress test on synthetic mathematical surfaces; NOT field data and NOT validated on real data.

| shape | subset | windows | residual_m p10 / **p50** / p90 (mean) | weighted_cos p10 / **p50** / p90 (mean) | pairwise_cos p50 |
|---|---|---|---|---|---|
| gaussian_control | active_windows_all_snr | 3824 | 1.57 / **6.88** / 17.28 (8.56) | -0.796 / **0.722** / 0.994 (0.378) | -0.065 |
| gaussian_control | active_windows_snr_gt_2 | 1819 | 1.07 / **3.23** / 11.55 (5.27) | -0.427 / **0.952** / 0.998 (0.623) | -0.065 |
| gaussian_control | active_windows_snr_gt_5 | 1214 | 0.97 / **2.90** / 10.45 (4.57) | -0.437 / **0.965** / 0.998 (0.666) | -0.077 |
| trough_panel | active_windows_all_snr | 3824 | 1.19 / **8.56** / 18.60 (9.63) | -0.838 / **0.450** / 0.997 (0.270) | -0.100 |
| trough_panel | active_windows_snr_gt_2 | 1819 | 0.75 / **4.12** / 16.18 (6.18) | -0.545 / **0.920** / 0.999 (0.493) | -0.107 |
| trough_panel | active_windows_snr_gt_5 | 1214 | 0.67 / **3.13** / 16.03 (5.72) | -0.600 / **0.959** / 0.999 (0.469) | -0.135 |
| asymmetric | active_windows_all_snr | 3824 | 1.68 / **6.14** / 16.59 (7.96) | -0.673 / **0.849** / 0.994 (0.466) | -0.043 |
| asymmetric | active_windows_snr_gt_2 | 1819 | 1.09 / **2.79** / 9.45 (4.10) | 0.025 / **0.980** / 0.997 (0.779) | -0.031 |
| asymmetric | active_windows_snr_gt_5 | 1214 | 0.99 / **2.30** / 6.27 (3.26) | 0.607 / **0.990** / 0.999 (0.864) | -0.078 |
| two_basin | active_windows_all_snr | 3824 | 1.33 / **7.42** / 17.85 (8.94) | -0.883 / **0.690** / 0.992 (0.322) | -0.058 |
| two_basin | active_windows_snr_gt_2 | 1819 | 1.01 / **3.83** / 13.85 (5.86) | -0.908 / **0.944** / 0.996 (0.538) | -0.058 |
| two_basin | active_windows_snr_gt_5 | 1214 | 0.88 / **3.52** / 12.45 (5.16) | -0.951 / **0.956** / 0.997 (0.592) | -0.049 |
| planar_slope | active_windows_all_snr | 3824 | 5.86 / **10.43** / 42.11 (16.38) | -0.983 / **0.226** / 0.996 (0.116) | 0.888 |
| planar_slope | active_windows_snr_gt_2 | 1819 | 6.79 / **9.68** / 50.00 (16.89) | -0.989 / **0.910** / 0.998 (0.321) | 0.993 |
| planar_slope | active_windows_snr_gt_5 | 1214 | 7.01 / **9.65** / 47.61 (16.11) | -0.980 / **0.960** / 0.998 (0.383) | 0.997 |
