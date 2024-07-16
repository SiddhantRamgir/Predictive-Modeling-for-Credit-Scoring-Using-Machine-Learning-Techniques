# Credit Scoring Using Machine Learning Techniques

## Description
This project applies machine learning techniques to a credit scoring dataset to predict borrower financial distress and other features. It includes data preprocessing, model training, and evaluation for classification and regression tasks. Key models used are Random Forest, Gradient Boosting classifiers, and regressors. The study demonstrates how machine learning can improve credit scoring models and aid financial institutions in making informed lending decisions.

## Table of Contents
1. [Abstract](#abstract)
2. [Introduction](#introduction)
3. [Data Description](#data-description)
4. [Data Cleaning and Exploratory Data Analysis](#data-cleaning-and-exploratory-data-analysis)
5. [Methodology](#methodology)
    - [Data Preprocessing](#data-preprocessing)
    - [Model Training and Evaluation](#model-training-and-evaluation)
    - [Feature Importance Analysis](#feature-importance-analysis)
    - [Regression Analysis](#regression-analysis)
6. [Results and Discussion](#results-and-discussion)
7. [Conclusion](#conclusion)

## Abstract
This report presents an analysis of a credit scoring dataset using various machine learning techniques. The analysis involves data preprocessing, model training, evaluation, and comparison of different machine learning algorithms for both classification and regression tasks.

## Introduction
Credit scoring is crucial for assessing borrower creditworthiness. Machine learning offers powerful tools for predictive modeling based on historical data. This report analyzes a credit scoring dataset to predict borrower financial distress using machine learning algorithms.

## Data Description
The dataset includes features like age, income, loan history, and a target variable indicating financial distress within two years. Key features are UtilizationOfUnsecuredLinesTotal, Age, CustomerLifeTime, DebtRatio, MonthlyIncome, and various late payment indicators.

## Data Cleaning and Exploratory Data Analysis
### Data Cleaning
- **Outlier Removal:** Iterative cycles using the IQR method for key columns.
- **Duplicate Removal:** Using pandas' `.duplicated()` method.
- **Missing Value Check:** Using `.isna().sum()`.

### Exploratory Data Analysis
- **Correlation Analysis:** Using heatmaps to identify relationships.
- **Descriptive Statistics:** Summary statistics, dimensions, and data structure overview.

## Methodology
### Data Preprocessing
Data is loaded, and features (X) and target (y) are extracted. The dataset is split into training, validation, and test sets.

### Model Training and Evaluation
- **Random Forest Classifier:** Trained with class weighting, evaluated with precision, recall, F1-score, and confusion matrix.
- **Gradient Boosting Classifier:** Trained on under-sampled data, evaluated similarly.

### Feature Importance Analysis
Analyzing and plotting feature importances from the Random Forest model.

### Regression Analysis
- **Gradient Boosting Regressor:** Predicts borrower age, evaluated with mean absolute error and R-squared.
- **K-Nearest Neighbor Regressor:** Compared with Gradient Boosting Regressor on the same metrics.

## Results and Discussion
- Random Forest and Gradient Boosting classifiers' performance and their handling of imbalanced classes.
- Feature importance analysis reveals significant predictors.
- Gradient Boosting Regressor outperforms K-Nearest Neighbor Regressor in predicting borrower age.

## Conclusion
Machine learning techniques effectively enhance credit scoring models. The study emphasizes the importance of data preprocessing, model selection, and evaluation. Future work could explore additional algorithms and feature engineering to further improve predictive performance.

## Usage
Clone the repository and follow the instructions in the Jupyter notebooks to replicate the analysis. Ensure all dependencies are installed as per the `requirements.txt` file. 

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.
