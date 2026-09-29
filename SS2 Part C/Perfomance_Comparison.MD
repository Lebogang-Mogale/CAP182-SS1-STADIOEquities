 # Comparison – Model 1 and Model 2

| Metric | Logistic Regression | Random Forest |
|---|---:|---:|
| Accuracy | 83.26% | 84.73% |
| Precision | 82.59% | 85.20% |
| Recall | 84.29% | 84.07% |
| F1-score | 83.43% | 84.62% |
| ROC-AUC | 91.96% | 93.86% |

These are published benchmark results from Mettle et al. (2026), not independently executed results from the student's exact pipeline. In that published benchmark, Logistic Regression reported higher recall, while Random Forest reported higher accuracy, precision, F1-score and ROC-AUC.

For STADIOEquities, the eventual model should be evaluated using recall, precision, F1, ROC-AUC, threshold analysis and temporal validation using information available before the prediction point.

**Run:** notebooks/Performance_Comparison.ipynb` to generate results .

