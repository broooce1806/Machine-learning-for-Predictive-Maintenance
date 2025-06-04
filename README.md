**Predictive Maintenance – Machine Learning Classifier**


Overview
This project uses machine learning to predict potential failures in industrial machines based on sensor and operational data. The solution applies multiple classification models to forecast failures and specific failure types, enabling proactive maintenance and minimizing downtime.

Features
Multi-Target Classification: Predicts both general machine failure and sub-failure types (TWF, HDF, PWF).

End-to-End Workflow: Includes data cleaning, EDA, feature engineering, model selection, and evaluation.

Model Persistence: Trained models saved using joblib or pickle for easy deployment.

Jupyter Notebooks: Step-by-step explanation and code for full transparency and reproducibility.

Performance Metrics: Reports RMSE, MAE, R², confusion matrices, and classification reports.

Dataset
Source: UCI Machine Learning Repository – AI4I 2020 Predictive Maintenance Dataset

Description: Contains 10,000+ records of simulated sensor data, machine conditions, and labeled failure types.


How to Use
Clone this repository.

Open the Jupyter notebooks in sequence:

step1.ipynb for data exploration and preprocessing

multi model classifier.ipynb for multi-label classification

Other notebooks for specific failure type analysis

Install required libraries:

nginx
Copy
Edit
pip install pandas scikit-learn matplotlib joblib
Run the cells to train and evaluate models.

Use the saved machine_failure_model.pkl to make predictions on new data.

Key Results
Achieved robust classification accuracy for general and sub-failure modes.

Demonstrated how predictive maintenance can reduce unplanned downtime and optimize servicing schedules.


model = load('machine_failure_model.pkl')
X_new = ... # your new data here
prediction = model.predict(X_new)
License
This repository is for educational and demonstration purposes.
Data source: UCI ML Repository (see above).

Confusion Matrix:
![image](https://github.com/user-attachments/assets/e7a63b77-ad6f-4ca3-aa52-8ed65bc407ab)


Acknowledgments
Dataset: UCI ML Repository, AI4I 2020 Predictive Maintenance

Project author: Shaiprashaanth
