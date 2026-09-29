# Model 2 – Random Forest

Random Forest is the second classifier. It provides a nonlinear ensemble approach capable of modelling interactions between customer/account variables.**

| Hyperparameter | Value |
|---|---|
| n_estimators | 300 |
| max_depth | 12 |
| min_samples_split | 5 |
| min_samples_leaf | 2 |
| class_weight | balanced |
| random_state | 42 |
| n_jobs | -1 |


The same train/test split and preprocessing approach is used so that the comparison of the models can be more fairly.

**Implementation:** Notebooks/04_Model2_Random_Forest.ipynb.
