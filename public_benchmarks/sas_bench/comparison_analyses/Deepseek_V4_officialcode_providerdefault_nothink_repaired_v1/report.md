# SAS-Bench Official-Pipeline Cross-Model Replication

- Run tag: `Deepseek_V4_officialcode_providerdefault_nothink_repaired_v1`
- Samples: 4109
- Valid predictions: 4109/4109
- Silent fallback: 0

## Macro Results

| Metric | Current run | Paper DeepSeek-V3 | Delta |
|---|---:|---:|---:|
| QWK | 69.83% | Not uniformly reported | - |
| CCS | 75.96% | 74.11% | +1.85 pp |
| ECS | 55.62% | 54.00% | +1.62 pp |

## Interpretation

This run validates the official SAS-Bench pipeline using the current DeepSeek endpoint.
It is a cross-model replication rather than an exact reproduction of the paper's DeepSeek-V3 experiment.
The result does not yet evaluate RefGrader or its three-way decision mechanism.
