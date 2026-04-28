# Medical Cost Analysis — Data Analytics Project

## Overview
Analysis of medical insurance costs for 1,337 beneficiaries using Excel.  
Identified key factors driving healthcare expenses including smoking, BMI, region, and dependents.

---

## Dataset
- **Source:** IBM Medical Cost Dataset (Kaggle)
- **Records:** 1,337 patients
- **Features:** Age, Sex, BMI, Children, Smoker, Region, Charges

---

## Tools Used
- Microsoft Excel
- Pivot Tables
- Excel Charts (Bar, Scatter, Histogram, Pie)
- DAX Formulas (AVERAGEIF, COUNTIF, IF, PERCENTILE)

---

## Project Structure
```
Medical-Cost-Analysis/
│
├── Medical_Cost_Analysis.xlsx     # Main Excel workbook
├── Medical_Cost_Analysis.pptx    # Presentation with insights
├── insurance.csv                  # Raw dataset
└── README.md
```

---

## Analysis Performed

### Q1 — Basic Statistics
- Average Charges: **$13,279**
- Median Charges: **$9,386**
- Std Dev: **$12,110**
- Distribution is right-skewed — small group has very high costs

### Q2 — Gender Analysis
| Gender | Avg Charges | Avg BMI |
|--------|------------|---------|
| Male   | $13,975    | 30.94   |
| Female | $12,570    | 30.38   |

### Q3 — Smoking Impact
| Status      | Avg Charges |
|-------------|------------|
| Smokers     | $32,050    |
| Non-Smokers | $8,441     |

> **Smokers pay 3.8x more than non-smokers — single biggest cost driver**

### Q4 — Dependents Analysis
- Beneficiaries with 2–3 children have highest charges (~$15,000+)
- Scatter plot shows wide variation across all dependent groups

### Q5 — Regional Insights
| Region    | Avg Charges | Avg BMI |
|-----------|------------|---------|
| Southeast | $14,735 ▲  | 33.36 ▲ |
| Southwest | $12,347 ▼  | 30.60   |
| Northeast | $13,406    | 29.17   |
| Northwest | $12,451    | 29.20   |

### Q6 — Cost Distribution
- Most beneficiaries fall in **$1,000–$5,000** bracket (356 patients)
- Distribution is right-skewed

### Q7 — BMI Classification
| Category    | Count | Share |
|-------------|-------|-------|
| Obese       | 706   | 53%   |
| Overweight  | 386   | 29%   |
| Normal      | 225   | 17%   |
| Underweight | 20    | 1%    |

> **82% of beneficiaries are overweight or obese**

### Q8 — BMI vs Charges Correlation
- R² = 0.039 — weak positive correlation
- BMI alone is not a strong predictor of costs
- Smoking + High BMI = biggest combined risk factor

### Q9 — Smoking × Region
| Region    | Smokers Avg Charges |
|-----------|-------------------|
| Southeast | $34,845 ▲         |
| Southwest | $32,269           |
| Northwest | $30,192           |
| Northeast | $29,674           |

### Q10 — Interactive Dashboard
- Built in Excel with 6 charts and 4 slicers
- Filters: Sex, Smoker, Region, BMI Classification

---

## Key Insights

1. **Smoking = #1 Cost Driver** — 3.8x higher charges vs non-smokers
2. **Southeast = Highest Risk Region** — highest charges + highest BMI
3. **82% Overweight or Obese** — systemic health risk in dataset
4. **2–3 Children = Peak Costs** — families with 2–3 dependents pay most

---

## Dashboard Preview
![Dashboard](images/dashboard.png)

---

## Author
**Ikram Hussain**  
Data Analyst | SQL • Power BI • Advanced Excel  
[LinkedIn](https://www.linkedin.com/in/ikramhussain-6886b454) | [GitHub](https://github.com/Ikramhussain90)
