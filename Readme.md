# 📱 Spam SMS Detection

This project implements a **Spam SMS Classifier** using machine learning models in Python.  
It uses the **SMS Spam Collection Dataset** to classify text messages as either **ham (not spam)** or **spam**.

---

## 📂 Dataset

- Dataset: [SMS Spam Dataset](https://drive.google.com/file/d/1A2ySkoOIaAdSA_Bx-QX6BV2RBK-XamgX/view?usp=drive_link)  
- Format: CSV file with two main columns:
  - `v1`: Label (`ham` or `spam`)
  - `v2`: SMS message text

---

## ⚙️ Features

- Preprocessing:
  - Keeps only required columns (`label`, `message`)
  - Converts labels into binary form (`ham → 0`, `spam → 1`)
- Train/test split (**80% training / 20% testing**)
- Feature extraction using **TF-IDF Vectorization**
- Models implemented:
  - ✅ Naive Bayes (MultinomialNB)
  - (Code also imports Logistic Regression & SVM — can be extended easily)
- Evaluation:
  - Accuracy score
  - Confusion matrix
  - Classification report (precision, recall, f1-score)

---

## 📦 Dependencies

Install the required Python libraries before running the notebook:

```bash
pip install pandas numpy scikit-learn
