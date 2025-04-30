# 🛡️ System_Threat_Prediction(Kaggle Competition)


This repository contains my solution for the **System Threat Prediction** competition hosted on Kaggle. The challenge was to develop a model that predicts whether a Windows machine will be infected by malware, based on anonymized telemetry data collected by antivirus software.

> 🔒 **Note**: The dataset used in this project is from a private Kaggle competition and cannot be shared or uploaded to this repository due to confidentiality restrictions.

---

## 🎯 Objective

The goal is to predict the probability that a system will get infected with malware, using system configuration and software/hardware details provided in the telemetry data.

---

## 📁 Files in This Repo

- `malware_prediction.ipynb`: Jupyter notebook containing data exploration, preprocessing, feature selection, model training, and evaluation. All outputs are included.
- `README.md`: This file.

---

## 📊 Dataset Summary

Each row in the dataset represents a unique machine and contains features such as:

- **Software/Version Info**: `OSVersion`, `AppVersion`, `EngineVersion`, `SignatureVersion`
- **Security Settings**: `FirewallEnabled`, `IsSystemProtected`, `IsSecureBootEnabled`
- **Hardware Specs**: `ProcessorCoreCount`, `TotalPhysicalRAMMB`, `HasTPM`
- **Geographic & System Metadata**: `CountryID`, `GeoRegionID`, `LocaleEnglishNameID`
- **Target Column**: `target` (1 = malware detected, 0 = not detected)

---

## ⚙️ My Approach

- Exploratory Data Analysis (EDA)
- Handling missing values and rare categories
- Label and one-hot encoding for categorical features
- Feature selection using Random Forest importance
- Model training with:
  - **Random Forest**
  - **XGBoost**
- Evaluation using AUC and cross-validation

---

## 📈 Results

- ✅ **My Kaggle Public Score**: `0.62`
- 🥇 **Best Score on Leaderboard**: `0.70`

---

## 🚀 Future Improvements

- Advanced ensembling or stacking techniques
- More sophisticated feature engineering
- Hyperparameter tuning via Bayesian optimization
- Deep learning-based approaches for tabular data

---

## 📌 Notes

- This notebook was developed and submitted on Kaggle.
- Outputs are preserved in the notebook file.
- Dataset access requires joining the official competition via Kaggle.

---

## 🔗 Useful Links


- [XGBoost Documentation](https://xgboost.readthedocs.io/)
- [scikit-learn Documentation](https://scikit-learn.org/stable/)

---
