
# California House Price Prediction

## Project Overview

A machine learning project that predicts median
house values using the California Housing Dataset.

The project compares three regression models and
investigates the effect of hyperparameter tuning.

## Dataset

- Dataset: California Housing Dataset
- Observations: 20,640
- Input features: 8
- Target: Median house value
- Target unit: $100,000

## Technologies

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Project Workflow

1. Dataset loading and inspection
2. Exploratory Data Analysis
3. Missing value and duplicate checks
4. Correlation analysis
5. Feature and target separation
6. Train-test split (80/20)
7. Linear Regression
8. Random Forest Regression
9. Hyperparameter tuning
10. Model evaluation and comparison

## Model Performance

| Model | MAE | MSE | RMSE | R2 |
|---|---:|---:|---:|---:|
| Linear Regression | 0.5332 | 0.5559 | 0.7456 | 0.5758 |
| Random Forest | 0.3275 | 0.2554 | 0.5053 | 0.8051 |
| Tuned Random Forest | 0.3283 | 0.2463 | 0.4962 | 0.8121 |

## Best Model

Tuned Random Forest Regression.

- MAE: 0.3283
- MSE: 0.2463
- RMSE: 0.4962
- R2 Score: 0.8121

## Hyperparameter Tuning

RandomizedSearchCV was used with three-fold
cross-validation and eight sampled configurations.

Best parameters:

```python
{'n_estimators': 200, 'min_samples_split': 5, 'min_samples_leaf': 1, 'max_features': 'sqrt', 'max_depth': 30}
```

## Conclusion

Random Forest outperformed Linear Regression
on the test dataset.

Hyperparameter tuning improved the R2 score
from 0.8051 to 0.8121.

The project demonstrates the use of supervised
machine learning, regression, model evaluation,
and hyperparameter optimization.

## Limitations

- The dataset represents California housing data from 1990.
- Some house values are capped at approximately $500,000.
- Results may not generalize to other locations.
- Predictions are estimates, not guaranteed property values.

## Future Improvements

- Feature importance analysis.
- Additional regression algorithms.
- More extensive hyperparameter tuning.
- Streamlit prediction application.

## Author

Machine Learning Portfolio Project
