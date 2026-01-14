# Hospital Readmission & Discharge Risk Analysis (NY SPARCS)

## 1. Business Problem
Hospital readmissions and unsafe discharges increase costs and negatively impact patient outcomes.
This project analyzes inpatient hospital discharge data to identify **patients at high risk of readmission
or requiring intensive post-acute care**.

**Key Question:**  
Which inpatient discharges are most likely to result in readmission risk or complex post-discharge needs,
and what factors drive that risk?

---

## 2. Dataset
**New York Statewide Planning and Research Cooperative System (SPARCS)**  
Source: New York State Department of Health

SPARCS is a comprehensive, all-payer inpatient discharge dataset used by health systems,
researchers, and policymakers to analyze hospital utilization, outcomes, and efficiency.

> This project uses publicly available SPARCS data (CSV format).  
> No restricted or licensed data is included in this repository.

---

## 3. Objectives
- Identify high-risk discharge patterns using inpatient data
- Engineer clinically and operationally meaningful features
- Build a predictive risk model for discharge/readmission risk
- Translate insights into hospital operational recommendations

---

## 4. Target Definition (Portfolio-Appropriate)
Because SPARCS does not always include a direct 30-day readmission flag, risk is modeled using:
- Discharge disposition (SNF, rehab, home health)
- Length of stay (extended LOS)
- Emergency admissions
- Diagnosis severity categories

This approach mirrors real-world hospital risk stratification.

---

## 5. Methods Overview

### Feature Engineering (Examples)
- Demographics: age group, sex
- Admission context: emergency vs elective
- Clinical complexity: diagnosis groupings
- Utilization: length of stay buckets
- Discharge disposition
- Payer category

### Modeling
- Baseline: Logistic Regression
- Advanced: Tree-based model (Random Forest / Gradient Boosting)

### Evaluation Metrics
- ROC-AUC
- Precision / Recall
- Confusion Matrix
- Feature importance for interpretability

---

## 6. Project Structure

## 7. Tools
- Python (pandas, scikit-learn)
- Jupyter (VS Code)
- SQL (optional)
- Power BI (later stage)

## 8. Status
Project in progress — dataset selected, structure finalized.

