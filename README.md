# Titanic Disaster Prediction

## Overview
This project aims to predict the survival of passengers on the Titanic using machine learning techniques. The dataset used for this analysis includes various features such as passenger demographics, ticket information, and fare prices.

## Dataset
The dataset used is the Titanic dataset, which includes the following columns:
- **Survived**: Survival status (0 = No, 1 = Yes)
- **Pclass**: Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd)
- **Sex**: Gender of the passenger
- **Age**: Age of the passenger
- **SibSp**: Number of siblings or spouses aboard the Titanic
- **Parch**: Number of parents or children aboard the Titanic
- **Fare**: Fare paid by the passenger
- **Embarked**: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)
- **Pclass_Fare**: Derived feature representing the product of passenger class and fare.

## Key Steps
1. **Data Preprocessing**: 
   - Removed irrelevant columns such as `PassengerId`, `Name`, `Cabin`, and `Ticket`.
   - Handled missing values in the `Age` column by filling with the mean.
   - Encoded categorical variables using one-hot encoding for `Embarked` and converted `Sex` to binary.
   - Scaled numerical features (`Age` and `Fare`) for better model performance.
   - Applied SMOTE to address class imbalance.

2. **Model Training**: 
   - Used Logistic Regression and performed hyperparameter tuning using GridSearchCV to find the best parameters.
   - Evaluated the model using accuracy, confusion matrix, and classification report.

3. **Results**: 
   - Achieved an accuracy score of **82%**.
   - The model showed promising results in predicting survival with a confusion matrix indicating good classification performance.

## Conclusion
This project demonstrates the effectiveness of machine learning techniques in predicting survival outcomes. The insights gained from this analysis can contribute to better understanding the factors influencing survival on the Titanic.

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Seaborn
- Matplotlib
- Imbalanced-learn
