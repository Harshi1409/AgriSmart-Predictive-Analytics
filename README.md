# AgriSmart – Agricultural Market Price Estimation

**A Machine Learning Project for Agricultural Market Price Estimation**

## 1. Project Overview

AgriSmart is a machine learning project focused on estimating agricultural commodity market prices using agricultural market and production-related data.

The project combines multiple agricultural datasets, performs data preprocessing and applies regression algorithms to analyse relationships between agricultural features and market prices.

It aims to explore how machine learning techniques can support agricultural price analysis through data-driven estimation.

## 2. Problem Statement

Agricultural commodity prices vary across markets, states, districts and crop varieties. Understanding these variations is important for analysing agricultural market behaviour.

The objective of AgriSmart is to develop a machine learning approach for estimating agricultural commodity modal prices using available market and production-related features.

## 3. Project Objectives

- Integrate agricultural market and crop production datasets.
- Perform data cleaning and preprocessing.
- Explore relationships between agricultural features and market prices.
- Implement and compare multiple regression algorithms.
- Evaluate model performance using standard regression metrics.
- Identify the best-performing model based on test results.

## 4. Dataset Description

The project uses agricultural data from the following sources:

| Dataset | Description |
|---|---|
| APMC Market Prices | Agricultural commodity market price information |
| ICRISAT District-Level Data | District-level agricultural statistics |
| India Agriculture Crop Production | Crop area, production and yield information |

**Processed Dataset:** `crop_data_v2.csv`

- Total observations: 2,444
- Total columns: 14

The processed dataset was prepared for machine learning analysis.

## 5. Project Workflow

**1. Data Collection**

Collected agricultural market price and agricultural production datasets from multiple sources.

**2. Data Preprocessing**

Performed data cleaning, handling of missing values and dataset integration.

**3. Feature Preparation**

Prepared relevant numerical and categorical features for regression analysis.

**4. Model Development**

Implemented five regression algorithms to estimate agricultural market prices.

**5. Model Evaluation**

Compared model performance using MAE, MSE, RMSE and R² score.

**6. Result Analysis**

Analysed the performance of each model and identified the best-performing algorithm.

## 6. Machine Learning Algorithms

Five regression algorithms were implemented and evaluated:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- Support Vector Regression (SVR)

## 7. Model Evaluation and Results

The models were evaluated using an 80:20 train-test split with a random state of 42.

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | 1,147.05 | 2,132.87 | **0.7550** |
| Gradient Boosting | 1,451.33 | 2,398.15 | 0.6903 |
| Random Forest | 1,636.86 | 2,650.12 | 0.6218 |
| Decision Tree | 1,849.93 | 2,966.52 | 0.5261 |
| Support Vector Regression | 1,886.15 | 4,268.53 | 0.0189 |

### Best Performing Model: Linear Regression

Linear Regression achieved the best performance among the five evaluated models.

- **R² Score:** 0.7550
- **MAE:** 1,147.05
- **RMSE:** 2,132.87

The model achieved an R² score of approximately 75.5% on the test dataset.

## 8. Technologies and Libraries

**Programming Language**
- Python

**Libraries**
- Pandas
- NumPy
- Scikit-learn

**Development Environment**
- Jupyter Notebook

**Machine Learning**
- Regression Analysis
- Model Training
- Model Evaluation
- Predictive Analytics

## 9. Repository Structure

```text
AgriSmart-Predictive-Analytics/
│
├── model_training.ipynb
├── prepare_dataset.ipynb
│
├── APMC_Market_Prices.csv
├── ICRISAT_District_Level_Data.csv
├── crop_data_v2.csv
│
├── model_evaluation_results.csv
└── test_set_predictions.csv
```

## 10. Project Files

| File | Description |
|---|---|
| `prepare_dataset.ipynb` | Data cleaning, preprocessing and dataset integration |
| `model_training.ipynb` | Model training and performance evaluation |
| `APMC_Market_Prices.csv` | Agricultural market price dataset |
| `ICRISAT_District_Level_Data.csv` | District-level agricultural dataset |
| `crop_data_v2.csv` | Processed dataset used for model development |
| `model_evaluation_results.csv` | Comparative model evaluation results |
| `test_set_predictions.csv` | Actual and predicted test-set values |

## 11. Key Findings

- Linear Regression achieved the highest R² score among the five evaluated models.
- Gradient Boosting was the second-best-performing model.
- Support Vector Regression showed the lowest predictive performance.
- Model comparison demonstrated that different regression algorithms produced different estimation results on the same dataset.

## 12. Project Limitations

- Model performance depends on the availability and quality of agricultural data.
- The evaluation is based on a random train-test split and does not establish future-date forecasting accuracy.
- Additional market observations and external validation would be useful to assess performance across different time periods and regions.

## 13. Author

**Harshita Bansal**

B.Tech – Computer Science and Engineering  
Lovely Professional University

[GitHub Profile](https://github.com/Harshi1409)

---

*AgriSmart – Agricultural Market Price Estimation using Machine Learning.*
