itanic Survival Prediction
Overview

This project predicts passenger survival on the Titanic using machine learning classification techniques. The work includes data preprocessing, exploratory data analysis, feature engineering, and model training to understand which factors most influenced survival outcomes.

Dataset

File: tested.csv

Records: 418 passengers

Target Variable: Survived (0 = Did not survive, 1 = Survived)

Exploratory Data Analysis

Exploratory analysis was performed to study survival patterns based on:

Gender and age distribution

Passenger class

Fare ranges

Port of embarkation

Family size and whether passengers traveled alone

Missing values in age, fare, and cabin features were identified and handled during preprocessing.

Feature Engineering

The following feature transformations were applied:

Created family-based features such as relatives and not_alone

Extracted passenger titles from names and encoded them numerically

Converted categorical variables (Sex, Embarked, Deck) into numerical values

Binned age and fare into ordinal categories

Generated interaction features including Age_Class and Fare_Per_Person

Removed non-informative features such as passenger name, ticket number, and cabin

Models Used

Multiple machine learning classifiers were implemented and compared, including:

Logistic Regression

K-Nearest Neighbors (KNN)

Decision Tree

Random Forest

Support Vector Machine (SGD-based)

Output

The final output of the project is a trained classification model capable of predicting whether a passenger survived based on input features. The notebook outputs:

Survival predictions for passengers

Model accuracy scores during training

Visualizations illustrating feature relationships and survival trends

The results demonstrate that engineered features significantly improve predictive performance.

Tools & Technologies

Python

NumPy, Pandas

Matplotlib, Seaborn

Scikit-learn

Key Learnings

Feature engineering has a strong impact on classification performance.

Family-related and socio-economic features are important predictors of survival.

Comparing multiple models helps in understanding trade-offs between interpretability and performance.

Future Work

Introduce cross-validation to reduce overfitting

Perform hyperparameter tuning

Evaluate models on unseen test data

Add explainability using feature importance or SHAP
