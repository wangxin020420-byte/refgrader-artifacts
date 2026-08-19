# Mohler ACL 2011 Statistical Analysis

Deployment class: `experimental_external_validation`

## Paired question-cluster bootstrap

| Comparison | Metric | Gain | 95% CI | P(gain > 0) | Significant |
|---|---:|---:|---:|---:|---:|
| avg_to_3wd_core | MAE | 0.009151 | [0.003546, 0.014902] | 0.9995 | True |
| avg_to_3wd_core | RMSE | 0.006366 | [0.002606, 0.010559] | 0.9997 | True |
| 3wd_core_to_3wd | MAE | 0.151034 | [0.128005, 0.174486] | 1.0000 | True |
| 3wd_core_to_3wd | RMSE | 0.154402 | [0.134701, 0.173658] | 1.0000 | True |
| avg_to_3wd | MAE | 0.160185 | [0.135815, 0.184506] | 1.0000 | True |
| avg_to_3wd | RMSE | 0.160767 | [0.140474, 0.180823] | 1.0000 | True |

Positive gain means the target score has lower error. Questions are resampled as clusters.

## Per-question QWK aggregate

| Method | Common-question weighted QWK | Method-defined weighted QWK | Defined questions | Undefined questions |
|---|---:|---:|---:|---:|
| single | 0.540814 | 0.540814 | 80 | 1 |
| avg | 0.574178 | 0.567357 | 81 | 0 |
| selected | 0.574178 | 0.567357 | 81 | 0 |
| 3wd_core | 0.577950 | 0.571085 | 81 | 0 |
| 3wd | 0.629292 | 0.629292 | 80 | 1 |

Scores are clipped to 0-5, rounded to the nearest 0.5, encoded as 0-10, and QWK is computed independently per question.

## Comparison boundary

Direct comparison with the ACL 2011 reported numbers is not authorized.
- The distributed archive contains 81 included questions while the paper reports 80.
- The current RefGrader run is zero-shot with a private-data A3WA configuration, while the paper trains supervised regressors inside its folds.
- The active A3WA configuration was used under an experimental deployment override.
