# Unsupervised Unknown Anomaly Detector — Threshold Selection on `val` Normal Runs (`SYNTHETIC / SIMULATION`)

- **Fit Data:** Strictly `train` windows with `label == 'normal'` (`21,305` windows across all `train` runs, including normal lead-in and benign confounder windows; `81` model features from `feature_columns(df)`; zero `diag_` columns).
- **Threshold Tuning Data:** Strictly `val` normal-only runs (`20` runs, `1,900` windows), evaluated under `(k=3, m=3)` episode persistence with target `<= 1.0` false-alarm episode per normal run.
- **Score Naming:** Output score is `anomaly_score` (never a probability or confidence); flag is `unknown_anomaly`.

| Detector | Fitted `train` Normal Windows | `val` Normal Runs (`windows`) | Persistence `(k, m)` | Target FA / Normal Run | Chosen `anomaly_score` Threshold | `val` Normal Window Quantile | Achieved `val` FA Episodes / Run | Achieved `val` FA Windows / Run |
| :--- | ---: | ---: | :---: | ---: | ---: | ---: | ---: | ---: |
| `isolation_forest` | 21305 | 20 (1900) | `(3, 3)` | <= 1.00 | **0.467299** | 0.8700 | **1.000** | 4.40 |
| `robust_mahalanobis` | 21305 | 20 (1900) | `(3, 3)` | <= 1.00 | **9.759898** | 0.8250 | **1.000** | 10.70 |
