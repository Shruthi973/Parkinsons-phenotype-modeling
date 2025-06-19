# Parkinsons-phenotype-modeling
Statistical Modeling &amp; Machine Learning for Parkinson’s Disease Subtype Classification and Severity Prediction
## Parkinson’s Phenotype Modeling – Classification & Regression

This project explores clinical subtypes of Parkinson’s Disease using machine learning models to classify patients into Tremor-Dominant (TD) vs. Postural Instability and Gait Disorder (PIGD) types, and to model the continuous phenotype ratio using dual-task, cognitive, and psychological features.

### 🔍 Project Highlights
- **Data Source**: Real clinical research dataset of PD patients (TD + PIGD only)
- **Tools Used**: R, Naive Bayes, Logistic Regression, Random Forest, `mice`, `ggplot2`
- **Classification Models**:
  - Logistic Regression (Accuracy: 57.1%)
  - Naive Bayes (Balanced Accuracy: 58.3%) – best sensitivity
  - Random Forest (High specificity but failed to detect TD)
- **Regression Model**:
  - Adjusted R² = 0.555 on test data
  - Key predictors: Anxiety, Depression, Balance Discordance, HY Stage
  - RMSE = 1.14, MAE = 0.91

### 📈 Key Insight
Psychological and perceptual variables (e.g., anxiety, depression, balance confidence) were stronger predictors of PD phenotype than cognitive tests. The results support a continuous understanding of motor symptom dominance rather than binary classification.

### 📂 What's Inside
- `R_FILE.Rmd`: Source code with classification + regression modeling
- `R_JUNE.pdf`: Final report with clinical/statistical interpretations
- `R_FILE.knit.html_JUNE.html`: Rendered notebook with plots and model outputs
