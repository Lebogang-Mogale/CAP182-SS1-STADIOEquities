# Model 1 – Logistic Regression

Logistic Regression is the baseline binary classifier. It provides an interpretable linear benchmark and probability estimates.

| Hyperparameter | Value |
|---|---|
| C | 1.0 |
| solver | liblinear |
| max_iter | 1000 |
| class_weight | balanced |
| random_state | 42 |

The model is combined with the preprocessing ColumnTransformer in a pipeline.

**Implementation:** Notebooks/03_Model1_Logistic_Regression.ipynb.
