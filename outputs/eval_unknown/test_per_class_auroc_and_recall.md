# Per-Class vs Normal Window AUROC and Flag Recall on `test` (`SYNTHETIC / SIMULATION`)

> **Note:** Evaluated on trainable windows of the held-out `test` split (`2,850` normal windows vs each known anomaly class). Unsupervised detectors never see class labels and output only `anomaly_score` and `unknown_anomaly`.

| Detector | Class vs `normal` | Class Windows | Normal Windows | Window AUROC [95% CI] | Raw Window Flag Recall [95% CI] | Persisted `(k=3,m=3)` Window Flag Recall [95% CI] |
| :--- | :--- | ---: | ---: | :---: | :---: | :---: |
| `isolation_forest` | `gradual` | 1333 | 7154 | **0.594 [0.536, 0.662]** | 0.206 [0.135, 0.310] | 0.145 [0.064, 0.271] |
| `isolation_forest` | `rapid` | 1167 | 7154 | **0.617 [0.545, 0.693]** | 0.211 [0.145, 0.283] | 0.156 [0.078, 0.233] |
| `isolation_forest` | `abnormal_vibration` | 502 | 7154 | **1.000 [1.000, 1.000]** | 1.000 [1.000, 1.000] | 0.966 [0.954, 0.978] |
| `isolation_forest` | `sensor_fault` | 555 | 7154 | **0.664 [0.595, 0.733]** | 0.261 [0.191, 0.351] | 0.182 [0.095, 0.279] |
| `isolation_forest` | `comm_fault` | 530 | 7154 | **0.909 [0.862, 0.946]** | 0.719 [0.597, 0.827] | 0.713 [0.567, 0.841] |
| `isolation_forest` | `all_known_anomalies` | 4087 | 7154 | **0.701 [0.655, 0.740]** | 0.379 [0.318, 0.438] | 0.328 [0.264, 0.391] |
| `robust_mahalanobis` | `gradual` | 1333 | 7154 | **0.621 [0.549, 0.698]** | 0.260 [0.154, 0.393] | 0.185 [0.081, 0.317] |
| `robust_mahalanobis` | `rapid` | 1167 | 7154 | **0.686 [0.571, 0.801]** | 0.397 [0.222, 0.570] | 0.347 [0.163, 0.530] |
| `robust_mahalanobis` | `abnormal_vibration` | 502 | 7154 | **0.997 [0.992, 1.000]** | 1.000 [1.000, 1.000] | 0.962 [0.951, 0.972] |
| `robust_mahalanobis` | `sensor_fault` | 555 | 7154 | **0.752 [0.666, 0.852]** | 0.510 [0.347, 0.674] | 0.454 [0.271, 0.628] |
| `robust_mahalanobis` | `comm_fault` | 530 | 7154 | **0.983 [0.968, 0.993]** | 0.959 [0.920, 0.987] | 0.921 [0.885, 0.947] |
| `robust_mahalanobis` | `all_known_anomalies` | 4087 | 7154 | **0.750 [0.695, 0.798]** | 0.514 [0.422, 0.596] | 0.459 [0.365, 0.541] |
