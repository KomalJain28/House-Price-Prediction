Project Overview
This project aims to predict house prices based on various features such as area, number of bedrooms and bathrooms, number of floors, year built, location, condition, and garage availability. The dataset was preprocessed, visualized, and analyzed using multiple regression techniques to determine the best model for accurate price prediction.

Dataset Description
The dataset includes the following features:
Numerical Features: Area, Year Built, Price
Categorical Features: Bedrooms, Bathrooms, Floors, Location, Condition, Garage

Data Preprocessing
Feature Bifurcation: Separated categorical and numerical columns.
Data Visualization: Plotted various graphs to understand feature distributions and correlations.
Encoding: Applied One-Hot and Label Encoding for categorical variables.
Train-Test Split: Divided the data into 80% training and 20% testing.

Models Implemented
1. Linear Regression
Training R² Score: 0.0059
Testing R² Score: -0.0005
High multicollinearity was detected, reducing model effectiveness.

2. Polynomial Regression
Training R² Score: -27.44
Testing R² Score: -0.0166
Poor performance due to overfitting.

3. Lasso Regression (Regularization)
Training R² Score: 0.0059
Testing R² Score: -0.0005
Regularization did not improve the results significantly.

4. Ridge Regression (Regularization)
Training R² Score: 0.0059
Testing R² Score: -0.0004
Marginal improvement but still not effective.

5. Elastic Net Regression
Training R² Score: 0.0040
Testing R² Score: 0.00007
Slight improvement over Ridge and Lasso.

6. KNN Regressor
Training R² Score: 0.2016
Testing R² Score: -0.2330
Poor performance on testing data due to high variance.

7. Support Vector Regression (SVR)
Training R² Score: -0.0002
Testing R² Score: -0.0009
Failed to capture the relationship between features and price.

8. Decision Tree Regression
Training R² Score: 0.9216
Testing R² Score: -1.0065
Severe overfitting, leading to poor generalization.

9. Random Forest Regression
Training R² Score: 0.8351
Testing R² Score: -0.0548
Performed better than Decision Tree but still overfitting.

10. XGBoost Regressor
Training R² Score: 0.6996
Testing R² Score: -0.1497
Best generalization among all models but still requires tuning.

Best Model Selection
From the above results, Random Forest Regression and XGBoost Regressor performed better than other models. However, overfitting remains an issue, and further hyperparameter tuning may be required to improve generalization.

Conclusion
Feature engineering and selection need improvement to enhance model accuracy.
Regularization techniques (Lasso, Ridge, Elastic Net) did not significantly improve performance.
Ensemble methods (Random Forest, XGBoost) performed better than simple regression models.
Further tuning of hyperparameters, feature selection, and outlier treatment is needed to improve prediction accuracy.
