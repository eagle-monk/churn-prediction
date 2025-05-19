# Churn Prediction using Google Colab

This project uses machine learning models to predict customer churn using a dataset from Kaggle. The entire workflow is implemented in a Google Colab notebook.

---

##  Overview

- Tool: Google Colab (Python)
- ML Algorithms: Random Forest Classifier, etc.
- Purpose: Predict which customers are likely to leave the company

---

##  Dataset

Source: [Kaggle - Telco Customer Churn](https://www.kaggle.com/blastchar/telco-customer-churn)

Dataset includes customer interest, account info, churn label and other details.

*Note: Dataset not uploaded due to size. Download it from Kaggle directly.*

---

## Model Performance
The model was trained to predict customer churn using a classification algorithm. Below are the performance metrics evaluated on the test set:

#### Overall Accuracy: 77.86%

#### Confusion Matrix:
[[878 158]
 [154 219]]
True Negatives (No Churn predicted correctly): 878

False Positives (Predicted Churn but actually No Churn): 158

False Negatives (Predicted No Churn but actually Churn): 154

True Positives (Churn predicted correctly): 219

#### Classification Report:

Metric	Class 0 (No Churn)	Class 1 (Churn)
Precision	0.85	0.58
Recall	0.85	0.59
F1-score	0.85	0.58
Support	1036	373

#### Averages:
Macro Avg F1-score: 0.72
Weighted Avg F1-score: 0.78

#### Observations:
The model performs well on non-churn customers (majority class).

Performance on churn prediction (minority class) is modest — consider:

Using techniques like SMOTE or class weighting

Exploring additional features or different model architectures

---

##  How to Run

1. Open the notebook in Google Colab:  
   [Open in Colab](https://colab.research.google.com/github/your-username/churn-prediction/blob/main/notebooks/churn_model.ipynb)

2. Follow the instructions in the notebook

---

## 📦 Requirements

Install packages via:

```bash
pip install -r requirements.txt
