# 📊 Sales Performance Analysis (Excel)

<p align="center">
  <img src="images/Sales Analysis - Overview.png" width="500">
</p>

## 🚀 Project Overview

This project analyses sales performance for a Superstore retail business to understand what drives revenue growth and where sales efficiency breaks down using historical sales data.

While the business shows consistent year-over-year sales growth, profit trends indicate that not all sales contribute equally to sustainable revenue.

An interactive Excel dashboard was built to analyse sales trends, discount dependency, and loss-making orders. Scenario-based analysis was then used to evaluate ways to improve revenue quality without reducing overall sales volume.

---

## 🎯 Business Problem

The business is growing sales year over year, but profitability fluctuates due to heavy reliance on discounting. The objective was to understand overall sales performance and identify the factors contributing to unstable profitability.

Key questions addressed:

- Which discount levels genuinely support profitable sales growth  
- How discounts and shipping decisions impact outcomes  
- Where loss-making sales practices occur  
- How much revenue could potentially be recovered through policy changes  

---

## 📊 Dataset Overview

- Source: Kaggle - Superstore Sales Dataset
- Time period: 2014-2017
- Order-level data including sales, profit, discount, shipping mode, category, and region

---

## 🧹 Data Cleaning & Preparation

Data cleaning and preparation were carried out using Power Query and Excel.

I began by removing duplicate records to ensure each order was counted only once. Since missing values accounted for less than 1% of the dataset, I removed null values to avoid introducing unnecessary assumptions. I then reviewed the data for inconsistencies, such as irregular entries in categorical fields, and corrected them where required. Date fields were also standardised to ensure consistency for time-based analysis.

Once the data was clean, I created additional analytical columns in Excel. Discount bands were defined using an IFS formula and grouped into:
- No Discount - 0%  
- Low Discount - ≤10%  
- Medium Discount - 11–29%  
- High Discount - ≥30%  

A separate flag column was created to identify **loss-making orders**, enabling targeted efficiency analysis.

---

## 💡 Analysis & Calculations

After preparing the dataset, I performed EDA analysis by using pivot tables and calculated fields for the analysis. Key metrics calculated included:

Discounted sales

Number of loss-making orders

Discount dependency

Year-over-year sales growth

Profit and loss contribution by discount level, region, and shipping modes.

These calculations formed the basis for identifying sales inefficiencies and revenue leakage.

---

## 📈 Key Findings

- Sales show consistent year-over-year growth  
- Technology is the highest revenue-generating category  
- **Over 50% of orders rely on discounts**  
- Low (≤10%) and medium (11–29%) discounts drive sales while remaining largely profitable  
- **High discounts (≥30%) frequently result in loss-making orders**  
- **Profit percentage fluctuates despite increasing sales**  
- High discounts combined with certain shipping modes significantly amplify losses  
- The Central region (2017) shows a concentration of inefficient sales  

---

## 📊 Dashboard Design

Insights were visualised using charts, KPIs, slicers, and navigation buttons in Excel.

Interactive slicers allow filtering by:
- Year  
- Region  
- Category  
- Discount band  

Navigation buttons enable movement between dashboard pages.

### Overall Sales Analysis Page

Focuses on revenue trends, profit behaviour, and discount usage across regions and categories. It shows that sales growth has been steady while profitability remains inconsistent.
<p align="left">
  <img src="images/Sales Analysis - Overview.png" width="800">
<p align="right">
  <img src="images/Sales Analysis - Light.png" width="500">
</p>

---

### Loss Drivers Page

Focuses on sales efficiency and loss drivers, including:

- Loss-making orders by discount band  
- Discount × shipping mode interaction  
- Regional concentration of inefficient sales  
- Identification of high-risk discount ranges
  
<p align="center">
  <img src="images/Sales Analysis - Loss Drivers.png" width="800">
</p>

---

## 🔮 Scenario & What-If Analysis

What-If analysis was conducted to estimate potential revenue recovery from reducing high-risk discounts (>30%).

Excel What-If Data Tables were used to simulate multiple reduction scenarios.

Results indicate:

- Reducing high discounts by **20–30%** could recover approximately **4–6% of revenue**  
- Assumes demand shifts toward historically effective low and medium discounts  
- Combining discount controls with restricted premium shipping eligibility further improves recovery potential  

Together, these measures could recover **~10% of revenue currently lost** due to inefficient discounting and shipping decisions.

These results are scenario-based and intended to guide decisions, not predict outcomes.

---

## 📈 Revenue Recovery Scenarios

| % Reduction in High Discounts | Recoverable Revenue | Revenue Impact % |
|------------------------------|---------------------|------------------|
| 10% | 17,661.96 | 1.6% |
| 15% | 26,492.94 | 2.4% |
| 20% | 35,323.92 | 3.2% |
| 25% | 44,154.90 | 4.0% |
| 30% | 52,985.88 | 4.8% |
| 40% | 70,647.84 | 6.4% |

---

## ✅ Recommendations

- Cap discounts for low-margin products  
- Restrict high-discount orders to cost-efficient shipping modes  
- Continue controlled use of low and medium discount ranges  
- Monitor loss-making orders using rule-based indicators  

---

## 🛠️ Tools Used

- Microsoft Excel — Pivot Tables, Charts, Slicers  
- Power Query — data cleaning and transformation  
- What-If & Scenario Analysis  
- Trend analysis and basic forecasting  

---

## ⚠️ Notes

- Dataset: Superstore Sales (Kaggle)  
- Scenario outputs are assumption-based  
- Focus is on sales efficiency and revenue quality, not demand forecasting  

