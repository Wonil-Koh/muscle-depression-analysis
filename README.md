# Global Analysis: Muscle Mass & Depression Correlation

## 📌 Project Overview
This project performs a comprehensive statistical analysis to investigate the **correlation between muscle mass and depression** across different racial groups (White, Black, Asian, and Hispanic).

Instead of relying on a single dataset, this project utilizes **Monte Carlo Simulation** to reverse-engineer and synthesize raw data points based on summary statistics (sample size, correlation coefficient, and slope) derived from prior research. The goal is to determine if there is a universal, cross-demographic inverse relationship between muscle mass and depression symptoms.

## 📊 Key Findings
Based on the integrated simulation of **2,201 individuals**, the global analysis reveals:

* **Total Sample Size (N):** 2,201
* **Pearson Correlation (r):** `-0.1440`
* **P-value:** `1.13e-11` (p < 0.001)
* **Conclusion:**
    The analysis demonstrates a **statistically significant negative correlation** between muscle mass and depression scores. Regardless of racial background, higher muscle mass is consistently associated with lower depression levels.

## 🛠 Methodology
This project does not use restricted raw medical data. Instead, it employs a statistical simulation approach:

1.  **Input Parameters:** Utilizing reported summary statistics ($N$, $r$, $Slope$) for four major demographic groups.
2.  **Data Simulation:** Generating synthetic data points using **Multivariate Normal Distribution** to replicate the statistical properties of the original populations.
3.  **Global Integration:** Merging specific group data into a single global dataset to perform a unified regression analysis.

## 📁 Repository Structure
```bash
muscle-depression-analysis/
├── main.py              # Main script for data generation, analysis, and plotting
├── requirements.txt     # List of dependencies
├── muscle_depression_analysis.png  # Generated regression plot
└── README.md            # Project documentation

Wonil Koh, DKM, DiplOM, PhD
wkoh1231@gmail.com
