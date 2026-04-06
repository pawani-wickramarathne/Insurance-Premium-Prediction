# Insurance Premium Prediction

Predicting medical insurance charges using machine learning.  
Built as a portfolio project leveraging my actuarial and statistical background.

## Problem Statement
Insurance companies need accurate premium pricing models. This project predicts  
individual medical charges based on demographic and health factors.

## Dataset
- **Source:** [Kaggle — Medical Cost Personal Dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance)
- **Size:** 1,338 records, 7 features
- **Features:** age, sex, bmi, children, smoker, region, charges

## Methodology
1. **EDA** — distribution analysis, smoker vs charges, age vs charges
2. **Feature Engineering** — label encoding of categorical variables
3. **Correlation Analysis** — heatmap to identify key predictors
4. **Model Training** — compared 3 models on 80/20 train/test split
5. **Feature Importance** — identified most influential predictors

## Results

| Model | RMSE | R² |
|---|---|---|
| Linear Regression | $5,799 | 0.78 |
| Random Forest | $4,590 | 0.86 |
| XGBoost | $4,822 | 0.85 |

**Random Forest achieved the best performance** with R² = 0.86.

## Key Findings
- Smoking status is the dominant predictor of insurance charges (importance: 0.60)
- BMI and age are the next most influential features
- Sex and region have negligible impact on charges
- Tree-based models outperform Linear Regression due to non-linear risk interactions

## Tools & Libraries
Python, pandas, NumPy, scikit-learn, XGBoost, matplotlib, seaborn

## Author
**Pawani Wickramarathne**  
[LinkedIn](https://www.linkedin.com/in/pawani-madhusara) | [Portfolio](https://pawani-wickramarathne.github.io)
