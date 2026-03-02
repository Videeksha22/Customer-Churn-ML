# 📊 Customer Churn Prediction using Machine Learning

## 📌 Project Overview
This project focuses on predicting customer churn for a telecom company using supervised machine learning algorithms. The objective is to identify customers who are likely to leave the service so that the company can take proactive retention measures.

The project includes complete data preprocessing, model training, evaluation, and model serialization for future deployment.

---

## 📁 Dataset Information

- Dataset: Telco Customer Churn Dataset
- Records: ~7,000 customers
- Target Variable: `Churn`
- Features include:
  - Gender
  - SeniorCitizen
  - Partner
  - Dependents
  - Tenure
  - PhoneService
  - InternetService
  - Contract
  - PaymentMethod
  - MonthlyCharges
  - TotalCharges

---

## ⚙️ Project Workflow

### 1️⃣ Data Preprocessing
- Removed unnecessary columns
- Converted `TotalCharges` to numeric format
- Handled missing values
- Encoded categorical variables using **LabelEncoder**
- Split dataset into training and testing sets using `train_test_split`

---

### 2️⃣ Model Building

The following machine learning models were implemented and evaluated:

- Decision Tree Classifier
- Random Forest Classifier
- XGBoost Classifier

---

### 3️⃣ Model Evaluation

Models were evaluated using:

- Accuracy Score
- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)

This helped compare model performance and select the best performing algorithm.

---

### 4️⃣ Model Saving

The final trained model and encoders were saved using **Pickle**:

- `customer_churn_model.pkl`
- `encoders.pkl`

This allows the model to be reused without retraining.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib / Seaborn
- Pickle

---

## 📂 Project Structure

```
Customer-Churn-Prediction/
│
├── Cust_Churn_Pred.ipynb
│
├── models/
│ ├── customer_churn_model.pkl
│ └── encoders.pkl
│
├── WA_Fn-UseC_-Telco-Customer-Churn.csv
│
├── requirements.txt
└── README.md
```

---

## 🚀 Business Impact

Customer churn prediction helps telecom companies:

- Identify high-risk customers
- Reduce revenue loss
- Improve customer retention strategies
- Optimize marketing campaigns

---

## ▶️ How to Run the Project

1. Clone the repository:

```bash
git clone https://github.com/Videeksha22/customer-churn-ml.git
cd customer-churn-ml
```

2. Install requirements:

```bash
pip install -r requirements.txt
```

3. Open the notebook:

```bash
jupyter notebook Customer_Churn_Prediction.ipynb
```

4. Run all cells sequentially

---

## 📌 Key Learnings

* Importance of data cleaning and handling missing values in real-world datasets
* Encoding categorical variables for machine learning model compatibility
* Comparing multiple classification algorithms to select the best performing model
* Model serialization using Pickle for future deployment and reuse

---

## 🔮 Future Improvements

- Hyperparameter tuning (GridSearchCV)
- ROC-AUC evaluation
- Feature importance analysis
- SHAP explainability
- Deployment using Streamlit or Flask
