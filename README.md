# 🏥 Patient Readmission Prediction System

## 📌 Project Overview

This project predicts whether a patient is likely to be **readmitted to the hospital** after treatment using Machine Learning.

It helps hospitals:

* Identify high-risk patients
* Improve patient care
* Reduce unnecessary readmissions
* Optimize hospital resources

---

## 🎯 Problem Statement

Hospital readmissions increase costs and indicate potential gaps in patient care.
This project builds a predictive model to **classify patients into high-risk and low-risk categories**.

---

## 🛠️ Tech Stack

* **Python** (Data Processing & ML)
* **Pandas, NumPy** (Data Handling)
* **Scikit-learn** (Machine Learning)
* **Matplotlib, Seaborn** (Visualization)
* **MySQL** (Data Storage)
* **Power BI** (Dashboard & Insights)

---

## 📂 Project Structure

```
patient-readmission-prediction/
│
├── data/
│   └── hospital_data.csv
│
├── notebook/
│   └── model.ipynb
│
├── output/
│   └── plots.png
│
└── README.md
```

---

## 🔄 Project Workflow

```
Data Collection → Data Cleaning → Feature Engineering → Encoding
→ Train/Test Split → Model Training → Evaluation → Prediction
```

---

## 🧹 Data Preprocessing

* Handled missing values using mean/mode
* Cleaned categorical values (e.g., Yes/No formatting)
* Converted categorical data into numerical format using encoding

---

## ⚙️ Feature Engineering

* Created **Age_Group** (Young, Adult, Senior)
* Created **High_Cost** flag
* Created **Stay_Type** (Short, Medium, Long)
* Converted target variable (**Readmission → 0/1**)

---

## 🤖 Machine Learning Models

* Logistic Regression
* Random Forest Classifier

---

## 📊 Model Performance

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | 92.89%   |
| Random Forest       | 98.48%   |

### 🔁 Cross Validation Accuracy

**98.37%**

---

## 📉 Confusion Matrix (Random Forest)

```
[[143   1]
 [  2  51]]
```

* Very few misclassifications
* High precision and recall

---

## 📈 Key Insights

* **Age** is the most important factor
* High **treatment cost** indicates higher risk
* **Heart-related conditions** increase readmission probability
* Longer hospital stays increase risk

---

## 🚀 How to Run the Project

### 1️⃣ Clone Repository

```
git clone https://github.com/your-username/patient-readmission-prediction.git
cd patient-readmission-prediction
```

### 2️⃣ Install Requirements

```
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 3️⃣ Run Notebook

Open:

```
notebook/model.ipynb
```

---

## 🔮 Making Predictions

Example:

```python
prediction = model.predict(new_patient)
```

Output:

* `0` → Low Risk
* `1` → High Risk

---

## 💾 Model Saving

```python
import joblib
joblib.dump(model, "model.pkl")
```

---

## 🧠 Business Impact

* Helps hospitals take **preventive actions**
* Improves patient outcomes
* Reduces healthcare costs

---

## 🔥 Key Learnings

* Data Cleaning & Preprocessing
* Feature Engineering
* Handling Data Leakage
* Model Evaluation Techniques
* Cross Validation
* Real-world ML application

---

## 📌 Future Improvements

* Deploy using Streamlit (Web App)
* Integrate with hospital database
* Real-time prediction system
* Advanced models (XGBoost)

---

## 👨‍💻 Author

Vitthal Desai

---

## ⭐ If you like this project

Give it a ⭐ on GitHub!
