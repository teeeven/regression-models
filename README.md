# Regression Models

![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)
![scikit-learn](https://img.shields.io/badge/scikit--learn-compatible-orange.svg)
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)

A supervised learning study exploring two foundational regression techniques applied to real-world datasets. Each project follows a consistent workflow: exploratory data analysis, feature engineering, model training, and evaluation.

These notebooks represent the ML foundations that inform the production pipelines in my other work.

---

## Projects

### [Linear Regression](./linear-regression/) — MLB Runs Created
Predicts a player's offensive contribution (Runs Created) from MLB batting statistics.

- **Dataset:** MLB batting records (`Batting.csv`)
- **Technique:** Linear Regression with Ridge regularization
- **Key concepts:** EDA, numerical & categorical feature engineering, regularization to handle correlated features

> Ridge regularization adds a penalty equal to the square of the coefficients — useful for reducing the impact of noisy or correlated features while keeping all variables in the model.

---

### [Logistic Regression](./logistic-regression/) — Telco Customer Churn
Predicts whether a telecom customer will churn using binary classification.

- **Dataset:** Telco customer data (`telco-churn.csv`)
- **Technique:** Logistic Regression (binary & multi-class)
- **Key concepts:** Sigmoid function, probability thresholds, classification metrics

> The classification threshold — the probability cutoff that determines a positive prediction — is not purely a technical decision. It is determined collaboratively with stakeholders based on the cost of false positives vs. false negatives.

---

## Structure

```
regression-models/
├── linear-regression/
│   ├── workflow.ipynb     — Full EDA, engineering, and modeling notebook
│   └── Batting.csv        — MLB batting statistics dataset
└── logistic-regression/
    ├── workflow.ipynb     — Full EDA, engineering, and modeling notebook
    └── telco-churn.csv    — Telecom customer churn dataset
```

---

## Design Philosophy

These notebooks follow the same principles I apply in production:

- **Atomicity** — each transformation step is isolated and testable
- **Observability** — outputs and intermediate results are visible throughout
- **Composability** — feature engineering patterns are reusable across projects

---

## Contact

- **LinkedIn:** [steven-orizaga](https://www.linkedin.com/in/steven-orizaga/)
- **GitHub:** [teeeven](https://github.com/teeeven)
- **Email:** stevenorizaga@gmail.com

---

MIT License
