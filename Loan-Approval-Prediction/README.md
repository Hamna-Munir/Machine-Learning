# 🏦 Loan Approval Prediction

A machine learning project to predict whether a loan application will be approved based on applicant data. This project uses classification models and handles imbalanced data using SMOTE.

---

## 📂 Files in this Repository

| File Name                           | Description                                      |
|------------------------------------|--------------------------------------------------|
| `Loan_Approval_Prediction_Notebook.ipynb` | Jupyter Notebook with code, charts, and results |
| `Loan-Approval-Prediction.csv`     | Dataset used (from Kaggle - do not upload if private) |
| `README.md`                        | Project documentation                           |

---

## 📊 Problem Statement

Use applicant data to predict whether their loan will be approved (`Loan_Status`). The dataset includes both categorical and numerical features and contains missing values and class imbalance.

---

## 🧰 Tools & Libraries

- Python
- Pandas, NumPy
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Matplotlib, Seaborn

---

## 🧠 Models Used

- Logistic Regression
- Decision Tree Classifier

---

## 📌 Key Steps

1. Data Cleaning (Missing Values)
2. Categorical Encoding
3. Feature Correlation Analysis (Heatmap)
4. Class Imbalance Handling using **SMOTE**
5. Model Training: Logistic Regression vs Decision Tree
6. Evaluation Metrics: **Precision**, **Recall**, **F1-Score**
7. Confusion Matrix Heatmaps
8. Class Distribution Visualization

---

## 📷 Visual Outputs

- 📊 Class distribution before and after SMOTE
- 📈 Feature correlation heatmap
- 🔲 Confusion matrices for both models

---

## 📥 Dataset Source

**Kaggle Dataset:**  
[Loan Prediction Dataset](https://www.kaggle.com/datasets/altruistdelhite04/loan-prediction-problem-dataset)  
📁 File used: `train.csv` (renamed as `Loan-Approval-Prediction.csv`)

---

## ✅ Conclusion

- SMOTE significantly improved the performance on the minority class.
- Decision Tree provided more flexible results but Logistic Regression was more interpretable.
- Both models are useful depending on the business requirement (e.g., high recall vs precision).

---

## 🙋‍♀️ Author

**Hamna Munir**  
Machine Learning Intern  
GitHub: [@Hamna-Munir](https://github.com/Hamna-Munir)

---

## 📜 License

This project is for educational purposes only.
