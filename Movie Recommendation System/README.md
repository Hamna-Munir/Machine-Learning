# Loan Approval Prediction

## 📌 Project Overview
This project predicts whether a loan application will be approved or not based on various applicant details such as income, credit history, education, and loan amount.  
The model uses **Logistic Regression** to classify loan applications into approved or not approved categories.

## 📂 Dataset
- Dataset Name: **Loan-Approval-Prediction-Dataset**
- Source: [Kaggle - Loan Prediction Dataset](https://www.kaggle.com/datasets/ninzaami/loan-predication)
- Format: CSV (`loan_approval_dataset.csv`)
- Key Features:
  - `Gender`
  - `Married`
  - `Dependents`
  - `Education`
  - `Self_Employed`
  - `ApplicantIncome`
  - `CoapplicantIncome`
  - `LoanAmount`
  - `Loan_Amount_Term`
  - `Credit_History`
  - `Property_Area`
  - `Loan_Status` (Target Variable)

## ⚙️ Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## 🛠️ Steps Followed
1. **Data Loading**
   - Loaded CSV dataset using Pandas.
   
2. **Data Preprocessing**
   - Handled missing values.
   - Converted categorical values into numerical using Label Encoding.
   - Standardized numerical features for better model performance.

3. **Exploratory Data Analysis (EDA)**
   - Visualized data distributions and correlations using Seaborn and Matplotlib.
   - Checked relationships between features and the target variable.

4. **Model Building**
   - Used **Logistic Regression** classifier.
   - Split dataset into training (80%) and testing (20%).

5. **Model Evaluation**
   - Accuracy Score
   - Confusion Matrix
   - Classification Report

## 📊 Example Results
- **Accuracy:** ~82%
- **Precision, Recall, F1-score:** Detailed in the classification report.

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/loan-approval-prediction.git
Navigate to the project folder:

bash
Copy
Edit
cd loan-approval-prediction
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the Jupyter Notebook:

bash
Copy
Edit
jupyter notebook Loan_Approval_Prediction.ipynb
📌 Future Improvements
Try other classification models (Random Forest, XGBoost).

Implement hyperparameter tuning.

Deploy as a web application using Flask or Streamlit.

Author: Hamna Munir
Internship: Elevvo Pathways (Cairo, Egypt)
