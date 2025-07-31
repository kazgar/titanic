# Titanic - Machine Learning from Disaster

This repository is a Kaggle competition submission for the classic **Titanic** dataset. The goal is to build a predictive model that determines whether a passenger survived the Titanic shipwreck based on features like age, sex, class, and more.

## Dataset

The dataset includes:

- `train.csv`: labeled training data (used to train and validate the model)
- `test.csv`: test data (for which predictions are made and submitted to Kaggle)

Key features:

- `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Cabin`, `Embarked`, `Name`

## Methods and Workflow

### 1. Data Exploration (EDA)

- Visualized feature distributions and survival rates across classes
- Identified missing values and feature skew

### 2. Feature Engineering

- Extracted titles (prefixes) from names
- Created age groups and fare groups
- Generated new features like family size
- Imputed missing values based on conditional logic (e.g., age by gender)

### 3. Preprocessing Pipelines

- Built custom `AttributeTransformer` for feature creation
- Applied one-hot encoding to categorical variables
- Used `SimpleImputer` for missing values
- Combined transformations with `ColumnTransformer` and `Pipeline`

### 4. Modeling

- Tried baseline models (e.g., logistic regression)
- Focused on understanding how different features affect predictions
- Tracked performance using accuracy score

## Results

Achieved up to **78–79% accuracy**, matching common benchmarks. The focus was on building robust preprocessing and gaining hands-on experience with:

- Scikit-learn pipelines
- Transformer classes
- Preparing real-world data

______________________________________________________________________

## Acknowledgements

The Titanic competition on [Kaggle](https://www.kaggle.com/c/titanic).
