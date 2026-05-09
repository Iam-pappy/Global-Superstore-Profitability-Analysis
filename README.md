# Global Superstore Profitability Analysis
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)


## 🎯 Business Problem

**Global Superstore's management couldn't identify which products generated high sales but low profit margins.** The result? Inefficient discounting strategies that eroded millions in potential profit.

This project answers: *"Which products look successful but actually harm profitability?"*

## 📊 Key Business Insights

| Insight | Data | Financial Impact |
| :--- | :--- | :--- |
| 🔴 Discounts >20% destroy profit | -61% margin vs +23% for low discounts | **$814,682 LOSS** over 4 years |
| 📱 Top sellers ≠ top profit | 3 of top 10 products have <0% margin | Misaligned sales incentives |
| 🌍 Regional divergence | Western Europe +$218K, Western Africa -$50K | One-size-fits-all strategy fails |

## 📈 Dashboard Preview

<img width="1215" height="678" alt="Screenshot 2026-05-09 010956" src="https://github.com/user-attachments/assets/451e3433-baa6-4e4b-a2cb-95da13728104" />


*Interactive Power BI dashboard with year, Continent, and category filters*

## 💼 Recommendations for Stakeholders

| Priority | Recommendation | Expected Impact |
| :--- | :--- | :--- |
| 1 | Cap discounts at 15% across all products | **+$500K-$800K annual profit** |
| 2 | Add Profit Margin KPI to sales team dashboards | 5-10% profit improvement |
| 3 | Audit Western Africa & Western Asia operations | Turn around $50K+ annual losses |
| 4 | Technology category deep-dive with 10% temp discount cap | Category profitability clarity |


## 🛠️ Tools & Technical Process

### Phase 1: Excel (Data Preparation)
- Cleaned 51,290 rows of sales transaction data
- Handled missing values using Go To Special → Blanks
- Removed duplicate Order IDs
- Created calculated columns:
  - `Profit Margin = Profit/Sales`
  - `Discount Band = IF(Discount>0.2, "High", "Low")`
  - `Year` and `Month` from Order Date
- Built 3 PivotTables addressing business objectives

### Phase 2: Power BI (Interactive Dashboard)
- **DAX Measures Created:**
- Total Sales = SUM(sales[Sales])
Total Profit = SUM(sales[Profit])
Profit Margin % = DIVIDE([Total Profit], [Total Sales])
Avg Discount % = AVERAGE(sales[Discount])

- **Visuals Built:**
- KPI cards for executive overview
- Bar chart: Discount Band comparison
- Line chart: Profit trends by region (48 months)
- Scatter plot: Sales vs Profit by product
- Geographic map with profit color saturation
- **Slicers added:** Year (2012-2015), Continent, Category

### Phase 3: Analysis Framework 
- Project Description (Background, Problem Statement, Scope)
- Objectives (3 answerable business questions)
- Methodology (Tools justified, time frame explicit)
- Insights (Observation → Data → Implication)
- Recommendations (Tied to insights, prioritized)


## 🚀 How to Replicate

### Prerequisites
- Microsoft Excel 2016 or later
- Power BI Desktop (free)

### Quick Start
1. Clone this repository
2. Download Global Superstore dataset from [Kaggle](https://www.kaggle.com/datasets/tahir1413/global-superstore-2016)
3. Open Excel file from `data/processed/` to view pivot tables
4. Open `.pbix` file in Power BI to explore interactive dashboard

## 📫 Connect With Me

![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white) www.linkedin.com/in/saheed-afolabi
![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white) afolabisaheed556@gmail.com

## Author: Afolabi Saheed
## Date: 5/9/2026


