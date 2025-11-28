# Loan Default Prediction Model

A machine learning solution to identify high-risk loan applicants and reduce default-related losses for financial institutions.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Random%20Forest-orange)
![Status](https://img.shields.io/badge/Status-Ready%20for%20Pilot-brightgreen)

## 📊 Project Overview

**Business Problem:** Banks lose millions annually due to loan defaults. This project develops a predictive model to identify risky applicants before loan approval, enabling proactive risk management.

**Solution:** A Random Forest classification model that predicts loan default probability with 85% accuracy, successfully identifying 67% of potential defaults.

## 🎯 Key Features

- **Comprehensive Data Analysis**: 17+ visualizations uncovering default patterns
- **High-Performance Model**: 89% overall accuracy with 67% recall rate
- **Actionable Insights**: Clear risk factors identified and quantified
- **Production Ready**: Includes implementation strategy and bias mitigation

## 📈 Dataset

- **Total Records**: 255,347 historical loans
- **Features**: 17 borrower characteristics (demographic, financial, loan-specific)
- **Target Variable**: Loan default (Binary: Yes/No)
- **Class Distribution**: 
  - 88.4% Non-default (✅ Repaid)
  - 11.6% Default (❌ Defaulted)

## 🔍 Key Insights Discovered

### Demographic Risk Factors
- **Age**: 18-25 year olds have 70% higher default rates than 46+
- **Employment**: Full-time employees have 44% lower risk than unemployed
- **Education**: Master's degree holders default at 9.3% vs 13.8% for high school
- **Job Stability**: 10+ years at same employer = lowest default risk (8.9%)

### Financial Risk Indicators
- **Credit Score**: Below 500 = 25%+ default rate
- **Debt-to-Income**: DTI > 0.7 = 20%+ default rate
- **Loan-to-Income**: Large loans + low income = highest risk combination
- **Existing Debt**: 4+ credit lines = significantly higher risk

## 🤖 Machine Learning Model

### Model Selection
- **Algorithm**: Random Forest Classifier
- **Selection Reason**: Handles complex relationships, resists overfitting
- **Train/Test Split**: 80%/20% (204,277 / 51,070 records)

### Performance Metrics
| Metric | Score | Description |
|--------|-------|-------------|
| **Accuracy** | 85% | Overall prediction correctness |
| **Recall** | 67% | Percentage of actual defaults caught |
| **Precision** | 68% | Accuracy when predicting default |
| **F1-Score** | 68% | Balance of precision and recall |

### Feature Importance
The model identified these as the strongest predictors:
1. Credit Score
2. Interest Rate  
3. Debt-to-Income Ratio
4. Income
5. Loan Amount
6. Employment Type
7. Age

## 🚀 Business Impact

### Immediate Value
- **Risk Reduction**: Prevents ~67% of potential defaults
- **Cost Savings**: Estimated $40M+ annual savings
- **Better Decision Making**: Data-driven, consistent risk assessment
- **Faster Processing**: Automated risk scoring speeds up approvals

### Implementation Strategy
- **Phased Rollout**: Start with 10% of new applications
- **Human Oversight**: Loan officers review high-risk predictions
- **Bias Mitigation**: Regular fairness audits
- **Continuous Learning**: Monthly model retraining

## 🛠️ Technical Implementation

### Requirements
```bash
Python 3.8+
pandas
scikit-learn
matplotlib
seaborn
numpy
jupyter
