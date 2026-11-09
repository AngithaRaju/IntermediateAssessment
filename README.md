Car Price Prediction – End-to-End Machine Learning Project

1. Project Overview

This project aims to predict car prices in the US automobile market using machine learning regression algorithms. The analysis helps identify the key factors influencing car prices and provides insights into the characteristics that determine vehicle value.

2. Business Problem

A Chinese automobile company plans to enter the US market. The objective is to understand the factors affecting car prices in the American market and develop a predictive model to estimate car prices based on various automobile features.

3. Dataset Description

The dataset contains information about different cars, including their technical specifications, dimensions, engine characteristics, fuel type, and other attributes.

Target Variable: price

Problem Type: Supervised Machine Learning – Regression

4. End-to-End Workflow

Step 1: Data Loading and Understanding

Loaded the dataset using Pandas.

Examined dataset dimensions, data types, and statistical summaries.

Identified numerical and categorical variables.

Checked for missing values and duplicate records.

Step 2: Exploratory Data Analysis (EDA)

Analyzed the distribution of car prices.

Studied relationships between independent variables and car prices.

Used histograms, box plots, heatmaps, and correlation analysis.

Identified patterns, outliers, and potential relationships.

Step 3: Data Preprocessing

Removed unnecessary identifier columns such as car_ID.

Extracted manufacturer and model names from the CarName column.

Standardized inconsistent manufacturer names.

Checked and handled missing values.

Separated independent variables (X) and the target variable (y).

Step 4: Feature Engineering and Encoding

Created meaningful features from the original car name.

Applied One-Hot Encoding to categorical variables.

Aligned training and testing feature columns.

Step 5: Train-Test Split

Divided the dataset into training and testing sets.

Used 80% of the data for training and 20% for testing.

Set a random state to ensure reproducibility.

Step 6: Feature Scaling and Feature Selection

Applied StandardScaler to standardize the input features.

Used SelectKBest with the f_regression scoring function to select the top 15 features.

Identified relevant features for model training.

Step 7: Model Building

Implemented and compared seven regression algorithms:

Linear Regression

Ridge Regression

Lasso Regression

Decision Tree Regressor

Random Forest Regressor

Gradient Boosting Regressor

Support Vector Regressor (SVR)

Step 8: Model Evaluation

Evaluated model performance using:

R² Score: Measures how well the model explains variations in car prices.

Mean Squared Error (MSE): Measures the average squared prediction error.

Mean Absolute Error (MAE): Measures the average absolute prediction error.

Random Forest Regressor achieved the best initial performance with an R² score of approximately 0.9574.

Step 9: Feature Importance Analysis

Used Random Forest Feature Importance to identify significant variables.

Ranked features based on their contribution to model predictions.

Visualized the top 10 important features.

Analyzed the impact of feature selection on prediction performance.

Step 10: Hyperparameter Tuning

Applied RandomizedSearchCV to optimize Random Forest hyperparameters.

Used 5-fold cross-validation.

Tuned parameters such as n_estimators, max_depth, min_samples_split, min_samples_leaf, and max_features.

Compared tuned and original model performance.

The original Random Forest model performed better than the tuned model on the test dataset.

Step 11: Final Model Selection

Based on the evaluation metrics, the original Random Forest Regressor was selected as the best-performing model among the seven algorithms tested.

5. Technologies and Libraries Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

 Google Colab

 7. Final Conclusion

The project demonstrates an end-to-end machine learning approach to predicting car prices using various regression algorithms. Among the seven models evaluated, Random Forest Regressor achieved the highest initial R² score of approximately 95.74%, with relatively low prediction errors.

Feature importance analysis helped identify the most relevant variables contributing to car price predictions. Hyperparameter tuning was also performed to optimize the model, although the original Random Forest model demonstrated better test performance.

Overall, the project highlights how machine learning can support automobile market analysis and help identify the key factors influencing vehicle pricing.
