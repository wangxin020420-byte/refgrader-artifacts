# Repeated Public Benchmark Summary

Runs: 3
Samples per run: 331
Deployment class: experimental

## Global metrics

| Score | MAE mean | MAE SD | RMSE mean | SER mean | Bias mean |
|---|---:|---:|---:|---:|---:|
| single | 1.046495 | 0.005808 | 1.566369 | 17.22% | -0.971974 |
| avg | 1.048238 | 0.014049 | 1.523849 | 17.72% | -0.993656 |
| selected | 1.048238 | 0.014049 | 1.523849 | 17.72% | -0.993656 |
| 3WD-Core | 1.009970 | 0.012562 | 1.493251 | 17.12% | -0.948943 |
| 3WD | 0.832830 | 0.007769 | 1.333196 | 13.09% | -0.700705 |

## Mechanism ablation

| Component | Mean gain | SD | 95% cluster CI | P(gain > 0) |
|---|---:|---:|---:|---:|
| three_way_core | 0.038268 | 0.011338 | [0.023292, 0.055455] | 1.0000 |
| validation_residual | 0.177140 | 0.017529 | [0.138586, 0.215400] | 1.0000 |
| full_three_way | 0.215408 | 0.013145 | [0.170974, 0.260910] | 1.0000 |

## Routing and stability

- BND mean rate: 51.96%
- POS mean rate: 48.04%
- Risk recall: 70.52%
- Safe POS rate: 89.11%
- Final score exact across runs: 49.24%
- Route exact across runs: 74.02%
- Boundary action exact across runs: 64.05%
