#  Explainable Bitcoin Volatility Prediction using Machine Learning and Technical Indicators

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange.svg)
![XGBoost](https://img.shields.io/badge/XGBoost-Latest-green.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-Deployed-red.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

---

#  Project Overview

Bitcoin is one of the most volatile financial assets, making volatility prediction an important task for traders, investors, and financial analysts.

This project develops an **Explainable Machine Learning framework** to predict **21-day Bitcoin volatility** using historical market data and technical indicators. Multiple machine learning models are trained and compared, while explainability techniques such as **SHAP** are used to interpret model predictions.

---

#  Objectives

- Predict Bitcoin's 21-day volatility.
- Perform comprehensive feature engineering using technical indicators.
- Compare multiple machine learning models.
- Explain model predictions using SHAP.
- Evaluate model performance using time-series validation.
- Build a deployable machine learning application.

---

#  Dataset

**Source:** Kaggle

The dataset contains historical Bitcoin market data from **2013 to 2021**, including:

- Date
- Open
- High
- Low
- Close
- Volume
- Market Capitalization

---

#  Data Preprocessing

The following preprocessing steps were performed:

- Removed unnecessary columns
- Converted Date column to datetime format
- Checked missing values
- Exploratory Data Analysis (EDA)
- Correlation analysis
- Distribution analysis
- Time-series visualization

---

#  Feature Engineering

A total of **45 features** were created, including:

## Price-Based Features

- Returns
- Log Returns
- Price Change
- High-Low Spread
- Open-Close Spread

## Volatility Features

- 7-Day Volatility
- 14-Day Volatility
- 21-Day Volatility
- Lagged Volatility Features

## Trend Indicators

- SMA (10,20)
- EMA (10,20)
- MACD
- MACD Signal
- MACD Histogram

## Momentum Indicators

- RSI
- ROC
- Stochastic Oscillator
- Williams %R

## Volatility Indicators

- Bollinger Bands
- ATR
- Donchian Channels

## Rolling Statistics

- Rolling Mean
- Rolling Standard Deviation
- Rolling Maximum
- Rolling Minimum

---

#  Machine Learning Models

The following regression models were trained and evaluated:

- Decision Tree Regressor
- Random Forest Regressor
- XGBoost Regressor

---

#  Explainability

The project includes:

- Feature Importance
- SHAP Summary Plot
- SHAP Feature Contribution Analysis

These techniques improve model transparency and interpretability.

---

#  Model Performance

| Model | RMSE | MAE | R² |
|-------|------:|------:|------:|
| Decision Tree (Tuned) | 0.003780 | 0.001915 | 0.9536 |
| Random Forest | 0.003311 | 0.001584 | 0.9646 |
| **XGBoost ** | **0.002931** | **0.001644** | **0.9722** |

###  Best Performing Model

**XGBoost Regressor**

---

#  Model Validation

The project uses:

- Chronological Train-Test Split
- TimeSeriesSplit Cross Validation
- Hyperparameter Tuning
- Residual Error Analysis
- Actual vs Predicted Comparison

---

#  Project Structure

```text
Bitcoin-Volatility-Prediction/
│
├── data/
├── notebooks/
├── models/
├── images/
├── research_paper/
├── streamlit_app/
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

#  Results

The project includes visualizations such as:

- Bitcoin Price Trend
- Correlation Heatmap
- Closing Price Distribution
- Feature Importance
- SHAP Summary Plot
- Actual vs Predicted Graph
- Residual Error Plot
- Model Comparison
- Version 1 vs Version 2 Comparison

---

#  Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- XGBoost
- SHAP
- Joblib
- TA (Technical Analysis Library)
- Streamlit

---

#  Future Improvements

- Include news and social media sentiment.
- Use deep learning models such as LSTM and Transformer.
- Extend the framework to other cryptocurrencies.
- Develop a real-time prediction system using live market data.
- Improve the Streamlit dashboard with advanced visualizations.

---

#  Limitations

- Uses only historical Bitcoin market data.
- Does not include external news or sentiment.
- Performance on other cryptocurrencies has not been evaluated.
- Sudden market events may affect prediction accuracy.

---

#  Installation

### Clone the repository

```bash
git clone https://github.com/lakshya100806/BITCOIN-VOLATILITY-PREDICTOR-.git
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Run the Streamlit application

```bash
streamlit run app.py
```

---

#  Research Paper

The complete research paper is available in the **research_paper/** folder.

---

#  Author

**Lakshya Prajapat**
**Kanishka Bhandari**

Machine Learning Enthusiast | Python Developer | Data Science Student

**GitHub:**  
https://github.com/lakshya100806

**LinkedIn:**  
https://www.linkedin.com/in/lakshya-9171b9379/

---

#  Support

If you found this project helpful, please consider giving it a **⭐ Star** on GitHub.

It helps others discover the project and supports my work.
