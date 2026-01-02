# Hospital Readmission Risk Analysis (HCUP NRD)

## 1. Business Problem
Hospital readmissions within 30 days of discharge increase healthcare costs and often indicate gaps in care coordination and discharge planning.  
This project focuses on identifying patients at **high risk of 30-day readmission** to support targeted interventions and improve outcomes.

**Key Question:**  
Which patients are most likely to be readmitted within 30 days, and what clinical or operational factors drive that risk?

---

## 2. Dataset
**HCUP Nationwide Readmissions Database (NRD)**  
Source: Agency for Healthcare Research and Quality (AHRQ)

The NRD is a nationally representative U.S. inpatient database designed specifically for readmission analysis.

> ⚠️ Raw NRD data is not included in this repository due to licensing restrictions.  
> This project focuses on reproducible analytics workflows, feature engineering logic, and modeling approaches.

---

## 3. Objectives
- Build a **binary classification model** to predict 30-day readmission
- Engineer clinically meaningful features from inpatient encounter data
- Evaluate performance using healthcare-appropriate metrics
- Translate insights into actionable recommendations

---

## 4. Methods Overview

### Feature Engineering (Examples)
- Demographics: age group, sex
- Clinical burden: comorbidity count, chronic condition indicators
- Utilization history: prior admissions, length of stay
- Encounter context: admission type, discharge disposition
- Payer characteristics

### Modeling
- Baseline: Logistic Regression
- Advanced: Tree-based model (e.g., Random Forest or Gradient Boosting)
- Class imbalance handling via class weights or threshold tuning

### Evaluation Metrics
- ROC-AUC
- Precision, Recall, F1-Score
- Confusion Matrix
- Model interpretability for clinical relevance

---

## 5. Project Structure
01_readmission_risk_nrd
├── notebooks # EDA and modeling notebooks
├── src # Python scripts for reusable logic
├── sql # Cohort and feature SQL
├── docs # Reports and documentation
└── data # Raw/processed placeholders (no PHI stored)
---

## 6. Deliverables
- Exploratory Data Analysis
- Feature engineering pipeline
- Predictive readmission model
- Model performance evaluation
- Business and clinical insights

---

## 7. Tools
- Python (pandas, scikit-learn)
- SQL
- Jupyter (via VS Code)
- Power BI (later phase)

---

## 8. Status
🚧 Project in progress — structure and foundation completed.



