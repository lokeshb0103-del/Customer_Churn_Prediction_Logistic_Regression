# Customer Churn Prediction Using Machine Learning

## 📌 Project Overview
This project predicts whether a customer is likely to leave a telecommunications company using **Logistic Regression**, a supervised machine learning algorithm. The project covers data cleaning, preprocessing, categorical encoding, model training, and performance evaluation.

## 🎯 Objectives
- Analyze customer data to understand churn patterns.
- Clean and preprocess the dataset.
- Build a Logistic Regression classification model.
- Evaluate the model using accuracy, precision, recall, F1-score, and a confusion matrix.

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab

## 📂 Dataset
The project uses the **Telco Customer Churn** dataset, which contains customer demographics, service details, account information, and churn status.

- **Dataset source:** Kaggle
- **Dataset link:** https://www.kaggle.com/datasets/blastchar/telco-customer-churn
- **Original dataset size:** 7,043 rows and 21 columns
- **Rows after cleaning:** 7,032

### Dataset Preprocessing
1. Inspected the dataset using Pandas.
2. Checked for missing values and duplicate records.
3. Converted `TotalCharges` from text to numeric format.
4. Removed 11 rows with missing `TotalCharges`.
5. Separated input features (`X`) and target label (`y`).
6. Applied One-Hot Encoding to categorical input features.
7. Split the data into 80% training data and 20% testing data.

## 🤖 Model
**Algorithm:** Logistic Regression

The model was trained using Scikit-learn and evaluated on the test dataset.

## 📊 Model Performance

| Metric | No Churn | Churn |
|---|---:|---:|
| Precision | 0.85 | 0.65 |
| Recall | 0.89 | 0.57 |
| F1-score | 0.87 | 0.61 |
| Support | 1,033 | 374 |

**Overall Accuracy: 80.31%**

### Key Findings
- The model achieved 80.31% accuracy on the test dataset.
- It identifies customers who stay more effectively than customers who churn.
- Churn recall is 57%, meaning the model identifies 57% of actual churn cases.
- Future improvements could focus on increasing churn recall and comparing other classification algorithms.

## 📈 Confusion Matrix
The confusion matrix summarizes correct and incorrect predictions:

| Actual / Predicted | No | Yes |
|---|---:|---:|
| No | 916 | 117 |
| Yes | 160 | 214 |

## 🚀 How to Run
1. Clone or download this repository.
2. Open the Jupyter Notebook (`.ipyn
