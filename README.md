# spaceship_anamoly_survival_pred
🚀 Spaceship Titanic ML project predicting passenger transport using tabular data. Applied EDA, feature engineering (TotalSpend, GroupSize, Deck), and models like XGBoost. Used logical imputation and cross-validation to achieve ~0.80+ accuracy. Focused on strong tabular ML pipeline and real-world problem solving.

# 🚀 Spaceship Titanic Survival Prediction

This project is my solution to the Kaggle competition **Spaceship Titanic**, where the goal is to predict whether a passenger was transported to an alternate dimension after a spaceship anomaly.

## 📌 Problem Statement

Given passenger data such as demographics, spending patterns, and cabin information, the task is to build a machine learning model that accurately predicts the binary target variable **`Transported`**.

---

## 🧠 Approach

### 🔹 Exploratory Data Analysis (EDA)

* Analyzed distributions of key variables like `CryoSleep`, `HomePlanet`, and spending features
* Identified strong signals such as:

  * CryoSleep → high correlation with transport
  * Total spending → inverse relationship with transport
  * Cabin deck → location-based effects

---

### 🔹 Feature Engineering

* Extracted **Deck, CabinNum, Side** from cabin information
* Created **TotalSpend** from all expenditure features
* Engineered **GroupSize** and **IsAlone** from PassengerId
* Applied logical imputation for **CryoSleep** using spending behavior
* Binned **Age** to capture nonlinear patterns

---

### 🔹 Data Preprocessing

* Handled missing values using domain-driven strategies
* One-hot encoded categorical variables
* Ensured alignment between train and test datasets

---

### 🔹 Modeling

Implemented and compared multiple models:

* **XGBoost (primary model)**
* Random Forest
* Support Vector Machine (SVM)

Final approach used:

* Hyperparameter tuning
* Cross-validation (Stratified K-Fold)
* Ensemble (soft voting)

---

## 📊 Results

* Validation Accuracy: ~0.80–0.83
* Public Leaderboard Score: *(update with your score)*

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* XGBoost

---

## 📁 Project Structure

```
├── data/
├── notebooks/
├── src/
├── submission.csv
└── README.md
```

---

## 🚀 Key Learnings

* Importance of feature engineering in tabular ML
* Handling missing values using domain logic
* Benefits of cross-validation over single split
* Practical implementation of ensemble models

---

## 🔗 Kaggle Competition

https://www.kaggle.com/competitions/spaceship-titanic


⭐ If you found this useful, feel free to star the repository!
