# Network Attack Detection — Master's Thesis AITU 2026

**Title:** Development of a System for Analyzing Data on Network Attacks to Create Effective Strategies to Protect Against New Threats

**Author:** Muratbekova Milana Dulatovna
**Supervisor:** Rostislav Valerievich Lisnevsky
**Program:** 7M06103 Applied Data Analytics
**Institution:** School of Artificial Intelligence and Data Science, Astana IT University LLP

## Compiling in Overleaf

1. Upload this ZIP via **New Project → Upload Project**
2. Open **Menu** (top-left)
3. Under **Compiler** select **pdfLaTeX**
4. Click **Recompile**

## Project Structure

- `main.tex` — entry point (pdfLaTeX, English primary, T2A enabled for any Cyrillic in figures)
- `frontmatter/` — title page, abstract, list of abbreviations
- `chapters/` — Chapters 1–5 plus the supplementary appendix
- `figures/` — 10 figures (PNG)
- `logos/` — AITU logo
- `references.bib` — bibliography (21 sources)

## Chapter Outline

- **Chapter 1 — Introduction:** background, problem statement, hypothesis, objectives, contributions
- **Chapter 2 — Literature Review:** benchmark datasets, classical ML, anomaly detection, deep learning, hybrid systems
- **Chapter 3 — Methodology:** CICIDS2017 dataset, preprocessing pipeline (SMOTE + VIF + correlation filtering), six ML models with full mathematical formulation, evaluation protocol
- **Chapter 4 — Results and Discussion:** comparative model performance, per-class metrics, ROC analysis, SHAP/LIME interpretability, proposed SIEM architecture
- **Chapter 5 — Conclusion:** principal findings, scientific contributions, practical recommendations, future research directions
- **Appendix:** hyperparameter search space, optimal hyperparameters, Python environment, reproducibility notes, extended per-class report

## Key Result

LightGBM achieved Accuracy = 0.98, F1-score = 0.97, ROC-AUC = 0.99 on the CICIDS2017 benchmark, training in 89 seconds — outperforming Logistic Regression, KNN, Random Forest, XGBoost, and MLP across all metrics. SHAP analysis identified Flow Duration, InPktRate, and OutByteRate as the most discriminative features.
