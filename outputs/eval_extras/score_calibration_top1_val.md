# Model Score Reliability & Calibration on VAL Only (SYNTHETIC / SIMULATION)

> **Important Documentation on Model Scores:**
> 1. Output scores are raw, uncalibrated classifier outputs designated strictly as **`model_score`** (never 'probability' or 'confidence').
> 2. Random Forest and Logistic Regression probabilities are **NOT** calibrated Bayesian probabilities.
> 3. Tree ensembles typically exhibit under-confidence in extreme regimes and push scores toward intermediate values due to finite-leaf smoothing.
> 4. No 'uncertain' classification outcome is produced; each window receives raw model scores across the 6 condition classes.

| Model | Bin Range (model_score) | Mean model_score | Empirical Accuracy | Window Count |
|---|---|---|---|---|
| random_forest | [0.0, 0.1) | N/A | N/A | 0 |
| random_forest | [0.1, 0.2) | N/A | N/A | 0 |
| random_forest | [0.2, 0.3) | 0.2879 | 0.3878 | 49 |
| random_forest | [0.3, 0.4) | 0.3549 | 0.6206 | 4433 |
| random_forest | [0.4, 0.5) | 0.4438 | 0.7092 | 3704 |
| random_forest | [0.5, 0.6) | 0.5398 | 0.7688 | 995 |
| random_forest | [0.6, 0.7) | 0.6464 | 0.7576 | 396 |
| random_forest | [0.7, 0.8) | 0.7508 | 0.886 | 228 |
| random_forest | [0.8, 0.9) | 0.8549 | 0.9563 | 252 |
| random_forest | [0.9, 1.0) | 0.9756 | 1.0 | 1187 |
| logistic_regression | [0.0, 0.1) | N/A | N/A | 0 |
| logistic_regression | [0.1, 0.2) | N/A | N/A | 0 |
| logistic_regression | [0.2, 0.3) | 0.284 | 0.2672 | 348 |
| logistic_regression | [0.3, 0.4) | 0.3563 | 0.3835 | 3364 |
| logistic_regression | [0.4, 0.5) | 0.446 | 0.4713 | 3246 |
| logistic_regression | [0.5, 0.6) | 0.5432 | 0.5718 | 1796 |
| logistic_regression | [0.6, 0.7) | 0.6418 | 0.6645 | 918 |
| logistic_regression | [0.7, 0.8) | 0.7392 | 0.737 | 308 |
| logistic_regression | [0.8, 0.9) | 0.8439 | 0.6842 | 152 |
| logistic_regression | [0.9, 1.0) | 0.9943 | 0.9532 | 1112 |
