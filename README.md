# Credit Risk Prediction

This repository contains a credit risk analysis and prediction project using machine learning techniques.  
The goal is to predict the likelihood of loan default (credit risk) from customer and loan features.

**Models used:** XGBoost, CatBoost, Random Forest

## Project structure

credit-risk-prediction/
├── data/
│ └── credit_risk_dataset.csv
├── notebook/
│ └── Credit_Risk_final.ipynb # main Jupyter Notebook (analysis, modeling, evaluation)
└── README.md

## Summary

This project performs data preprocessing, exploratory data analysis (EDA), model training with XGBoost, CatBoost and Random Forest, and model evaluation using common classification metrics. The notebook contains the full workflow from raw data to model evaluation and feature importance analysis.


## Technologies & Libraries

- Python (pandas, numpy)
- Scikit-learn (preprocessing, metrics)
- XGBoost
- CatBoost
- Random Forest
- Matplotlib, Seaborn
- Jupyter Notebook

## Key steps in the notebook

1. Load dataset and inspect shape / missing values.  
2. Data cleaning and preprocessing (missing values, encoding categorical variables, scaling if needed).  
3. Exploratory Data Analysis (distributions, correlations, visualizations).  
4. Model training and hyperparameter tuning for: XGBoost, CatBoost, Random Forest.  
5. Evaluation: confusion matrix, Accuracy, Precision, Recall, F1-score, ROC-AUC.  
6. Feature importance analysis and interpretation.  

## Results (from the notebook outputs)
- Accuracy: **93.87%**  
- Precision: **94%**  
- Recall: **92%**  
- F1-score: **83.60%**  
- ROC-AUC: **0.95**

> If you want the README to list per-model metrics (e.g. XGBoost → accuracy 93%; CatBoost → accuracy 91%; ...), I can update it after extracting per-model outputs from the notebook.

## How to run locally

1. Clone the repo:
```bash
git clone https://github.com/your-username/credit-risk-prediction.git
cd credit-risk-prediction
Create a virtual environment and install dependencies:
python -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows

pip install pandas numpy scikit-learn matplotlib seaborn xgboost catboost jupyter
Put the dataset credit_risk_dataset.csv inside the data/ folder (already included if you upload it).

Open the notebook:
jupyter notebook notebook/Credit_Risk_final.ipynb
Run cells from top to bottom. 
