**Table R.1.** Experiment results on OPT-13B.
| Dataset | SST-2 |           |  RTE |           | SQuAD |           |
|---------|:-----:|-----------|:----:|-----------|:-----:|-----------|
|         | Acc.  | GPU hours | Acc. | GPU hours | Acc.  | GPU hours |
| MeZO    |  91.4 | 100%      | 66.1 | 100%      |  84.7 | 100%      |
| HiZOO   |  91.9 | 86%        | 71.3| 82%        |  82.9| 91%       |
| DiZO    |  **92.4** | **69%**        | **72.6** | **76%**        |  **85.2** | **73%**     |

**Table R.2.** Finetuning Llama2-7B on Alpaca GPT-4 dataset and then evaluation. 
|           | MT-Bench |  MMLU (5 shot) | GPU hours |
|-----------|:--------:|:-----:|:---------:|
| Zero-shot |   3.93   | 45.87 |     -     |
| MeZO      |   4.59   | 45.22 |    100%   |
| HiZOO     |   4.64   | 45.42 |    92%    |
| DiZOO     |   **4.79**   | **45.91** |    **78%**    |

**Table R.3.** Finetuning Llama3-8B on Alpaca GPT-4 dataset and then evaluation.  
|           | MT-Bench |  MMLU(5 shot) | GPU hours |
|-----------|:--------:|:-----:|:---------:|
| Zero-shot |   5.46   | 65.20 |     -     |
| MeZO      |   5.89   | 65.08 |    100%   |
| HiZOO     |   5.93   | 65.20 |    95%    |
| DiZOO     |   **6.15**   | **65.42** |    **83%**    |


**Table R.4.** Experiment results on fine-tuning OPT-2.7B with and without layer-wise divergence.
|          | SST2       | RTE        |
|----------|------------|------------|
| W/ Norm (W/O divergence)  | 92.5 (2.3) | 76.8 (7.8) |
| Vallina (W/ divergence)| 94.2 (1.2) | 81.2 (3.7) |

**Table R.5.** Results of Finetuning OPT-2.7B on SST-2 for 1K iteraions. 
|      | Optimizer | Acc. | Train FLOPs. | 
|------|:---------:|:----:|:-----------:|
| MeZO |    SGD    | 87.0 |     100%    | 
| MeZo |    Adam   | 88.3 |    431%    | 
| DiZO |    SGD    | 91.6 |     122%    |
