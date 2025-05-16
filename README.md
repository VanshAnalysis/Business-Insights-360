# ![icons8-360-48 (1)](https://github.com/user-attachments/assets/cd652607-08aa-4a67-8994-83fef1e98b8d) Business Insights 360  
## 🏬 Company Overview

AtliQ Hardware(imaginary company) is a rapidly growing electronics company specializing in hardware products, including PC accessories, printers, and more. Over the years, AtliQ has expanded significantly, establishing a strong global presence in key regions such as APAC, North America, Latin America, and the European Union.

The company distributes its products through two primary sales platforms:
- Brick-and-Mortar Stores – Partnering with physical retail outlets like Croma and Best Buy.
- E-Commerce Platforms – Selling through online giants like Amazon and Flipkart.

Moreover, AtliQ operates through multiple sales channels:
- Retailers – Third-party sellers, both online and offline, that stock and sell AtliQ’s products.
- Direct Stores – AtliQ’s own branded stores, where consumers can purchase directly.
- Distributors – In restricted markets like China and South Korea, AtliQ collaborates with large distributors to ensure product availability.

**Note:** AtliQ’s customers are retailers and distributors, while the consumers are the end users.

## 🔎 Problem Statement

AtliQ Hardware has been relying on scattered Excel sheets for analytics, which has resulted in inefficient decision-making and significant losses—especially during its expansion in Latin America. In contrast, competitors using advanced data analytics have gained a competitive edge, leaving AtliQ struggling to keep pace with outdated methods. To address these challenges, AtliQ has launched a data analytics project aimed at improving transparency, enhancing decision-making, and driving strategic growth.

## 🎯 Project Objective

To develop an intuitive dashboard that delivers actionable insights for finance, sales, marketing, and supply chain teams, along with an executive and key performers view. This will enhance transparency, improve data accessibility, and empower stakeholders to make informed, data-driven decisions for strategic growth and efficiency.

## 🛢 Data Overview

AtliQ Hardware has provided two SQL databases and three Excel files for analysis.  

The three Excel files are:
- Operating Expenses
- Targets (available only for FY 2022)
- Market Share (limited to the Personal Computer division)

The two databases contain the following tables:  

- gdb041:
  - Fact tables: fact_forecast_monthly, fact_sales_monthly
  - Dimension tables: dim_customer, dim_market, dim_product

- gdb056:
  - Contains freight_cost, gross_price, manufacturing_cost, post_invoice_deductions, and pre_invoice_deductions

AtliQ’s fiscal year runs from September to August, and the dataset covers actual sales from September 1, 2017, to December 31, 2021.

## 🧹️ Data Cleaning & Transformation

#### Standardized & Trimmed Data:
- Removed leading and trailing spaces from text fields.
- Standardized naming conventions for consistency.

#### Data Structuring & Optimization:
- Created a dim_date table for better time-based analysis.
- Merged fact_sales_monthly and fact_forecast_monthly into a single table, fact_actual_estimates, to simplify calculations.
- Added calculated fields in fact_actual_estimates using data from relevant tables (e.g., deriving pre-invoice deductions using percentage values from the pre_invoice_deductions table).
- Disabled load for tables that were used to derive calculations in fact_actual_estimates to optimize performance and reduce the Power BI report size.

## 📑 Report Inclusions  
This repository includes a PDF version of the Power BI report hosted on the Power BI Service, along with its underlying data model. Below, you’ll find a screenshot of the data model and a PDF of the report for a quick preview.

- [Dashboard](https://github.com/VanshAnalysis/Business-Insights-360/blob/main/BI%20360.pdf)
- [Data Model](https://github.com/VanshAnalysis/Business-Insights-360/blob/main/Data%20Modeling.png)

## 🛠️ Tools Used:  
**Data Cleaning & Transformation:** Power Query  
**Data Visualization:** Power BI  
**Data Analysis:** DAX

## 🌐 Goal for project:

- Target is to enlarge the sales in a proper manner that can forecast the events in future for betterment.
- The aim is to manage the difficulty faced by business to achieve higher Income.💰

## 📝 Recommendations

- Once a strong market position is secured, gradually scale back operational and marketing expenditures to boost net profit margins.
- Transition from a flat-rate post-discounting model to a performance-based pricing strategy tailored to individual products and customer segments across markets.
- Strengthen distribution channels and implement targeted marketing efforts in high-growth areas, particularly within the APAC region—especially India.
- Reassess the pricing model or cost structure of the Notebook category to enhance overall profitability.
- Analyze the reasons behind the USB flash drives’ weak performance and consider strategic actions such as repositioning, discontinuation, or redesign.
- Create region-specific initiatives to grow market share in North America.
- Fine-tune marketing budgets in the UK and Germany to ensure higher return on investment.
- Align inventory management and promotional strategies with the seasonal sales peak from September to December to fully capitalize on increased demand.


## 🧠 Skills Gained

- Enhanced expertise in analyzing key business metrics and their direct correlation to organizational performance.
- Created intuitive, data-driven Power BI dashboards tailored to end-user needs, enabling actionable insights.
- Built cross-functional business acumen across finance, sales, marketing, and supply chain, understanding their interdependencies and impact on strategic outcomes.
- The project helps me to learn many advanced and latest use of visuals and gain the idea to acknowledge about the Domain.
