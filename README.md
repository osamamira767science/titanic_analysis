# Titanic Dataset Analysis

## Overview

This repository contains an analysis of the famous **Titanic dataset**, which provides information about passengers aboard the RMS Titanic. The dataset includes various features that describe each passenger, such as their age, gender, ticket class, fare, and whether they survived the disaster.

### Dataset Description

The dataset contains the following columns:

- **PassengerId**: A unique identifier for each passenger.
- **Survived**: Indicates whether the passenger survived (1) or did not survive (0).
- **Pclass**: The passenger class (1 = 1st class, 2 = 2nd class, 3 = 3rd class).
- **Name**: The name of the passenger.
- **Sex**: The gender of the passenger (male/female).
- **Age**: The age of the passenger (some values are missing).
- **SibSp**: The number of siblings/spouses aboard the Titanic.
- **Parch**: The number of parents/children aboard the Titanic.
- **Ticket**: The ticket number.
- **Fare**: The fare paid by the passenger.
- **Cabin**: The cabin number (many values are missing).
- **Embarked**: The port where the passenger embarked (C = Cherbourg, Q = Queenstown, S = Southampton).

### Key Observations

- **Missing Data**: Some entries have missing values for **Age**, **Cabin**, and **Embarked**.
- **Target Variable**: The **Survived** column is the target variable for predictive modeling.
- **Features**: Potential predictors for survival include **Pclass**, **Sex**, **Age**, **SibSp**, **Parch**, **Fare**, and **Embarked**.

### Analysis Steps

1. **Exploratory Data Analysis (EDA)**:
   - Visualize the distribution of key features like **Age**, **Fare**, and **Pclass**.
   - Analyze the relationship between **Survived** and other variables (e.g., survival rates by gender, class, age group).
   - Check for correlations between numerical features (e.g., **Fare** and **Pclass**).

2. **Handling Missing Data**:
   - Impute missing **Age** values using mean, median, or more sophisticated methods.
   - Decide how to handle missing **Cabin** values (e.g., drop the column, create a binary indicator for missing vs. non-missing).
   - Impute or drop rows with missing **Embarked** values.

3. **Feature Engineering**:
   - Extract titles from **Name** (e.g., Mr., Mrs., Miss, Master) as a new feature.
   - Create family size by combining **SibSp** and **Parch**.
   - Encode categorical variables like **Sex** and **Embarked** (e.g., one-hot encoding or label encoding).

4. **Modeling**:
   - Build predictive models (e.g., logistic regression, decision trees, random forests) to predict **Survived** based on other features.
   - Evaluate model performance using metrics like accuracy, precision, recall, and F1-score.

### Example Questions for Further Analysis

- What is the survival rate by passenger class?
- How does age correlate with survival?
- Are there any patterns in survival based on the port of embarkation?
- Does having family members (siblings/spouses or parents/children) aboard affect survival chances?

For more details, check out the [Jupyter Notebook](link_to_your_notebook.ipynb) in this repository, which contains the full analysis and code.

---

Feel free to contribute or suggest improvements!
