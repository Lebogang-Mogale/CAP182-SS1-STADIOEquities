# CAP182 SS3 Part B — STADIOEquities Dormancy Prediction

## Files
- `SS3_PartB.ipynb`: end-to-end notebook for loading, point-in-time feature engineering, preprocessing, model training, validation and visualisation.
- `README_SS3_PartB.md`: setup and reproducibility instructions.

## Data setup
1. Extract `mogalelebogang_client_data.zip`.
2. Ensure the folder `stadioequities` containing the ten CSV files is beside the notebook, or set `DATA_DIR` in the first code section.
3. Open `SS3_PartB.ipynb` in Jupyter Notebook/JupyterLab and run all cells from top to bottom.

## Target and prediction date
- Target: `dormant_within_6m` from `table9_target_dormancy.csv`.
- Observation date: `2025-01-01`.
- The notebook uses event timestamps to exclude records after the observation date and does not use target-detail fields as predictors.
- The identifier `customer_id` is used only for joining and is excluded from the feature matrix.
- Table 10 is metadata without a customer identifier and is not joined to the customer-level modelling table.

## Models
The notebook compares logistic regression with random forest using a stratified 80/20 train/test split. Imputation, scaling and one-hot encoding are fitted within each pipeline on training data only. The selected model is the one with the best held-out F1-score, using ROC-AUC as a tie-breaker.

## Dependencies
Install if needed:
```bash
pip install pandas numpy matplotlib scikit-learn jupyter
```

## GitHub commit history
Commit the work in separate stages, rather than uploading everything in one commit. Suggested commits:
1. Add SS3 Part B notebook scaffold and dataset loading.
2. Add point-in-time feature engineering and preprocessing.
3. Add logistic regression and random forest training.
4. Add test-set validation metrics and classification report.
5. Add result visualisations and README documentation.



