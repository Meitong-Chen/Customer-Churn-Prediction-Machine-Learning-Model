# Customer Churn Prediction Project

## Project Overview
This project develops predictive models to analyze customer churn for a bank. The process involves data cleaning, feature engineering, and deploying various machine learning models to predict the likelihood of customers discontinuing their services.

## Data Preparation
The dataset is initially processed to optimize it for modeling:
- **Initial Cleaning**: Unnecessary identifiers such as 'RowNumber', 'CustomerId', and 'Surname' are removed to focus on relevant data.
- **Transformation**: Categorical variables 'Geography' and 'Gender' are encoded numerically. 'Balance' and 'EstimatedSalary' are scaled using MinMaxScaler to normalize their distributions.

## Feature Engineering
The analytical approach includes both statistical summaries and visual explorations:
- **Statistical Analysis**: Descriptive statistics are calculated for all numerical features to understand data distributions.
- **Visualization**: Distribution plots and box plots are generated for each numerical feature to identify outliers and distribution characteristics.
- **Correlation Analysis**: A correlation matrix is visualized through a heatmap to detect relationships between features and guide feature selection.

## Modeling
Three models are evaluated for their effectiveness in predicting customer churn:
1. **Logistic Regression**: Implemented with a class balance mechanism to handle unequal class distributions.
2. **Support Vector Machine (SVM)**: Configured with different kernels to find the optimal boundary between classes.
3. **Random Forest**: Analyzed with varying numbers of trees and depths to capture complex patterns in the data.

### Model Evaluation
- **Performance Metrics**: Each model is assessed using precision, recall, and the ROC AUC score to determine its predictive accuracy.
- **Model Selection**: Grid search techniques are utilized to fine-tune model parameters and select the best performer based on accuracy metrics.
- **Visualization**: ROC curves are plotted to visually compare model performances.

## Conclusion
The project concludes with a detailed discussion of each model's performance, focusing on their practical implications for identifying and mitigating customer churn. The effectiveness of the models is compared, and the best-performing model is highlighted based on key metrics.

## Running the Project
Ensure the following are installed: Python, pandas, numpy, matplotlib, seaborn, and sklearn. Download the dataset and adjust the file path in the script as necessary. Execute the script sequentially to reproduce the results.

