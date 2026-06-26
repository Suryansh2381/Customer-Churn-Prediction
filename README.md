# Customer Churn Prediction

A machine learning project that predicts whether a telecom customer is likely to churn using the IBM Telco Customer Churn dataset. The project covers the complete ML workflow, from data preprocessing and exploratory data analysis to model training, evaluation, and interpretation.

---

## Project Overview

Customer churn prediction helps businesses identify customers who are likely to discontinue a service, enabling proactive retention strategies. This project develops a machine learning classification model using the IBM Telco Customer Churn dataset, with **recall** prioritized to maximize the identification of customers at risk of churn.

* Built an end-to-end customer churn prediction pipeline.
* Performed data cleaning, feature engineering, and exploratory data analysis.
* Trained and compared multiple classification models.
* Selected the **Tuned Random Forest** model based on its highest recall.
* Interpreted model predictions using Feature Importance and SHAP.

---

## Dataset

**IBM Telco Customer Churn Dataset**

https://www.kaggle.com/datasets/yeanzc/telco-customer-churn-ibm-dataset

---

## Skills & Technologies

**Language**

* Python

**Libraries**

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* SHAP

**Machine Learning**

* Data Preprocessing
* Exploratory Data Analysis (EDA)
* Feature Engineering
* One-Hot Encoding
* Feature Scaling
* Class Imbalance Handling
* Hyperparameter Tuning (RandomizedSearchCV)
* Model Evaluation
* Model Explainability

**Models**

* Logistic Regression
* Decision Tree
* Random Forest
* XGBoost

---

## Model Performance

| Model                   |    Recall |  Accuracy |  F1-score |
| ----------------------- | --------: | --------: | --------: |
| Logistic Regression     |     54.3% |     79.9% |     58.9% |
| Decision Tree           |     51.1% |     78.3% |     55.5% |
| Random Forest           |     80.2% |     71.9% |     60.3% |
| **Tuned Random Forest** | **81.3%** | **70.8%** | **59.7%** |
| XGBoost                 |     54.3% |     79.2% |     58.2% |
| Tuned XGBoost           |     53.2% |     79.3% |     57.8% |

**Final Model:** Tuned Random Forest (selected for achieving the highest recall, aligning with the project's objective of maximizing churn detection.)

---

## Key Insights

* Customer tenure was the strongest predictor of churn.
* Contract type, payment method, and internet service significantly influenced churn.
* Customers with month-to-month contracts showed a higher likelihood of leaving.

---

## Future Improvements

* Evaluate the model on larger real-world telecom datasets.
* Experiment with advanced ensemble techniques to further improve recall.
