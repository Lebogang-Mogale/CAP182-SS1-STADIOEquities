# Model 2 Performance – Random Forest

Model 2 uses Random Forest with n_estimators=300, max_depth=12, min_samples_split=5, min_samples_leaf=2, class_weight=balanced, random_state=42 and n_jobs=-1.

## Published benchmark context
Mettle et al. (2026), using the IBM Telco Customer Churn dataset, reported Accuracy 84.73%, Precision 85.20%, Recall 84.07%, F1-score 84.62% and ROC-AUC 93.86%.

These are published benchmark figures, not independently executed results from this repository. Run the supplied evaluation code on the exact Part A dataset before final submission and replace the benchmark figures with your actual outputs.

## Reproduction
**Run:** Notebooks/Model2Perfomance.ipynb`.
