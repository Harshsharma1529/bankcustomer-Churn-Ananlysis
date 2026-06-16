# 🏦 Bank Marketing Campaign & Term Deposit Prediction

An end-to-end data science and machine learning web application built using **Scikit-Learn**, **Joblib**, and **Streamlit**. The project analyzes data from direct marketing campaigns (phone calls) of a Portuguese banking institution to predict whether a client will subscribe to a term deposit (`yes` or `no`).

This repository contains both the exploratory data/churn analysis notebook and a production-ready interactive dashboard for real-time predictions.

---

## 🚀 Features

* **Predictive Modeling:** Uses a trained **Decision Tree Classifier (`dtc_model.pkl`)** optimized to evaluate client responses based on socioeconomic and demographic inputs.
* **Automated Label Encoding:** Includes an exported preprocessing pipeline via **`encoder.pkl`** to handle multiple categorical attributes like job profiles, marital status, education, and contact months seamlessly.
* **Interactive Web UI:** Built an intuitive frontend using Streamlit where bank managers or marketing executives can manually enter customer parameters and get instant conversion feedback.
* **Deep Churn & Behavior Analysis:** The included Jupyter Notebook runs extensive Exploratory Data Analysis (EDA) on over 45,000 marketing instances to uncover hidden trends behind client rejection and engagement duration.

---

## 📊 Dataset Metadata

* **Source:** UCI Machine Learning Repository (Bank Marketing Dataset)
* **Total Instances:** 45,211 rows
* **Total Features:** 16 categorical/numerical features (Age, Job, Balance, Housing loan, Duration of call, etc.)
* **Target Variable (`y`):** Has the client subscribed to a term deposit? (`yes` / `no`)

---

## 🛠️ Project Structure

```text
├── ChurnAnalysis.ipynb  # Jupyter Notebook with EDA, profiling, and model training
├── app.py              # Production script for the Streamlit prediction dashboard
├── dtc_model.pkl       # Serialized Decision Tree Classifier model
├── encoder.pkl         # Serialized Scikit-Learn LabelEncoders for feature transformation
├── y.pkl               # Target variable matrix backup file
└── requirement.txt     # Complete Python dependencies checklist
