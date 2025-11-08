# 🧠 IEEE-CIS Fraud Detection

**Predicting fraudulent online transactions using advanced machine learning models.**  
This project explores and compares multiple ensemble and boosting algorithms on the IEEE-CIS Fraud Detection dataset to identify high-risk fraudulent activities with high precision and recall.

---

## 📋 Project Overview

Online fraud detection is a critical problem faced by financial institutions and e-commerce platforms.  
This project focuses on developing, tuning, and evaluating machine learning models that classify transactions as fraudulent or legitimate based on anonymized transaction features.

The workflow includes:
- Exploratory Data Analysis (EDA)
- Feature Engineering & Preprocessing
- Model Training (Logistic Regression, Random Forest, XGBoost, LightGBM)
- Cross-Validation & Hyperparameter Tuning
- Evaluation on Validation Set
- Model Interpretation (Feature Importance & ROC Curves)

---

## ⚙️ Tech Stack

- **Language:** Python 3.10  
- **Frameworks & Libraries:**  
  `pandas`, `numpy`, `scikit-learn`, `xgboost`, `lightgbm`, `matplotlib`, `seaborn`, `imbalanced-learn`  
- **Environment:** Jupyter Notebook  

---

## 🚀 How to Run

1️⃣ **Clone this repository**

git clone https://github.com/<your-username>/IEEE-Fraud-Detection.git
cd IEEE-Fraud-Detection
2️⃣ **Install dependencies**

pip install -r requirements.txt

3️⃣ **Run the notebook**

jupyter notebook IEEE_Fraud_Detection.ipynb

Execute all cells to preprocess data, train models, and view performance results. 

## 📊 Model Performance Summary

| Model                | Validation ROC-AUC | CV ROC-AUC |
|-----------------------|--------------------|-------------|
| Logistic Regression   | 0.8636             | 0.8560      |
| Random Forest         | 0.8665             | 0.8662      |
| XGBoost               | 0.9277             | 0.9172      |
| LightGBM              | **0.9283**         | **0.9162**  |

🏅 **Best Model:** Tuned **XGBoost**  
✅ **Final Validation ROC-AUC:** **0.9408**
## 🧩 XGBoost Classification Report

| **Metric**   | **Class 0** | **Class 1** |
|:-------------:|:-----------:|:-----------:|
| **Precision** | 0.99        | 0.50        |
| **Recall**    | 0.97        | 0.71        |
| **F1-Score**  | 0.98        | 0.59        |

**Overall Performance**

- **Accuracy:** 0.97  
- **Macro Avg F1:** 0.79  

🧠 The XGBoost model achieved a strong balance between **recall** (ability to catch frauds) and **precision** (minimizing false positives), outperforming other models on both validation and cross-validation metrics.

---

## 📈 Key Insights

- Ensemble and boosting methods (**XGBoost**, **LightGBM**) outperform linear and bagging models.  
- Feature scaling, one-hot encoding, and handling missing values significantly improved model stability.  
- Precision-recall tradeoff was carefully optimized to minimize financial loss due to undetected fraud.  
- Model explainability was ensured via **feature importance visualization**.

---

## 📚 Future Improvements

- Integrate **SMOTE** or **ADASYN** for advanced class balancing.  
- Deploy the trained model using **FastAPI** or **Streamlit**.  
- Add **SHAP/LIME** analysis for interpretability.  
- Optimize inference pipeline for **real-time fraud scoring**.

---

## 👨‍💻 Author

**Jasveen Singh Sahani**  
🎓 Computer Science Student @ York University  
📍 Toronto, Canada  
🔗 [LinkedIn](https://www.linkedin.com/in/jasveen-singh-sahani-92716b249/) • [GitHub](https://github.com/jsahani9)
