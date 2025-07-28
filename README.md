# 🧠 Phenotype Modeling – Subtype Classification & Severity Regression in Parkinson’s Disease

This machine learning project applies supervised learning to classify Parkinson’s Disease patients into motor subtypes — **Tremor Dominant (TD)** vs. **Postural Instability and Gait Difficulty (PIGD)** — and to model a continuous **phenotype ratio score** that reflects motor severity progression. The pipeline integrates structured psychological, cognitive, and motor assessments with regression and classification models to support clinical phenotyping.

<p align="center">
  <img src="phenotype_modeling.jpg" width="600"/>
  <br>
  <em>  Subtype classification and ratio prediction using psychological & sensorimotor indicators</em>
</p>

---

## 🧪 Dataset

- **Source**: IRB-approved clinical dataset (`DATA.csv`)
- **Observations**: Mild-to-moderate PD patients (n = 36)
- **Features**: 144 variables including:
  - Cognitive tests (TMT A/B, SDMT, MMSE)
  - Mood scores (GDS, PAS)
  - Balance metrics (ABC, mFFABQ, discordance)
  - Motor scores (MDS-UPDRS, HY stage)
- **Targets**:
  - `phenotype`: Binary (TD = 1, PIGD = 2)
  - `phenotype_ratio`: Continuous (TD:PIGD severity index)

---

## 🎯 Objectives

1. **Classification Task**
   - Identify TD vs. PIGD phenotype using:
     - Logistic Regression  
     - Gaussian Naive Bayes  
     - Random Forest Classifier

2. **Regression Task**
   - Predict phenotype ratio using:
     - Linear Regression
     - Feature selection + scaling

---

## ⚙️ ML Methods

- **Imputation**: IterativeImputer (scikit-learn)  
- **Scaling**: StandardScaler  
- **Validation**: Stratified Train-Test Split (75:25)  
- **Metrics**: Accuracy, Recall, Balanced Accuracy, R², MAE, RMSE  
- **Exploration**: Correlation heatmaps, bar plots, residual analysis

---

## 📈 Key Results

### 🔹 Classification Performance:
| Model | Accuracy | Notes |
|-------|----------|-------|
| Logistic Regression | **75%** | Balanced across both phenotypes |
| Naive Bayes | 75% | Slight bias toward PIGD |
| Random Forest | Moderate | High specificity for PIGD, lower TD sensitivity |

### 🔹 Regression Performance:
- **Adjusted R²**: 0.555  
- **RMSE**: 1.14  
- **MAE**: 0.91  
- **Top Predictors**: Persistent Anxiety (PAS), Depression (GDS), TMT B, HY Stage

---

## 📂 Files

- `Phenotype_Modeling_Final.ipynb` – Full modeling workflow with preprocessing, training, and evaluation  
- `DATA.csv` – Cleaned feature matrix with labeled targets  
- `phenotype_modeling.jpg` – Visual overview of modeling strategy

---

## 🧠 Why It Matters

Understanding how psychological and cognitive symptoms influence motor subtypes in PD could enable early, non-invasive screening and personalized interventions — especially for underserved or remote populations.

---

> This project bridges applied ML with human-centered health analytics — combining small-sample neurobehavioral data with interpretable model pipelines.

