## Module 02 Mini-Project — Classical ML Pipeline

### Project Goal

Build a **full classical ML pipeline** with:

- Clean, honest evaluation
- Thoughtful feature engineering
- Strong baselines + several models
- Final model selection with justification
- Reproducible code and a short written report

Recommended problem: **Customer Churn Prediction** (or **Loan Default Risk**).

### Repository Layout

```text
modules/module-02-classical-ml/mini-project/
├─ README.md
├─ data/
│  ├─ raw/                 # original dataset (optionally gitignored)
│  └─ processed/           # cleaned parquet/csv
├─ notebooks/
│  ├─ 00-data-audit.ipynb
│  ├─ 01-baseline.ipynb
│  ├─ 02-models.ipynb
│  └─ 03-thresholding.ipynb
├─ src/
│  ├─ __init__.py
│  ├─ config.py
│  ├─ data.py              # load/clean/split
│  ├─ features.py          # feature engineering
│  ├─ train.py             # training entry-point
│  ├─ evaluate.py          # metrics + plots
│  └─ infer.py             # inference on new samples
├─ reports/
│  └─ report.md
└─ outputs/
   ├─ models/              # saved models
   └─ figures/             # plots
```

### Suggested Workflow

1. **Data audit** (`00-data-audit.ipynb`)
   - Inspect schema, missingness, leakage risk, imbalance, feature types.
2. **Baselines first** (`01-baseline.ipynb`)
   - Dummy classifier (most frequent) + simple logistic regression.
3. **Feature engineering loop** (`02-models.ipynb`)
   - Encoding, scaling, ratios/aggregates where appropriate.
4. **Model training + selection** (`02-models.ipynb`)
   - Logistic Regression, Random Forest, Gradient Boosting.
5. **Thresholding + business trade-offs** (`03-thresholding.ipynb`)
   - Precision/recall, confusion matrix, threshold sweep.
6. **Report** (`reports/report.md`)
   - What you tried, what worked, why the final choice, failure modes, next steps.

This mini-project is meant to be **portfolio-grade** and suitable for a YouTube walkthrough.

