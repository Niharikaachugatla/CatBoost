# 🫀 CatBoost Classifier for Heart Disease Prediction

A comprehensive machine learning pipeline using **CatBoost** to predict heart disease from structured clinical data. This project demonstrates end-to-end modeling including preprocessing, training, evaluation, and interpretability — all aligned with best practices and academic standards.

---

## 📌 Project Overview

Heart disease remains one of the most common causes of mortality globally. In this project, we leverage **CatBoost**, a powerful gradient boosting library, to classify whether a patient is likely to have heart disease based on clinical and demographic attributes.

CatBoost is particularly well-suited for this task due to its **native handling of categorical features**, **robust performance**, and **interpretable output**.

---

## 🧠 What You'll Learn

- How to preprocess a real-world medical dataset  
- The strengths of CatBoost for tabular data  
- How to evaluate a classification model using:
  - Classification report
  - Confusion matrix
  - ROC curve (AUC)
- How to interpret model decisions using:
  - Feature importance
  - Partial dependence plots  

---

## 📂 Dataset Overview

- **Source:** [Cleveland Heart Disease dataset](https://www.kaggle.com/datasets/cherngs/heart-disease-cleveland-uci)  
- **Total samples:** ~1,000 (717 train / 308 test after split)  
- **Target variable:** `target`  
  - `0` = No heart disease  
  - `1` = Presence of heart disease  

---

## ⚙️ Features Used

| Feature      | Description                                  |
|--------------|----------------------------------------------|
| age          | Age in years                                 |
| sex          | 1 = male, 0 = female                         |
| cp           | Chest pain type (categorical)               |
| trestbps     | Resting blood pressure (mm Hg)              |
| chol         | Serum cholesterol (mg/dl)                   |
| fbs          | Fasting blood sugar (>120 mg/dl)            |
| restecg      | Resting ECG results (categorical)           |
| thalach      | Maximum heart rate achieved                 |
| exang        | Exercise-induced angina                     |
| oldpeak      | ST depression induced by exercise           |
| slope        | Slope of the peak ST segment (categorical) |
| ca           | Number of major vessels (0–4)               |
| thal         | Thalassemia status (categorical)           |

---

## 🧪 Results

- ✅ **Accuracy:** 99%
- ✅ **Precision & Recall:** Balanced (F1 = 0.99 for both classes)
- ✅ **ROC AUC:** 1.00
- ✅ **False Negatives:** Only 3 (out of 308 test samples)

---

## 📊 Visualizations Included

- Confusion Matrix (`flare` colormap)
- ROC Curve (AUC = 1.00)
- Feature Importance (via CatBoost)
- Partial Dependence Plot (e.g., age → target)

---

## 🛠️ How to Run

```bash
# Clone the repository
git clone https://github.com/Niharikaachugatla/CatBoost.git
cd CatBoost-HeartDisease

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook notebooks/heart_disease_catboost.ipynb
