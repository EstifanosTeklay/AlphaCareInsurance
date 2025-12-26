# AlphaCareInsurance
# Insurance Claims & Premium Optimization using Machine Learning

This project applies statistical modeling and machine learning techniques to
analyze insurance claims and optimize premium pricing for AlphaCare Insurance
Solutions. The goal is to identify key risk drivers and develop predictive
models that support data-driven underwriting and pricing decisions.

## 📌 Business Problem

Accurate premium pricing and claims prediction are critical for insurance
profitability and customer retention. Traditional pricing models often fail
to capture complex non-linear relationships between policy, vehicle, customer,
and location attributes.

This project addresses:
- Claims prediction at policy and location level
- Premium optimization using machine learning
- Identification of key risk and pricing drivers
## 📊 Dataset Overview

The dataset contains over **618,000 insurance policy records**, including:

- Customer demographics and financial attributes
- Vehicle characteristics and age
- Policy and coverage details
- Geographic risk indicators
- Historical premium and claims information

Target variables:
- `TotalClaims`
- `TotalPremium`
## 🔧 Methodology
1. **Data Cleaning & Preparation**
   - Missing value treatment
   - Feature engineering (vehicle age, power ratios, loss metrics)
   - Categorical encoding
   - Train-test split (80/20)

2. **Modeling Techniques**
   - Linear Regression (baseline)
   - Random Forest Regression
   - XGBoost Regression

3. **Evaluation Metrics**
   - RMSE
   - MAE
   - R² Score

4. **Feature Importance Analysis**
   - Tree-based feature importance
   - Business interpretation of drivers

## 🤖 Models Implemented

| Model              | Purpose |
|-------------------|--------|
| Linear Regression | Baseline & interpretability |
| Random Forest     | Non-linear modeling & feature importance |
| XGBoost           | High-performance predictive modeling |

XGBoost delivered the best performance for both claims and premium prediction.

## 📈 Key Findings

- Tree-based models significantly outperform linear regression
- Premium is strongly influenced by:
  - Sum insured
  - CalculatedPremiumPerTerm
  - TransactionMonthNum
- Claims risk is heavily affected by:
  - Vehicle age
  - Geographic risk (CRESTA zones, postal codes)
  - Coverage structure
## 💡 Business Recommendations
- Introduce risk-adjusted pricing using vehicle age and power metrics
- Enhance location-based pricing granularity
- Optimize excess structures to balance affordability and risk
- Integrate ML-driven pricing into underwriting workflows
## ▶️ How to Run the Project
1. Clone the repository
bash
git clone https://github.com/EstifanosTeklay/AlphaCareInsurance.git
2. Install dependencies
pip install -r requirements.txt
3. Run AcisData.ipynb notebook

🛠️ Tools & Technologies

Python

Pandas, NumPy

Scikit-learn

XGBoost

Matplotlib / Seaborn

📌 Disclaimer

This project is for analytical and educational purposes only. All data has
been anonymized and does not represent real customers.

👤 Author
### Estifanos Teklay
### Senior Business Intellegence Analyst | Data Scientist 

