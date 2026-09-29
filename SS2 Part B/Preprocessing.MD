# Prepare the public Bank Customer Churn Modelling dataset for classification as a reproducible proxy for the STADIOEquities dormancy problem.

**Steps**
1. Inspect data types, missing values and target distribution.
2. Remove RowNumber, CustomerId and Surname.
3. Separate predictors from the Exited target.
4. Use a stratified 80:20 train/test split with random_state=42.
5. Impute numerical values with the training-set median.
6. Impute categorical values with the training-set most frequent category.
7. One-hot encode categorical variables with handle_unknown="ignore".
8. Standardise numerical variables.
9. Use class_weight="balanced" in both classifiers because the target is imbalanced.
10. Fit preprocessing only on training data through a scikit-learn Pipeline/ColumnTransformer to prevent leakage.

**Implementation:** Notebooks/01_Preprocessing.ipynb.
