# House Price Prediction with Ensembles

Predicting home sale prices on the House Price dataset using tree-based ensemble models. The workflow includes data cleaning, feature engineering, model training, evaluation, and generating Kaggle-ready submissions.

## Models
- Random Forest (bagging)
- Gradient Boosting (sklearn)
- XGBoost
- LightGBM
- Stacking ensemble (Ridge meta-learner)

## Key Metrics (validation)
- RMSE, MAE, R²

## How to run
1. Open the notebook `house-prices-prediction-using-rf.ipynb` in VS Code or Jupyter.
2. Run cells in order; the notebook installs any missing packages.
3. Compare model metrics, then generate a submission with the best model.
	 - Outputs:
		 - `xgboost_submission.csv`

## Notes
- Feature engineering includes total baths, total square footage, porch area, age features, and simple interactions.
- Categorical NAs like PoolQC, Alley, Fence are encoded as explicit "None" categories; numeric absences (e.g., MasVnrArea) are filled with 0.

## Reference
[Kaggle(Dataset)](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)
