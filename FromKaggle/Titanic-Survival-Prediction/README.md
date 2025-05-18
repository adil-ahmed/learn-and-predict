# Titanic - Machine Learning from Disaster 🚢  
A Kaggle project predicting survival on the Titanic using Random Forest Classifier.

## 🧠 Objective  
To build and evaluate a machine learning model that predicts which passengers survived the Titanic disaster based on passenger features.

This is one of the most popular beginner-friendly classification problems hosted on [Kaggle](https://www.kaggle.com/competitions/titanic).

---

## 📊 Dataset Overview

We used the datasets provided by the competition:
- `train.csv` — contains the training data with labels
- `test.csv` — contains the test data without labels

Main features include:  
- `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Embarked`, `Cabin`, `Name`

---

## 🛠️ Process Summary

### 1. Data Cleaning & Preprocessing
- Imputed missing values (Age, Embarked, Fare)
- Feature Engineering:
  - Extracted `Title` from `Name`
  - Created `FamilySize` and `IsAlone` features
  - Created `HasCabin` binary feature
- One-hot encoding for categorical variables (`Embarked`, `Title`)
- Mapped `Sex` to binary

### 2. Model Training
- Model Used: `RandomForestClassifier` from scikit-learn
- Train/Test split used for local evaluation
- Final accuracy on validation set: **~83%**

### 3. Submission
- Predictions made on test set
- `submission.csv` prepared and submitted to Kaggle
- Public leaderboard score: **0.76**

---

## 📈 Libraries Used
- `pandas`, `numpy`
- `scikit-learn`
- `seaborn`, `matplotlib`

---

## 🏷️ Tags
`Machine Learning` `Kaggle` `Titanic` `Random Forest` `Classification` `Data Science`
