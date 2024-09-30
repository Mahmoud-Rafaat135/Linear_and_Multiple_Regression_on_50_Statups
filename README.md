# Linear_and_Multiple_Regression_on_50_Statups
 You are predicting the company's profit based on features like R&D Spend, Administration, Marketing Spend, and State. You used three models: two linear regression models (Model 1 and Model 2) and an XGBoost model (Model 3), comparing their performance
Model 1: Simple Linear Regression
Target variable: Profit
Feature used: R&D Spend
Steps:
Split the data into training and test sets (train_test_split).
Scaled the R&D Spend feature using StandardScaler.
Trained a linear regression model using the scaled feature.
Obtained predictions and evaluated performance.
Result: The model had an RMSE of ~6955, with good accuracy on both training (95.69%) and testing (94.04%).
Model 2: Multiple Linear Regression
Target variable: Profit
Features used: R&D Spend, Administration, Marketing Spend, and State
Steps:
Same preprocessing and scaling steps, but included all four features this time.
Trained a multiple linear regression model.
Obtained predictions and evaluated performance.
Result: The model showed a higher RMSE (~8118), indicating a slight overfitting despite using all features. The training score was higher than Model 1 (96.40%), but the testing score was slightly lower (91.87%).
Model 3: XGBoost Regressor
You introduced XGBoost as a third model to improve prediction performance:
Used the scaled data to train an XGBoost model.
The RMSE was higher than both linear regression models (~11,709), suggesting XGBoost did not outperform the simpler models in this case.
Evaluation Metrics
For all models, you used:

Mean Absolute Error (MAE): measures the average magnitude of errors.
Root Mean Squared Error (RMSE): emphasizes larger errors more, useful for seeing model fit in comparison to others.
