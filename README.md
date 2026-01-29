
## Overview
This project predicts passenger survival on the Titanic using machine learning classification techniques. The work includes data preprocessing, exploratory data analysis, feature engineering, and model training to understand which factors most influenced survival outcomes.


## Dataset
- **Records:** 418 passengers  
- **Target Variable:** Survived  
  - 0 = Did not survive  
  - 1 = Survived  

## Exploratory Data Analysis
Exploratory analysis was performed to study survival patterns based on:
- Gender and age distribution  
- Passenger class  
- Fare ranges  
- Port of embarkation  
- Family size and whether passengers traveled alone  

Missing values in age, fare, and cabin features were identified and handled during preprocessing.


## Feature Engineering
The following feature transformations were applied:
- Created family-based features such as `relatives` and `not_alone`
- Extracted passenger titles from names and encoded them numerically
- Converted categorical variables (Sex, Embarked, Deck) into numerical values
- Binned age and fare into ordinal categories
- Generated interaction features including `Age_Class` and `Fare_Per_Person`
- Removed non-informative features such as passenger name, ticket number, and cabin


## Models Used
The following machine learning models were implemented:
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- Support Vector Machine (SGD-based)


## Tools & Technologies
- Python  
- NumPy, Pandas  
- Matplotlib, Seaborn  
- Scikit-learn  

## Output
The notebook produces:
- Survival predictions for passengers
- Accuracy scores for trained models
- Visualizations highlighting relationships between features and survival outcomes

The results show that feature engineering plays a significant role in improving model performance.

## Key Learnings
- Feature engineering has a strong impact on prediction quality
- Family-related and socio-economic features are important indicators of survival
- Comparing multiple models helps understand performance trade-offs

## Future Work
- Apply cross-validation to reduce overfitting
- Perform hyperparameter tuning
- Evaluate models on unseen data
- Add model explainability techniques
