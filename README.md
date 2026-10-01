# Final_Thesis_Project
🚗 Indian Used Car Price Prediction using Python and Machine Learning | EDA, Data Preprocessing, Feature Engineering, Decision Tree, Random Forest, GridSearchCV &amp; Model Evaluation.
# 🚗 Indian Used Car Price Prediction Using Machine Learning

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python" alt="Python">
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-purple?style=for-the-badge&logo=pandas" alt="Pandas">
  <img src="https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange?style=for-the-badge&logo=scikit-learn" alt="Scikit-Learn">
  <img src="https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter" alt="Jupyter">
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" alt="Status">
</p>

## 📌 Project Overview

The **Indian Used Car Price Prediction** project applies **Data Science and Machine Learning** techniques to analyse the Indian used-car market and predict vehicle prices.

The project combines **Exploratory Data Analysis (EDA), data preprocessing, feature engineering, regression modelling, hyperparameter tuning, and model evaluation** to understand the factors associated with used-car prices.

Two regression algorithms were implemented:

- 🌳 **Decision Tree Regressor**
- 🌲 **Random Forest Regressor**

The models were evaluated using **Mean Squared Error (MSE), Mean Absolute Error (MAE), and R² Score**.

The analysis also investigates how factors such as **car company, model, fuel type, colour, mileage, body style, car age, location, ownership, warranty, and quality score** relate to used-car prices.

---

## 🎯 Project Objectives

The main objectives of this project are to:

- Understand the characteristics of the Indian used-car dataset.
- Perform exploratory data analysis to identify important market patterns.
- Clean and preprocess the raw dataset.
- Convert categorical variables into numerical representations.
- Identify and remove outliers using the **Interquartile Range (IQR)** method.
- Analyse correlations between variables.
- Develop regression models for used-car price prediction.
- Tune model hyperparameters using **GridSearchCV**.
- Compare Decision Tree and Random Forest regression performance.
- Identify important features influencing predicted car prices.

---

## 📊 Dataset

The dataset contains **1,064 used-car records and 19 original variables**.

### Dataset Features

| Feature | Description |
|---|---|
| `Id` | Unique identifier of the car |
| `Company` | Car manufacturer |
| `Model` | Car model |
| `Variant` | Specific car variant |
| `FuelType` | Fuel type |
| `Colour` | Car colour |
| `Kilometer` | Distance travelled |
| `BodyStyle` | Body style of the vehicle |
| `TransmissionType` | Transmission type |
| `ManufactureDate` | Vehicle manufacture date |
| `ModelYear` | Vehicle model year |
| `CngKit` | CNG kit information |
| `Price` | Used-car selling price |
| `Owner` | Ownership information |
| `DealerState` | State where the car is sold |
| `DealerName` | Dealer name |
| `City` | City where the car is sold |
| `Warranty` | Warranty availability |
| `QualityScore` | Vehicle quality score |

### Target Variable

**`Price`** is used as the target variable for the regression models.

---

# 🔄 Project Workflow

```text
                    ┌─────────────────────┐
                    │   Used Car Dataset  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Data Understanding  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Data Cleaning     │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Exploratory Data    │
                    │      Analysis       │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Feature Processing  │
                    │ & Label Encoding    │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Outlier Detection   │
                    │      Using IQR      │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Correlation Analysis│
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Train-Test Split    │
                    └──────────┬──────────┘
                               │
                ┌──────────────┴──────────────┐
                ▼                             ▼
       ┌─────────────────┐          ┌─────────────────┐
       │ Decision Tree   │          │ Random Forest   │
       │   Regressor     │          │   Regressor     │
       └────────┬────────┘          └────────┬────────┘
                │                            │
                ▼                            ▼
       ┌─────────────────┐          ┌─────────────────┐
       │ GridSearchCV &  │          │ GridSearchCV &  │
       │ 5-Fold CV       │          │ 5-Fold CV       │
       └────────┬────────┘          └────────┬────────┘
                │                            │
                └──────────────┬─────────────┘
                               ▼
                    ┌─────────────────────┐
                    │ Model Evaluation    │
                    │ MSE | MAE | R²      │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Feature Importance  │
                    └─────────────────────┘
