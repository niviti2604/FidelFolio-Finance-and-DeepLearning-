# FidelFolio Mid Prep — Finance + Deep Learning

##  Problem Statement

In equity markets, valuation and investment decisions are driven by fundamental indicators such as earnings, margins, growth rates, and capital structure. This project aims to build deep learning models that predict **market capitalization growth** of Indian listed companies using a curated dataset of **historical fundamental features**.
You are to model complex, non-linear relationships between these indicators and future market performance across **1-year, 2-year, and 3-year time horizons**.

---

##  Dataset Overview

Each data sample includes:
- **Year**: Fiscal year of the snapshot
- **Company**: Name of the listed Indian company
- **Feature1 - Feature28**: 28 financial indicators
- **Target1**: 1-year forward market cap growth (%)
- **Target2**: 2-year forward market cap growth (%)
- **Target3**: 3-year forward market cap growth (%)

Dataset link: [Google Drive](https://drive.google.com/file/d/13pZZNGg9xaCVVNs4yLHfZQhK9VJ4DNQt/view?usp=drive_link)

---

##  Steps to Run the Project
1.Install Required Libraries
pip install -r requirements.txt

2.Preprocessing
Missing Value Imputation
Outlier Handling (via IQR/Winsorisation)
Feature Normalization
Avoiding Data Leakage: Only past data is used for training.

3.We experimented with a range of deep learning models:
MLP (Multi-Layer Perceptron)
LSTM (Long Short-Term Memory)
Transformer-Based Tabular Models

4.Models were evaluated on Root Mean Squared Error (RMSE) across:
Target1: 1Y forward growth
Target2: 2Y forward growth
Target3: 3Y forward growth

5.Feature importance visualizations
