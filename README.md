# Customer Churn Analysis & Prediction

## Overview
End-to-end customer churn prediction project to identify customers at high risk of leaving and uncover key churn drivers using Python.

### Objective
- Build a predictive model to classify customers as high or low churn risk
- Perform comprehensive Exploratory Data Analysis (EDA)
- Identify the most important factors driving customer churn
- Provide actionable business insights for customer retention

## Tech Stack
- **Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **Tools**: Jupyter Notebook

## Dataset
- Source: [Hugging Face - d0r1h/customer_churn](https://huggingface.co/datasets/d0r1h/customer_churn)
- **Size**: 36,992 records
- Features include: age, membership category, feedback, points in wallet, transaction value, complaints, etc.

## Project Structure

customer-churn-analysis/
├── Customer_Churn_Analysis.ipynb
├── cleaned_customer_churn.csv
├── requirements.txt
├── README.md
├── insights/
│   ├── churn_distribution.png
│   ├── membership_vs_churn.png
│   ├── feature_importance.png
│   ├── feedback_vs_churn.png
│   └── key_insights.md
└── data/
└── cleaned_customer_churn.csv


## Key Steps Performed
1. Data Loading & Cleaning (handled missing values, invalid entries like `?`, `Error`, `-999`)
2. Exploratory Data Analysis (EDA)
3. Feature Engineering & Encoding
4. Model Building using **Random Forest Classifier**
5. Model Evaluation
6. Feature Importance Analysis

## Model Performance

| Metric       | Score      |
|--------------|------------|
| **Accuracy** | **92.69%** |
| **Precision**| 92.30%     |
| **Recall**   | **94.43%** |
| **F1 Score** | **93.35%** |

### Classification Report

precision    recall  f1-score   support
0       0.93      0.91      0.92      3377
1       0.92      0.94      0.93      4022

accuracy                           0.93      7399

macro avg       0.93      0.93      0.93      7399

weighted avg       0.93      0.93      0.93      7399


### Confusion Matrix

[[3060  317]
[ 224 3798]]

- True Negatives: 3060  
- False Positives: 317  
- False Negatives: 224  
- True Positives: 3798

## Key Insights
- Customers with **No Membership** or **Basic Membership** have significantly higher churn risk.
- **Low points in wallet** and **high days since last login** are strong indicators of churn.
- Negative feedback categories ("Poor Customer Service", "Poor Website", "Too many ads") are highly correlated with churn.
- Platinum and Gold membership customers show much higher loyalty.
- The model achieved excellent recall (94.43%), meaning it is very good at identifying customers who are likely to churn.

## Actionable Recommendations
1. Target **Basic/No Membership** customers with upgrade offers and loyalty programs.
2. Run re-engagement campaigns for customers with low wallet points and long inactivity periods.
3. Address common complaints related to customer service and website experience.
4. Use the model to prioritize retention efforts on high-risk customers.

## How to Run the Project
```bash
# Clone the repository
git clone https://github.com/geethalakshmi579/customer-churn-analysis.git

# Navigate to project folder
cd customer-churn-analysis

# Install required packages
pip install -r requirements.txt

# Open Jupyter Notebook
jupyter notebook
