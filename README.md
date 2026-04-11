# California Housing Price Prediction
<br>

## Overview
This project focuses on predicting housing prices using the California Housing dataset. Multiple supervised learning regression models are implemented and compared to evaluate their performance.

## Objectives
<ul> <li>Apply and compare different regression algorithms</li><br> <li>Understand the effect of regularization techniques</li><br> <li>Explore tree-based and ensemble learning methods</li><br> <li>Evaluate model performance using standard regression metrics</li> </ul>

## Technologies Used
<ul> <li>Python</li><br> <li>NumPy</li><br> <li>Pandas</li><br> <li>Matplotlib</li><br> <li>Seaborn</li><br> <li>Scikit-learn</li><br> <li>XGBoost</li> </ul>

## Dataset

Source: sklearn.datasets.fetch_california_housing<br>
The dataset includes features such as median income, house age, average rooms, population, and location-based attributes

## Workflow
### 1. Data Preprocessing
<ul> <li>Checked for missing values</li><br> <li>Split dataset into training and testing sets (80/20)</li><br> <li>Applied feature scaling using StandardScaler</li> </ul>

### 2. Models Implemented
<ul> <li>Linear Regression</li><br> <li>Ridge Regression (L2 Regularization)</li><br> <li>Lasso Regression (L1 Regularization)</li><br> <li>Decision Tree Regressor</li><br> <li>Random Forest Regressor</li><br> <li>XGBoost Regressor</li><br> <li>AdaBoost Regressor</li> </ul>

### 3. Hyperparameter Tuning
<ul> <li>GridSearchCV used for Ridge, Lasso, and XGBoost</li> </ul>

### 4. Evaluation Metrics
<ul> <li>R² Score</li><br> <li>Mean Squared Error (MSE)</li><br> <li>Root Mean Squared Error (RMSE)</li><br> <li>Mean Absolute Error (MAE)</li> </ul>

### 5. Visualization
<ul> <li>Scatter plots of actual vs predicted values</li><br> <li>Diagonal reference line for performance comparison</li> </ul>

# Key Insights
<ul> <li>Linear, Ridge, and Lasso models showed similar performance, indicating limited impact of regularization</li><br> <li>Decision Trees produced step-like predictions and showed overfitting tendencies</li><br> <li>Random Forest improved performance by reducing overfitting</li><br> <li>XGBoost achieved the best results by capturing complex patterns in the data</li><br> <li>Feature importance analysis highlighted the most influential variables</li> </ul>

## Conclusion

Tree-based ensemble models outperform linear models for this dataset. XGBoost provides the most accurate and robust predictions.

## How to Run

pip install numpy pandas matplotlib seaborn scikit-learn xgboost
python main.py

## Future Work
<ul> <li>Add cross-validation comparison for all models</li><br> <li>Perform feature engineering</li><br> <li>Explore advanced boosting models such as LightGBM and CatBoost</li><br> <li>Deploy the model using Flask or Streamlit</li> </ul>

## Acknowledgements
<ul> <li>Scikit-learn dataset repository</li><br> <li>Open-source machine learning community</li> </ul>
