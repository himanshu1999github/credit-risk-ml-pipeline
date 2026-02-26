# Credit Risk Classification ML Pipeline

## 📌 Project Overview
This project builds an end-to-end machine learning pipeline to predict credit default risk for a digital lending platform. The aim is to automate credit assessment while maintaining strong predictive performance and interpretability.

---

## 🎯 Business Objective
- Identify potential loan defaulters accurately  
- Reduce financial losses due to defaults  
- Enable real-time loan decision-making (<1 second)  
- Maintain regulatory interpretability  

---

## 📊 Dataset Information
Dataset: German Credit Risk Dataset  

Contains 1000 credit applications with features such as:

- Age, Sex, Job category  
- Housing status  
- Saving & Checking account balance  
- Credit amount and duration  
- Loan purpose  

Target variable:
- 0 → Good Credit Risk  
- 1 → Bad Credit Risk (Default)

---

## 🔬 Machine Learning Pipeline

### 1️⃣ Data Preprocessing
- Missing value handling  
- Categorical encoding  
- Feature scaling  
- Train-test split (80/20)

### 2️⃣ Feature Engineering
Created additional features:

- Credit-to-duration ratio  
- Age group categorization  
- Account stability indicator  

---

## 🤖 Models Implemented
- Logistic Regression  
- Decision Tree  
- Random Forest  
- XGBoost  

Hyperparameter tuning performed on Random Forest.

---

## 🏆 Final Model Performance
**Tuned Random Forest Model:**

- Accuracy: ~86.5%  
- Recall (Default detection): ~80%  
- F1 Score: ~82.6%  
- AUC Score: ~0.92  

This meets the business requirement of at least 75% recall.

---

## 🔎 Model Evaluation Techniques
- Confusion Matrix  
- ROC Curve and AUC Score  
- Precision-Recall Curve  
- Feature Importance Analysis  

---

## 📈 Experiment Tracking
MLflow was used to:

- Track model parameters  
- Log evaluation metrics  
- Store trained models  

---

## 📁 Project Structure

│
├── data/
├── notebooks/
├── models/
│ └── tuned_random_forest.pkl
├── mlruns/
├── reports/
│ └── technical_report.pdf
├── requirements.txt
└── README.md

---

## 🚀 Deployment Considerations
The model can be deployed using Flask or FastAPI as a REST API and hosted on cloud platforms such as AWS, Azure, or GCP.

Monitoring should include:

- Prediction latency  
- Model accuracy & recall  
- Data drift detection  
- Periodic retraining strategy  

---

## 📦 Requirements
See `requirements.txt` for all dependencies.

---

## 👨‍💻 Author
**Himanshu Dhase**

---

## 📌 Conclusion
The project successfully demonstrates how machine learning can automate credit risk assessment, improve consistency, and reduce financial risk in digital lending environments.
