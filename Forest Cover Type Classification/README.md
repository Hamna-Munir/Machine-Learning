# 🌲 Forest Cover Type Classification using Random Forest

This project involves predicting forest cover types from cartographic variables using machine learning techniques. The dataset is provided by the U.S. Forest Service and contains data on 7 forest cover types based on 55 features.

## 📌 Project Objective
To build a classification model that can accurately predict the forest cover type using a Random Forest classifier.

---

## 📁 Dataset
- **Source**: UCI / Kaggle – Forest CoverType Dataset
- **Records**: 40,000+
- **Features**: 55 (Elevation, Aspect, Slope, Soil Type, Wilderness Area, etc.)
- **Target**: Cover_Type (1 to 7)

---

## 🧪 Technologies Used
- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Scikit-learn

---

## 📊 Steps Performed

### 1. Data Loading & Cleaning
- Loaded `covtype.data` and added column names
- Verified dataset structure and data types
- Checked for missing values

### 2. Exploratory Data Analysis (EDA)
- Summary statistics
- Feature distributions
- Correlation heatmaps

### 3. Model Building
- Split data into train/test sets
- Trained a Random Forest Classifier
- Evaluated with classification report and confusion matrix

### 4. Model Evaluation
- Accuracy Score
- Confusion Matrix
- Classification Report

---

## ✅ Results
The Random Forest Classifier achieved high performance in predicting cover types with balanced accuracy across all classes.

---

## 📎 Files Included
- `forest_cover_classification.ipynb`: Main notebook with all steps
- `covtype.data`: Dataset used in the project
- `README.md`: Project overview

---

## 📌 How to Run

```bash
# Clone this repository
git clone https://github.com/Hamna-Munir/Machine-Learning.git

# Navigate to the project folder
cd Machine-Learning/Forest_Cover_Type_Classification

# Open the Jupyter Notebook
jupyter notebook forest_cover_classification.ipynb
