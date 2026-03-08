# Regression Models

![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)
![scikit-learn](https://img.shields.io/badge/scikit--learn-compatible-orange.svg)
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)

A supervised learning study working through two foundational regression techniques using real-world datasets. These notebooks were built as part of my self-study through *Machine Learning Bookcamp* by Alexey Grigorev — working through the material hands-on, applying it to datasets I found meaningful, and learning by doing.

---

## From Study to Production

The logistic regression workflow in this repository directly informed a production machine learning system I built for the admissions office at my institution.

That project — built on the same foundations explored here — used institutional applicant data to predict student deposit likelihood, helping the admissions team prioritize outreach and allocate resources more effectively. It includes a full evaluation pipeline (confusion matrix, precision/recall, ROC-AUC, threshold tuning), model serialization, and a Flask API for serving predictions.

**These notebooks are where I learned it. That project is where I applied it.**

I cannot share institutional data or the production codebase publicly, but the connection is real and I'm happy to walk through both in conversation.

---

## Projects

### [Linear Regression](./linear-regression/) — MLB Runs Created

Predicts a player's offensive contribution (Runs Created) from MLB batting statistics.

- **Dataset:** MLB batting records (`Batting.csv`)
- **Technique:** Linear Regression with Ridge regularization
- **Key concepts:** EDA, feature engineering from baseball domain knowledge, log transformation for skewed targets, regularization to reduce the impact of correlated features

This was a useful domain to learn in because the features have real meaning — you have to think about what you're engineering and why, not just throw columns at a model.

---

### [Logistic Regression](./logistic-regression/) — Telco Customer Churn

Predicts whether a telecom customer will churn using binary classification.

- **Dataset:** Telco customer data (`telco-churn.csv`) — the same dataset used in *ML Bookcamp*
- **Technique:** Logistic Regression (binary classification)
- **Key concepts:** Class imbalance, sigmoid function, probability thresholds, feature importance via risk ratio and mutual information, model interpretability through coefficient inspection

The churn problem is a natural fit for admissions work — both are fundamentally about predicting whether someone stays or leaves, and the same logic applies. Working through this dataset made the transition to institutional data feel natural.

---

## What I Learned Along the Way

These notebooks reflect a real learning process — not a finished product. A few honest notes:

- **Evaluation depth grew over time.** Early on I leaned on accuracy and RMSE. After applying these techniques to production data, I understood why metrics like ROC-AUC, precision/recall, and confusion matrices matter — especially when classes are imbalanced.
- **Threshold selection is a business decision, not just a technical one.** The cost of a false positive (unnecessary outreach) vs. a false negative (missing a likely deposit) is something stakeholders have to weigh in on. That nuance isn't obvious from a textbook.
- **Feature engineering is where domain knowledge lives.** The most useful features in both projects came from understanding the data, not from running algorithms.

---

## Design Philosophy

These notebooks follow the same principles I apply across all my work:

- **Atomicity** — each step does one thing and documents why
- **Observability** — outputs and intermediate results are visible throughout
- **Composability** — patterns learned here carry forward into production work

---

## Structure

```
regression-models/
├── linear-regression/
│   ├── workflow.ipynb     — EDA, feature engineering, Ridge regression, evaluation
│   └── Batting.csv        — MLB batting statistics dataset
└── logistic-regression/
    ├── workflow.ipynb     — EDA, feature analysis, logistic regression, evaluation
    └── telco-churn.csv    — Telco customer churn dataset
```

---

## Contact

- **LinkedIn:** [steven-orizaga](https://www.linkedin.com/in/steven-orizaga/)
- **GitHub:** [teeeven](https://github.com/teeeven)
- **Email:** stevenorizaga@gmail.com

---

MIT License
