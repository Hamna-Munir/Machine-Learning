# 📧 Email Spam Classification using Machine Learning

This project is a simple and effective spam detection system using a logistic regression model trained on SMS messages. It classifies messages as **Spam** or **Ham (Not Spam)** using TF-IDF features.

## 📁 Folder Structure

```
Email-Spam-Classification-ML/
│
├── spam.csv
├── Task1_Email_Spam_Classification.ipynb
├── spam_classifier.pkl
├── tfidf_vectorizer.pkl
├── requirements.txt
└── README.md
```

## 📊 Dataset

- Dataset: [SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)
- Total Samples: 5,574
- Labels: `spam`, `ham`

## 💡 ML Pipeline

- **Vectorization**: TF-IDF (sklearn)
- **Model**: Logistic Regression
- **Libraries Used**:
  - pandas
  - numpy
  - scikit-learn

## 🧪 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/Email-Spam-Classification-ML.git
   cd Email-Spam-Classification-ML
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:
   ```bash
   jupyter notebook Task1_Email_Spam_Classification.ipynb
   ```

4. Inspect the accuracy, confusion matrix, and saved model files.

## ✅ Output

- Accuracy: ~97%
- Vectorizer and model saved as `.pkl` for future use

## ✍️ Author

**Hamna Munir**  
AI/ML Intern at Arch Technologies
