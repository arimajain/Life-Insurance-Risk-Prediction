# Life Insurance Risk Prediction

## Project Overview

This project focuses on predicting the risk level for life insurance applicants using machine learning. By analyzing key health and personal history attributes such as BMI, age, height, weight, employment history, insurance history, and medical history, the model aims to assist in decision-making for life insurance eligibility and risk assessment.

---

## Dataset

The project utilizes the **Prudential Life Insurance Assessment** dataset, which contains over 50,000 applications with more than 100 variables describing various attributes of life insurance applicants. This comprehensive dataset provides a rich foundation for predictive modeling of insurance risk.

---

## Exploratory Data Analysis (EDA)

During EDA, it was found that:

- **BMI (Body Mass Index)** is one of the most significant factors affecting insurance risk. Applicants with BMI values roughly between 0.12 and 0.50 tend to have a higher likelihood of being approved.
- **Age** also plays a critical role, with younger applicants generally being preferred for insurance coverage.
- Other features did not reveal strong or clear patterns related to insurance risk.

Visualizations such as distribution plots and pairplots helped in identifying these trends and relationships within the data.

---

## Machine Learning Model

A **Random Forest Classifier** was chosen for its robustness and ability to handle complex, high-dimensional data. 

- Hyperparameter tuning was performed using **GridSearchCV** with the **ROC AUC** metric to optimize model performance.
- The model achieved an accuracy of approximately **80.8% on the training data** and **80.4% on the test data**, indicating good generalization capability.

Confusion matrices were used to evaluate classification performance on both training and test datasets.

---

## Model Interpretation

To understand the driving factors behind the model’s predictions:

- Feature importance analysis identified the most influential variables affecting insurance risk predictions.
- **SHAP (SHapley Additive exPlanations)** values were used to interpret individual predictions, providing insights into how different features contribute to the model’s decisions.

This interpretability ensures transparency and trust in the predictive model, which is critical in insurance applications.

---

## Conclusion

The project successfully demonstrates the application of machine learning to predict life insurance risk based on personal health and history data. With an accuracy exceeding 80%, the Random Forest model serves as a reliable tool for insurance risk assessment. Model interpretability techniques further enhance understanding of key risk factors, aiding stakeholders in making informed decisions.

---

## Tools and Libraries

- Python 3
- Scikit-learn for machine learning and hyperparameter tuning
- SHAP for model interpretability
- Pandas and NumPy for data processing
- Matplotlib and Seaborn for visualization

---

## References

- Prudential Life Insurance Assessment dataset
- Random Forest and ensemble learning methods
- SHAP methodology for explainable AI

---
