# 🛳️ Titanic Survival Prediction — Binary Classification

This project explores **Machine Learning classification techniques** on the [Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic) dataset from Kaggle.  
It’s part of my journey to fully master **Machine Learning** before moving into **Deep Learning**.

---

## 📘 Project Overview

The goal is to predict **whether a passenger survived or not** during the Titanic disaster based on demographic, social, and ticket-related information.

This project is built in a single, complete notebook:

| Notebook | Description |
|-----------|--------------|
| 📓 `titanic_binary_classification.ipynb` | Full end-to-end pipeline: data cleaning, feature engineering, encoding, balancing, model training, and evaluation. |

---

## ⚙️ Technologies Used

- **Python 3.x**
- **NumPy**, **Pandas** → data manipulation  
- **Matplotlib**, **Seaborn** → visualization  
- **Scikit-Learn** → classification, preprocessing, evaluation  
- **Imbalanced-learn (SMOTE)** → class balancing  

---

## 🧩 Data Preprocessing Pipeline

1. **Handle missing values** in `Age`, `Fare`, `Embarked`, etc.  
2. **Feature Engineering**:  
   - Extracted `Title` from passenger names  
   - Grouped rare titles  
   - Encoded `Sex` (male → 0, female → 1)  
3. **Encoding**:  
   - One-Hot Encoding for categorical features (`Embarked`, `Title`)  
4. **Balancing**:  
   - Applied **SMOTE** to balance the “Survived” and “Died” classes  
5. **Scaling**:  
   - Standardized continuous features (`Age`, `Fare`) using `StandardScaler`  
6. **Model**:  
   - Trained a **Logistic Regression** classifier  
7. **Evaluation**:  
   - Accuracy, F1-score, Cross-Validation, Confusion Matrix, Classification Report, ROC Curve  

---

## 📊 Model Results

| Metric | Score |
|--------|--------|
| **Accuracy** | 0.8101 |
| **F1 Score** | 0.7875 |
| **Cross-Validation Mean** | 0.8255 |
| **ROC-AUC** | 0.87 |

### 🧠 Confusion Matrix

[[82 23]
[11 63]]

| Class | Precision | Recall | F1-Score | Support |
|--------|------------|--------|-----------|----------|
| **0.0 (Died)** | 0.88 | 0.78 | 0.83 | 105 |
| **1.0 (Survived)** | 0.73 | 0.85 | 0.79 | 74 |
| **Accuracy** | - | - | **0.81** | 179 |

---

## 🚀 Next Steps

- Experiment with **Decision Tree**, **Random Forest**, and **SVM** models  
- Perform **hyperparameter tuning** using `GridSearchCV`  
- Deploy using **Streamlit** for an interactive web interface  

---

## 🧾 Repository Structure

ML-Titanic-Survival-Classification/
│
├── data/
│   ├── train.csv
│   ├── test.csv
│
├── notebooks/
│   ├── titanic_classification.ipynb
│
├── requirements.txt
├── README.md
└── .gitignore

---

## 🧩 How to Run

```bash
git clone https://github.com/Ramy-Bahi/Titanic-Survival-Classification.git
cd Titanic-Survival-Classification
pip install -r requirements.txt
jupyter notebook notebooks/titanic_binary_classification.ipynb
```

---

## 📊 Dataset

Available on Kaggle: [Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic)

---

## 👨‍💻 Author

**Rami Bahi**

🎓 Master’s Student in Artificial Intelligence

💻 Passionate about Machine Learning, Deep Learning & Web Development

---

## ⭐ If you like this project...

Give it a star ⭐ on GitHub to support my work and journey!
