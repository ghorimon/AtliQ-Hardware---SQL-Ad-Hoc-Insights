# 📊 Atliq Hardware SQL Analytics Project

<div align="center">

![SQL](https://img.shields.io/badge/SQL-Advanced-blue?style=for-the-badge&logo=mysql)
![Status](https://img.shields.io/badge/Status-Complete-success?style=for-the-badge)
![Business](https://img.shields.io/badge/Domain-Consumer_Electronics-orange?style=for-the-badge)

*Transforming raw data into actionable business intelligence through SQL*

[View Queries](#-sql-queries) • [Report Bug](#) • [Request Feature](#)

</div>

---

## 🎯 Project Overview

This project delivers **data-driven insights** for **Atliq Hardware**, a leading global consumer electronics company. Through advanced SQL analytics, I've answered critical business questions spanning sales performance, product portfolio analysis, customer segmentation, and operational efficiency.

The goal: empower stakeholders with **ad-hoc analytical reports** to make informed decisions across sales, finance, and supply chain departments.

## 🏢 Business Context

Atliq Hardware operates in competitive international markets with:
- **Diverse product portfolio** spanning multiple categories and segments
- **Multi-channel distribution** (Retail, E-commerce, Direct)
- **Global customer base** across regions like APAC, EU, NA, and LATAM
- **Complex pricing structures** with pre-invoice deductions and manufacturing costs

Decision-makers need quick, accurate answers to strategic questions—this project provides exactly that.

## 🗄️ Database Schema

**Database:** `gdb023`

The relational database consists of six interconnected tables:

| Table | Description | Key Fields |
|-------|-------------|------------|
| `dim_customer` | Customer master data | customer_code, customer, region, market, channel |
| `dim_product` | Product catalog | product_code, product, segment, division, variant |
| `fact_gross_price` | Pricing by fiscal year | product_code, fiscal_year, gross_price |
| `fact_manufacturing_cost` | Production costs | product_code, cost_year, manufacturing_cost |
| `fact_pre_invoice_deductions` | Discount percentages | customer_code, fiscal_year, pre_invoice_discount_pct |
| `fact_sales_monthly` | Monthly sales transactions | customer_code, product_code, fiscal_year, sold_quantity |

## 🔍 Business Questions Solved

### 1️⃣ Market Analysis
**Q:** Provide the list of markets in which customer "Atliq Exclusive" operates in the APAC region.

*Insight: Understand regional market penetration*

---

### 2️⃣ Product Growth Analysis
**Q:** What is the percentage of unique product increase in 2021 vs. 2020?

*Insight: Measure product portfolio expansion*

---

### 3️⃣ Segment Distribution
**Q:** Provide a report with unique product counts for each segment, sorted in descending order.

*Insight: Identify high-volume product segments*

---

### 4️⃣ Segment Growth Leader
**Q:** Which segment had the most increase in unique products in 2021 vs 2020?

*Insight: Spot fastest-growing product categories*

---

### 5️⃣ Cost Extremes
**Q:** Get the products with the highest and lowest manufacturing costs.

*Insight: Optimize cost management strategies*

---

### 6️⃣ Customer Discount Analysis
**Q:** Generate a report with the top 5 customers who received the highest average pre-invoice discount percentage in 2021 (India market).

*Insight: Evaluate discount strategies and customer relationships*

---

### 7️⃣ Sales Trend Analysis
**Q:** Get the complete report of Gross sales amount for the customer "Atliq Exclusive" for each month.

*Insight: Track monthly revenue performance*

---

### 8️⃣ Quarterly Performance
**Q:** In which quarter of 2020 was the maximum total sold quantity?

*Insight: Identify seasonal demand patterns*

---

### 9️⃣ Channel Contribution
**Q:** Which channel helped bring the most gross sales in 2021 and what was the percentage of contribution?

*Insight: Optimize channel investment allocation*

---

### 🔟 Top Products by Division
**Q:** Get the Top 3 products in each division with the highest total_sold_quantity in 2021.

*Insight: Recognize star performers across divisions*

## 🛠️ Technical Skills Demonstrated

- **Advanced SQL Queries**: Complex multi-table joins, subqueries, CTEs
- **Aggregate Functions**: SUM, COUNT, AVG with GROUP BY
- **Window Functions**: ROW_NUMBER, RANK, DENSE_RANK
- **Conditional Logic**: CASE statements for business rules
- **Date Operations**: Fiscal year calculations and time-series analysis
- **Performance Optimization**: Efficient query design for large datasets

## 📂 Project Structure
```
atliq-hardware-sql-project/
│
├── queries/
│   ├── 01_market_analysis.sql
│   ├── 02_product_growth.sql
│   ├── 03_segment_distribution.sql
│   └── ... (all 10 queries)
│
├── results/
│   ├── output_screenshots/
│   └── summary_report.pdf
│
├── database/
│   └── schema_diagram.png
│
└── README.md
```

## 🚀 Getting Started

### Prerequisites
- MySQL 8.0 or higher
- Access to the `gdb023` database

### Running the Queries

1. Clone the repository
```bash
git clone https://github.com/ghorimon/atliq-hardware-sql-project.git
```

2. Connect to your MySQL database
```bash
mysql -u ghorimon -p
```

3. Use the database
```sql
USE gdb023;
```

4. Execute individual queries from the `queries/` folder

## 💡 Key Insights Delivered

✅ Identified high-value customer segments for targeted marketing  
✅ Revealed product portfolio gaps and growth opportunities  
✅ Optimized discount strategies based on data-driven thresholds  
✅ Uncovered seasonal trends to improve inventory planning  
✅ Determined most profitable sales channels for resource allocation  

## 📈 Impact

This project demonstrates how **SQL-driven analytics** can transform raw transactional data into strategic business intelligence, enabling:
- Faster decision-making
- Data-backed strategy formulation
- Operational efficiency improvements
- Revenue optimization opportunities

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## 📧 Contact

**Rimon Ghosh**  
📧 rimonsarbajitghosh@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/ghorimon)  
💼 [Portfolio](https://codebasics.io/portfolio/Rimon-Ghosh)

---

<div align="center">

**⭐ If you found this project helpful, please give it a star!**

Made with ❤️ and SQL

</div>
