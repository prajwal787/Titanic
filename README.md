# Titanic Survival Prediction

## Project Overview

This project aims to build a machine learning model to predict whether a passenger on the Titanic would have survived the disaster. Using the Titanic dataset from Kaggle, we perform data analysis, feature engineering, and apply classification algorithms to predict survival. This project serves as a practical application of a complete machine learning workflow.

## Dataset

The dataset used in this project is the Titanic dataset from Kaggle. It contains information about the passengers on the Titanic, including:

| Column | Description |
|---|---|
| `PassengerId` | Unique ID for each passenger |
| `Survived` | Survival (0 = No, 1 = Yes) |
| `Pclass` | Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd) |
| `Name` | Name of passenger |
| `Sex` | Gender of passenger |
| `Age` | Age in years |
| `SibSp` | # of siblings/spouses aboard |
| `Parch` | # of parents/children aboard |
| `Ticket` | Ticket number |
| `Fare` | Ticket fare |
| `Cabin` | Cabin number |
| `Embarked` | Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton) |

## Methodology

The project follows these steps:

1.  **Data Loading and Exploration**: The dataset is loaded, and an initial exploratory data analysis (EDA) is performed to understand the data's structure, identify missing values, and visualize relationships between different features.
2.  **Data Preprocessing**:
    *   Missing values in the `Age` and `Embarked` columns are imputed.
    *   Categorical features like `Sex` and `Embarked` are converted into numerical format using one-hot encoding.
    *   Irrelevant columns like `Name`, `Ticket`, and `Cabin` are dropped.
3.  **Model Training**: Two classification models are trained on the preprocessed data:
    *   Logistic Regression
    *   Random Forest Classifier
4.  **Model Evaluation**: The performance of each model is evaluated using metrics such as accuracy, precision, recall, and F1-score.
5.  **Hyperparameter Tuning**: GridSearchCV is used to find the optimal hyperparameters for both the Logistic Regression and Random Forest models to improve their performance.

## Results

The performance of the models is summarized below:

| Model | Accuracy | Precision (Survived) | Recall (Survived) |
|---|---|---|---|
| Logistic Regression | 0.80 | 0.77 | 0.74 |
| Tuned Logistic Regression | 0.80 | 0.78 | 0.72 |
| Random Forest | 0.82 | 0.81 | 0.74 |
| Tuned Random Forest | 0.82 | 0.81 | 0.74 |

The Random Forest model slightly outperformed the Logistic Regression model, achieving an accuracy of 82%.

 
