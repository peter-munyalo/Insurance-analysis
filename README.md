<img width="703" height="404" alt="image" src="https://github.com/user-attachments/assets/31f4b72d-c027-4cde-b55c-0d99b4ad3d48" />

# Kenya Motor Insurance: Underwriting Risk & Profitability Analytics

##  Project Overview
In the competitive Kenyan insurance landscape, maintaining a sustainable **Loss Ratio** is critical for long-term profitability. This project analyzes a portfolio of 2,000+ motor insurance policies (2023-2024) to identify high-risk segments, evaluate regional performance, and provide data-driven recommendations for premium loading.

The goal is to demonstrate how applied statistics and interactive business intelligence can reduce "claims leakage" and improve the **Combined Ratio**.

## 📊 Live Dashboard
> **[Click Here to View Interactive Dashboard](https://app.powerbi.com/links/jnNP1-Ch6D?ctid=14f13a17-3cb4-408b-b8e4-770d44d82165&pbi_source=linkShare)**

---

## Tech Stack & Methodology

### 1. Data Engineering (Python)
* **ETL Process:** Used Pandas and NumPy to clean raw insurance records.
* **Feature Engineering:** * Calculated `Loss_Ratio` per policy.
    * Engineered a `Risk_Profile` classifier based on claim-to-premium variance.
    * Standardized regional data for accurate geographic mapping.

### 2. Data Modeling & DAX (Power BI)
* Built a robust relational model to handle multi-year insurance trends.
* **Key Measures Created:**
    * **Total GWP (Gross Written Premium):** `SUM(Annual_Premium_KES)`
    * **Loss Ratio %:** `DIVIDE([Total Claims], [Total GWP], 0)`
    * **Combined Ratio %:** `[Loss Ratio %] + 0.30` (Factoring in 30% operational overhead).

### 3. Statistical Analysis
* **Frequency-Severity Matrix:** Utilized scatter plots to categorize risks into "Nuisance" (High Frequency/Low Severity) vs. "Catastrophic" (Low Frequency/High Severity) clusters.

---

## Key Insights & Business Value

* **Geographic Risk Benchmarking:** Identified that **Nakuru, Nairobi, and Mombasa** consistently exceed the **70% Target Loss Ratio**, suggesting a need for localized underwriting adjustments or targeted premium hikes.
* **Profitability Distribution:** While 68% of the portfolio is profitable, a significant portion of the **PSV and Taxi** segments are "Loss Making," indicating that current pricing models do not adequately reflect commercial risk.
* **Risk Segmentation:** The analysis revealed that specific accident causes, such as **Theft**, drive higher severity in specific counties, allowing the insurer to offer targeted security-based discounts or telemetry requirements.

---

## 📂 Repository Structure

| File | Description |
| :--- | :--- |
| `Kenya_Insurance_Analysis_Cleaned.csv` | The final processed dataset used for visualization. |
| `insurance analysis.ipynb` | Python source code for data cleaning and feature engineering. |
| `Motor_Insurance Risk &u Underwriting performance Dashboard Analytics.pbix` | The source Power BI file containing all DAX measures and visuals. |

---

## 📈 About Me
I am a **Statistician** specializing in turning complex datasets into actionable business strategies. My work focuses on the intersection of data science, actuarial logic, and financial services.

**Let's Connect:**
* [LinkedIn](www.linkedin.com/in/petermunyalo)
  

---
*Disclaimer: This project uses simulated insurance data for analytical demonstration purposes.*
