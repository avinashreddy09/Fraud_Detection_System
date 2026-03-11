# Fraud_Detection_System
# Credit Card Fraud Detection System


A simple yet powerful **real-time credit card fraud detection** web app built with **Streamlit** and **LightGBM**.  
It predicts whether a transaction is fraudulent using anonymized features (inspired by the classic Kaggle Credit Card Fraud dataset).

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Streamlit-1.x-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" alt="Streamlit" />
  <img src="https://img.shields.io/badge/LightGBM-4.x-1E90FF?style=for-the-badge" alt="LightGBM" />
  <img src="https://img.shields.io/badge/scikit--learn-1.6%2B-orange?style=for-the-badge" alt="scikit-learn" />
  <img src="https://img.shields.io/github/license/avinashreddy09/Fraud_Detection_System?style=for-the-badge" alt="License: MIT" />
</p>

## ✨ Key Features

- Upload CSV files with transaction data (V1–V28 PCA features + Time + Amount)
- Manual input mode for single transaction testing
- Real-time fraud probability score
- Geospatial distance calculation using **geopy** (customer ↔ merchant location)
- Trained **LightGBM** model (fast & high performance on imbalanced data)
- Clean, responsive Streamlit dashboard

## Demo (Add Your Own)

(Record a short 10–20s screen capture with ShareX / Loom → upload as GIF/MP4 to repo)

https://github.com/avinashreddy09/Fraud_Detection_System/assets/

## Project Structure
Fraud_Detection_System/

├── app.py                  
├── fraud_model.joblib     
├── label_encoder.joblib    
├── requirements.txt        
├── README.md

└── .gitignore

## Tech Stack

- **UI / Web App**: Streamlit
- **ML Model**: LightGBM (gradient boosting)
- **Data Handling**: pandas, numpy
- **Model Loading**: joblib
- **Geospatial**: geopy (geodesic distance)
- **Environment**: Python venv

## Quick Setup (Local)

### 1. Clone the repo

```bash
git clone https://github.com/avinashreddy09/Fraud_Detection_System.git
cd Fraud_Detection_System


# Create & activate venv
python -m venv .venv
.\.venv\Scripts\Activate.ps1          # Windows PowerShell

# Install dependencies
pip install streamlit lightgbm pandas numpy scikit-learn joblib geopy

# Run
python -m streamlit run app.py
