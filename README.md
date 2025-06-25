# 🧠 Parkinson’s Disease Phenotype Modeling – Subtype Classification & Severity Prediction

This clinical machine learning project explores the classification of Parkinson's Disease patients into two motor subtypes—Tremor Dominant (TD) vs. Postural Instability and Gait Disorder (PIGD)—and models a continuous severity ratio using psychological, cognitive, and balance-related variables.

## 🧪 Dataset
- Source: Real-world clinical study data (`DATA.csv`)
- 144 features → motor scores, cognitive test results, balance confidence, fear of falling, mood assessments, dual-tasking performance
- Target variables:
  - `phenotype` (1 = TD, 2 = PIGD)
  - `phenotype_ratio` (continuous: tremor/pigd dominance)

## 🎯 Goals
1. **Classify** phenotype groups using:
   - Logistic Regression
   - Naive Bayes
   - Random Forest

2. **Predict** phenotype ratio using:
   - Linear Regression
   - Feature scaling and imputation

## 🔧 Methods
- Imputation: `IterativeImputer` (PMM-style)
- Stratified Train-Test Split
- Standardization with `StandardScaler`
- Evaluation: Accuracy, Recall, Confusion Matrix, R², RMSE, MAE

## 🧠 Results Summary

### ✅ Classification
- **Logistic Regression Accuracy**: 75%
- **Naive Bayes Balanced Accuracy**: 75%
- **Random Forest**: High specificity but lower sensitivity to TD group

### 📈 Regression
- **Adjusted R²**: 0.555
- **Key Predictors**: Anxiety, Depression, Balance Discordance, HY Stage
- **RMSE**: 1.14, **MAE**: 0.91

## 📂 Files
- `Phenotype_Modeling_Final.ipynb`: Full classification and regression workflow with plots and interpretations
