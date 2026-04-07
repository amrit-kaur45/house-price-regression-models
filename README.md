<b>California Housing Price Prediction</b>
<br>
# Overview
This project focuses on predicting housing prices using the California Housing dataset. Multiple supervised learning regression models are implemented and compared to evaluate their performance.

# Objectives
Apply and compare different regression algorithms
Understand the effect of regularization techniques
Explore tree-based and ensemble learning methods
Evaluate model performance using standard regression metrics

# Technologies Used
Python
NumPy
Pandas
Matplotlib
Seaborn
Scikit-learn
XGBoost
Dataset
Source: sklearn.datasets.fetch_california_housing
The dataset includes features such as median income, house age, average rooms, population, and location-based attributes

# Workflow
1. Data Preprocessing
Checked for missing values
Split dataset into training and testing sets (80/20)
Applied feature scaling using StandardScaler
2. Models Implemented
Linear Regression
Ridge Regression (L2 Regularization)
Lasso Regression (L1 Regularization)
Decision Tree Regressor
Random Forest Regressor
XGBoost Regressor
AdaBoost Regressor
3. Hyperparameter Tuning
GridSearchCV used for Ridge, Lasso, and XGBoost
4. Evaluation Metrics
R² Score
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
Mean Absolute Error (MAE)
5. Visualization
Scatter plots of actual vs predicted values
Diagonal reference line for performance comparison
Results Summary
Model	Performance
Linear Regression	Moderate
Ridge Regression	Similar to Linear
Lasso Regression	Similar with slight feature reduction
Decision Tree	Tendency to overfit
Random Forest	Strong performance
XGBoost	Best performance
AdaBoost	Good performance

# Key Insights
Linear, Ridge, and Lasso models showed similar performance, indicating limited impact of regularization
Decision Trees produced step-like predictions and showed overfitting tendencies
Random Forest improved performance by reducing overfitting
XGBoost achieved the best results by capturing complex patterns in the data
Feature importance analysis highlighted the most influential variables
Conclusion

Tree-based ensemble models outperform linear models for this dataset. XGBoost provides the most accurate and robust predictions.

# How to Run

pip install numpy pandas matplotlib seaborn scikit-learn xgboost
python main.py

# Future Work
Add cross-validation comparison for all models
Perform feature engineering
Explore advanced boosting models such as LightGBM and CatBoost
Deploy the model using Flask or Streamlit
Acknowledgements
Scikit-learn dataset repository
Open-source machine learning community
