# Customer Churn Prediction

A machine learning project to predict customer churn and expose predictions through a Flask REST API.  


Notebook-first workflow. All training, EDA, and evaluation are done inside Jupyter notebooks (`notebooks/train.ipynb`).  

---

## 🚀 Project Overview
- **Goal:** Predict which customers are likely to churn.  
- **Models:** Logistic Regression, Random Forest.  
- **Deployment:** Flask REST API (with `/predict` endpoint coming in Sprint 3).  
- **Dataset:** Kaggle ["Churn Modelling"](https://www.kaggle.com/datasets/shrutimechlearn/churn-modelling) dataset → place in `data/raw/churn_modelling.csv`.  

---

## 📂 Project structure
Customer-Churn-Prediction/
├─ .gitignore
├─ README.md
├─ requirements.txt
├─ data/
│ └─ raw/ # place dataset here (ignored in git)
├─ models/ # trained models (ignored in git)
├─ notebooks/
│ └─ train.ipynb # training notebook (EDA + model training)
└─ src/
└─ api/
└─ app.py # Flask API with health check

## Setup
1. Create venv  -
   python -m venv venv
   .\venv\Scripts\Activate.ps1
2. Install dependencies-
pip install -r requirements.txt
3. Start Jupyter-
jupyter notebook

# Notebook Workflow 

Dataset check (verify file exists in data/raw/)

Load dataset and basic EDA (shape, head, summary)

Feature prep: drop ID cols, split into X, y

Preprocessing pipeline (numeric → impute+scale, categorical → impute+one-hot)

Train/test split

Baseline model (DummyClassifier)

Logistic Regression: train + evaluate

Random Forest: train + evaluate, compare metrics

Save best model → models/best_model.joblib

Save feature list → models/feature_columns.txt

