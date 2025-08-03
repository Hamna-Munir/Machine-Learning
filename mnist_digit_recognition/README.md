# 🧠 Project: MNIST Digit Recognition

This project involves building a machine learning model that can recognize and classify handwritten digits (0–9) using the MNIST dataset.

---

## 📂 Folder Structure

```
MNIST_Digit_Recognition/
├── mnist_digit_recognition.ipynb       # Jupyter Notebook with full code
├── model_mnist.h5                      # Trained Keras model file
├── requirements.txt                    # List of required Python packages
└── README.md                           # Project description and instructions
```

---

## 📊 Dataset

- **Name:** MNIST (Modified National Institute of Standards and Technology)
- **Size:** 70,000 images (60,000 train + 10,000 test)
- **Image Format:** 28x28 grayscale images of digits from 0–9
- **Source:** Automatically loaded via TensorFlow/Keras — no need to download manually

---

## 🛠️ Requirements

To run this project, install the necessary Python packages using the following command:

```bash
pip install -r requirements.txt
```

**requirements.txt**

```
tensorflow
matplotlib
numpy
seaborn
```

---

## 🚀 How to Run

1. Open the `mnist_digit_recognition.ipynb` file in Jupyter Notebook, VS Code, or Google Colab.
2. Run the notebook cell by cell.
3. The model will train and evaluate using the MNIST dataset.
4. The trained model is saved as `model_mnist.h5`.

---

## 🧠 Model Overview

- **Architecture:**
  - Flatten Layer (28x28 input)
  - Dense Layer (128 units, ReLU)
  - Dense Layer (64 units, ReLU)
  - Output Layer (10 units, Softmax)
- **Loss Function:** Categorical Crossentropy
- **Optimizer:** Adam
- **Metrics:** Accuracy

---

## 📈 Results

- Achieved accuracy of \~98% on test dataset
- Includes visualizations for:
  - Sample images
  - Loss and accuracy graphs
  - Confusion matrix

---

## 📬 Output Files

- `model_mnist.h5`: Trained model
- Predictions displayed within the notebook

---

## 📌 Notes

- No external dataset download required — MNIST loads directly using Keras.
- Designed for educational and demonstration purposes.

---

## 📜 License

Free for personal and academic use.

---

✅ **Author:** Hamna Munir\
🎯 **Task 2 - Arch Technologies AI/ML Internship**

