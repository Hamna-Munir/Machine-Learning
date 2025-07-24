# 🛍️ Customer Segmentation Using K-Means & DBSCAN

This project is part of my AI/ML Internship with [Elevvo](https://www.linkedin.com/company/elevvo/) and focuses on customer segmentation using clustering techniques.

---

## 📌 Objective

To segment mall customers into different groups based on their **Annual Income** and **Spending Score** using:

- **K-Means Clustering**
- **DBSCAN Clustering**

This segmentation helps in understanding customer behavior, allowing businesses to design targeted marketing strategies.

---

## 📊 Dataset

- **Dataset Name:** Mall Customers
- **Source:** [Kaggle - Customer Segmentation Data](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial)
- **Features Used:**
  - Annual Income (k$)
  - Spending Score (1–100)

---

## ⚙️ Tools & Technologies

- Python 3.x
- Pandas & NumPy
- Scikit-learn (KMeans, DBSCAN, StandardScaler)
- Matplotlib & Seaborn
- Jupyter Notebook

---

## 🔍 Project Workflow

1. Load and explore the dataset
2. Select features (Income & Spending Score)
3. Scale features using `StandardScaler`
4. Use Elbow Method to determine optimal K
5. Apply K-Means Clustering
6. Visualize clusters in 2D
7. Analyze average income/spending per cluster
8. Apply DBSCAN clustering (Bonus)
9. Export clustered data to CSV

---

## 📁 File Descriptions

| File                        | Description                                         |
|-----------------------------|-----------------------------------------------------|
| `customer_segmentation.ipynb` | Jupyter Notebook with full clustering pipeline     |
| `mall_customers.csv`         | Original Dataset (if allowed by license)           |
| `clustered_customers.csv`    | Final dataset with assigned cluster labels         |
| `requirements.txt`           | Python libraries used in the project (optional)    |

---

## 📷 Cluster Output

> 📌 All visualizations (K-Means and DBSCAN clusters) are displayed inside the notebook output cells.

---

## 📈 Key Learnings

- Practical use of **unsupervised learning** (KMeans, DBSCAN)
- How scaling and feature selection affect clustering
- Understanding and visualizing clusters in 2D
- Exporting model results to a structured CSV for real-world use

---

## ✅ Task Completed As Part Of

**Machine Learning Internship – Task 2: Customer Segmentation**  
✨ *Thanks to Elevvo for the learning opportunity and hands-on experience!*




