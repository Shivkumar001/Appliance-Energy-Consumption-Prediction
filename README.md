# ⚡ Appliance Energy Consumption Prediction

## Machine Learning Regression Project

Predicting household appliance energy consumption using environmental, temporal, lagged, and rolling features.

---

## 📌 Project Overview

Household appliance energy consumption varies according to time of day, environmental conditions, seasonal patterns, and recent consumption behavior.

This project develops a machine learning regression pipeline to predict appliance energy consumption using historical household and environmental measurements.

The project includes:

- Exploratory Data Analysis
- Data preprocessing
- Temporal feature engineering
- Lag features
- Rolling statistics
- Regression model comparison
- Hyperparameter tuning
- Time-series cross-validation
- SHAP explainability
- Residual and prediction error analysis

---

## 🎯 Objective

Build a regression model capable of predicting household appliance energy consumption from environmental and time-based features.

The project aims to identify the strongest factors affecting energy usage while comparing multiple machine learning approaches.

---

## 📊 Dataset

The dataset contains approximately **19,735 observations** collected over a one-year period.

The target variable is **Appliances**, representing appliance energy consumption.

The dataset includes measurements such as:

- Temperature
- Humidity
- Outdoor weather conditions
- Atmospheric pressure
- Wind speed
- Visibility
- Dew point
- Lighting energy usage
- Timestamp information

---

## 🔍 Exploratory Data Analysis

The analysis investigates:

- Appliance energy distribution
- Temporal consumption patterns
- Hourly usage
- Weekday vs weekend behavior
- Environmental relationships
- Temperature and humidity effects
- Correlation patterns
- Outliers and extreme consumption events

Key observations include higher consumption during evening hours and relationships between energy demand and environmental conditions.

---

## 🛠️ Feature Engineering

Several features were created to capture temporal and short-term consumption behavior.

### Temporal Features

- Hour of day
- Day of week
- Month / season

### Lag Features

- Previous-hour appliance consumption

### Rolling Features

- 10-hour rolling mean
- Short-term consumption trends

### Environmental Features

- Temperature differences
- Humidity patterns

---

## 🤖 Models Compared

Three regression approaches were evaluated:

1. Linear Regression
2. Random Forest
3. XGBoost

XGBoost was further tuned using randomized hyperparameter search and time-series cross-validation.

---

## 📈 Model Evaluation

Models were evaluated using:

- RMSE
- MAE
- R² Score

The current notebook reports the following final XGBoost evaluation:

| Metric | XGBoost |
|---|---:|
| RMSE | 64.57 |
| R² | 0.5498 |

Time-series cross-validation was also performed to evaluate model stability across temporal splits.

---

## 🧠 SHAP Explainability

SHAP was used to understand which features influence model predictions.

The analysis investigates:

- Global feature importance
- Feature impact direction
- Individual prediction explanations
- Dependence between important features and predictions

---

## 💡 Key Insights

The analysis highlights the importance of:

- Time of day
- Outdoor temperature
- Recent appliance consumption
- Indoor temperature
- Humidity conditions

These variables help capture both environmental demand and short-term household usage behavior.

---

## 📁 Repository Structure

Appliance-Energy-Consumption-Prediction/

├── data/
│   └── energydata_complete.csv
│
├── notebooks/
│   └── Predicting_Appliance_Energy_Consumption.ipynb
│
├── docs/
│   └── Appliance_Energy_Consumption_Report.pptx
│
├── .gitignore
├── README.md
├── requirements.txt
└── description.txt

---

## 🛠️ Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn
- SHAP
- Jupyter Notebook
- Joblib

---

## ⚠️ Note

This project is an analytical and machine learning exercise based on historical household energy consumption data.

Model performance may vary depending on the train/test split, feature engineering, temporal validation strategy, and future data.

---

## 👤 Author

**Shiv Kumar**

Data Analyst
