# Zeke Zhang

**Computer Science & Mathematics at the University of Wisconsin–Madison**

I build trading-system prototypes, machine learning systems, and quantitative research tools with an emphasis on reproducible evaluation, clear system boundaries, and measured results.

## Selected projects

### [Limit Order Book Matching Engine](https://github.com/Evihut/lob-matching-engine)

An independently developed C++20 price–time priority matching core with a flat price ladder, bitmap lookup, pooled FIFO queues, and an open-addressing order-ID map. Differential tests compare 1.6 million messages with a separate map reference. A single-thread Apple M4 synthetic replay reports **91.3M messages/s** versus **16.1M** for the reference; parsing and network I/O are excluded, so this is not production exchange throughput.

[Reviewed version](https://github.com/Evihut/lob-matching-engine/tree/fix/review-findings) · [Passing CI](https://github.com/Evihut/lob-matching-engine/actions/runs/36656935148)

`C++20` · `Cache-aware Data Structures` · `Differential Testing` · `ASan / UBSan`

### [A-Share Factor Research Pipeline](https://github.com/Evihut/a-share-factor-pipeline)

An independently developed, reproducible ten-factor study using the CSI 300 point-in-time universe. In-sample selection (2018–2021) is separated from evaluation (2022–2025 H1), with next-open execution, size neutralization, drift-adjusted turnover, and a survivorship-bias experiment. The composite records OOS **RankIC 0.0324** and annualized **ICIR 1.44**. Locked dependencies, data checksums, and a frozen 100-stock regression sample support reproducibility. This is historical A-share research, not a live trading or U.S.-market performance claim.

[Reviewed research report](https://github.com/Evihut/a-share-factor-pipeline/blob/fix/review-findings/reports/REPORT.md) · [Passing CI](https://github.com/Evihut/a-share-factor-pipeline/actions/runs/36656940586)

`Python` · `pandas / NumPy` · `Point-in-time Universe` · `Regression Testing`

### [MiniMind Systems](https://github.com/Evihut/minimind-systems)

Inference engineering extensions for MiniMind, including static KV caching, dynamic request batching, and observable FastAPI serving. Reproducible CPU microbenchmarks compare cache and batching configurations while documenting their experimental limits.

`PyTorch` · `FastAPI` · `Static KV Cache` · `Dynamic Batching` · `Prometheus`

### [Explainable ESG Risk & Reporting](https://github.com/Evihut/esg-risk-reporting)

A leakage-aware modeling benchmark, SHAP evidence bundle, and validated reporting API. A fixed-parameter evaluation records CatBoost OOF RMSE **4.870** against a training-fold mean baseline of **6.890** across 430 eligible companies.

`CatBoost` · `SHAP` · `scikit-learn` · `FastAPI`

**2025 Zhixiang Cup · Grand Prize**<br>
<sub>The award applies to the original competition case; the repository documents the subsequent engineering release.</sub>

## Interests

Machine learning systems · Applied mathematics · Interpretable modeling · Quantitative research

[Personal website →](https://evihut.github.io/) · [View all repositories →](https://github.com/Evihut?tab=repositories)
