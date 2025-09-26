# Customer Churn Prediction

A machine learning project to predict customer churn and expose predictions through a Flask REST API.  
This repo is being built step by step in **sprints**.  

Notebook-first workflow.
---

## 🚀 Project Overview
- **Goal:** Predict which customers are likely to churn.  
- **Models:** Logistic Regression, Random Forest.  
- **Deployment:** Flask REST API   
- **Dataset:** Kaggle "Churn Modelling" dataset → place in `data/raw/churn_modelling.csv`.  

## Project structure
- `src/api/app.py` → minimal Flask API with health check.
- `notebooks/` → Jupyter notebooks for training & EDA.
- `data/raw/` → put dataset here (ignored).
- `models/` → trained models saved here (ignored).
- `requirements.txt` → Python dependencies.

## Setup
1. Create venv  -
   python -m venv venv
   .\venv\Scripts\Activate.ps1
2. Install dependencies-
pip install -r requirements.txt
3. Start Jupyter-
jupyter notebook

