# Term Deposit Subscription Prediction

A machine learning project to predict whether a customer will subscribe to a term deposit based on historical data. This end-to-end solution covers data preprocessing, exploratory data analysis (EDA), model building, performance evaluation, and deployment of the best-performing classifier.

---

##  Problem Statement

Financial institutions aim to optimize marketing strategies for term deposit offerings. This project uses customer and campaign data to build a predictive model that classifies whether a client will subscribe to a term deposit or not.

---

##  Dataset Overview

- **Source:** UCI Bank Marketing Dataset
- **Records:** 41,188 customer entries
- **Features:** 20 attributes including:
  - Client attributes (e.g., age, job, marital, education)
  - Campaign interaction details (e.g., contact type, day, duration)
  - Economic indicators (e.g., employment variation rate, consumer confidence)

Target variable: `y` – whether the client subscribed (`yes`/`no`)

---

##  Project Pipeline

1. **Data Cleaning and Preprocessing**
   - Handled missing values and categorical encoding
   - Standardized numerical features

2. **Exploratory Data Analysis (EDA)**
   - Analyzed class imbalance
   - Explored correlations between predictors and target
   - Visualized customer behavior and feature distributions

3. **Model Building**
   - Compared the performance of 7 classification models:
     - Logistic Regression
     - Decision Tree
     - Random Forest
     - XGBoost
     - K-Nearest Neighbors
     - Support Vector Machine (SVM)
     - Naive Bayes

4. **Model Evaluation**
   - Metrics used: Accuracy, F1 Score, AUC-ROC, Recall
   - Hyperparameter tuning using GridSearchCV
   - Selected SVM as the best model based on overall performance

5. **Deployment (Optional)**
   - Trained model saved using `joblib`
   - Predictive pipeline ready for integration with front-end or dashboard

---

##  Key Results

| Model             | Accuracy | F1 Score | AUC Score | Recall |
|------------------|----------|----------|-----------|--------|
| Logistic Regression | 0.89     | 0.47     | 0.88      | 0.63   |
| Random Forest     | 0.90     | 0.52     | 0.89      | 0.61   |
| SVM (Best)        | 0.91     | 0.53     | 0.91      | 0.67   |

---


