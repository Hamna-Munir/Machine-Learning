# 🧠 Student Score Prediction using Regression

This project is part of my Machine Learning Internship with **Elevvo**. The goal is to predict students' final exam scores based on the number of study hours using **Linear Regression** and **Polynomial Regression**.

---

## 📊 Dataset

- Source: [Student Performance Dataset (Kaggle)](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)
- Simulated column: `study_hours` (normally distributed between 1 and 10 hours)
- Final score: Calculated as the average of Math, Reading, and Writing scores.

---

## 💼 Objectives

- Perform data cleaning and basic visualization
- Train a Linear Regression model to predict final exam scores
- Evaluate model performance using MSE and R²
- Visualize predictions and model fitting
- (Bonus) Train a Polynomial Regression model and compare performance

---

## 🔧 Technologies Used

| Tool/Library      | Purpose                              |
|------------------|--------------------------------------|
| `Python`          | Programming Language                 |
| `Pandas`          | Data Manipulation                    |
| `Seaborn` & `Matplotlib` | Data Visualization             |
| `Scikit-learn`    | Regression Modeling and Evaluation   |
| `Jupyter / Google Colab` | Notebook Environment           |

---

## 🚀 Model Workflow

1. Load and preprocess the dataset
2. Simulate `study_hours` data
3. Calculate `final_score`
4. Split data into training and test sets
5. Train Linear Regression Model
6. Evaluate using MSE and R²
7. Train Polynomial Regression Model
8. Compare both models

---

## 📈 Results

| Model                | Mean Squared Error | R² Score |
|---------------------|--------------------|----------|
| Linear Regression    | *e.g., 140.25*     | *0.68*   |
| Polynomial Regression| *e.g., 128.30*     | *0.72*   |

> *Note: Your actual values may vary depending on the simulation.*

---

## 📂 File Structure
├── StudentsPerformance.csv # Cleaned dataset with study hours & final score                                                                      
├── Student Score Prediction.ipynb # Complete notebook (Google Colab compatible)

├── README.md # Project documentation


## 📣 Credits

This project was completed as part of the **ML Internship Program by [Elevvo](https://www.linkedin.com/company/elevvo/)**.

---

## 📌 Tags

`#MachineLearning` `#Python` `#DataScience` `#LinearRegression` `#AIInternship` `#Elevvo`
