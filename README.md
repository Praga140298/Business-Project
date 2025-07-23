# Business-Project
Data Analysis for Business in sales project

Welcome to the complete end-to-end analysis project focused on uncovering trends, optimizing profitability, and guiding strategic decisions based on historical U.S. regional sales data. This project integrates statistical modeling, exploratory analysis, and interactive dashboards.

**Tools Used:** Python, Pandas, YData-Profiling, Power BI, Excel

**Dataset:** 5 years of sales transactions, customer segments, product SKUs, and budgets

**Objective:** Drive actionable insights for sales, finance, and executive stakeholders

**Business Problem**
Despite strong revenue figures, Acme USA experiences inconsistent performance across U.S. regions. Leadership lacks visibility into seasonal trends, top-performing products, and high-margin channels.

**Business Question:**
How can historical data be leveraged to identify revenue drivers, optimize product/channel mix, and guide strategic planning across states and regions?

**Project Workflow**
Data Ingestion → Preprocessing → Feature Engineering → EDA → Insights → Power BI Dashboard → Strategic Recommendations

**Repository Contents**
| File                          | Purpose                                                                        |
| ----------------------------- | ------------------------------------------------------------------------------ |
| `Regional Sales Dataset.xlsx` | Raw dataset containing orders, customers, products, budgets, regions           |
| `Sales_Report.html`           | Automated profiling report using YData for data quality and summary statistics |
| `sales_Report_file.csv`       | Cleaned and feature-engineered dataset used for Power BI modeling              |
| `Business project.pptx`       | Final presentation of findings, insights, and recommendations                  |
| `Business Project.pbix`       | Interactive Power BI dashboard for stakeholder exploration                     |


**Data Understanding & Profiling**

Sales_Report.html: Generated using ydata-profiling (v4.16). It provides:

Descriptive statistics for each column

Correlation heatmaps

Missing values check

Skewness & cardinality detection

**This helped in identifying:**

No missing values or duplicates

Strong correlation between unit price and revenue/profit (0.91–0.87)

Long-tail distribution in order values (AOV)

**Data Preprocessing & Feature Engineering**

**Steps performed:**

Merged multiple tables: Orders, Customers, Products, Budgets, States, Regions

Dropped redundant and unnecessary fields

Standardized naming conventions (snake_case)

**Engineered key columns:**

profit = revenue - cost

profit_margin_pct = profit / revenue

Calendar fields: order_month, order_month_name, etc.

**Final dataset includes 20+ columns categorized as:**

Identifiers: Order ID, Product ID, Customer

Financials: Revenue, Cost, Profit

Geography: State, Region, Latitude, Longitude

Time: Month, Year

Channel, Budget, Quantity

**Exploratory Data Analysis (EDA)**

Conducted in Power BI with the support of CSV data. Key insights include:

**1. Seasonal Trends**

Revenue dips in January; peak in May-June

Outlier drop in Q1 2017

**2. Product Insights**

Top SKUs: Product 26 & 25 (~25% revenue)

Mid-tier products (IDs 5, 13, 14) have potential

Bottom SKUs need price review or discontinuation

**3. Channel Contribution**

Wholesale: 54% of volume

Export: Highest margins (~38%)

Distributor: Moderate sales (~31%)

**4. Geographic Performance**

California leads in revenue ($230M+)

Midwest/Northeast underperform – candidates for marketing push

West Region: Highest fluctuations

**5. Customer Segmentation**

Aibox Company = top client

Bottom 10 customers contribute minimal revenue

High-value clients with poor margin = risk for over-discounting

**6. Financial Correlations**

unit_price ↔ cost ↔ revenue ↔ profit all highly linked

Volume (quantity) plays a secondary role compared to price

Power BI Dashboard (Business Project.pbix)

**Pages:**

Performance Summary – Trends, KPIs, seasonality

Product & Channel Analysis – Margins, top SKUs, pricing insights

Geographic Insights – State-wise maps, order heatmaps, region clusters

Built with bookmarks, slicers, and drill-down capabilities for executive-level decision making.

**Final Recommendations**

****Area	Recommendation****

Seasonal Strategy	Launch targeted campaigns in April, boost January sales
Product Mix	Promote high-margin SKUs (26, 25); review underperformers
Channel Strategy	Expand Export partnerships; renegotiate Distributor pricing
Geographic Focus	Replicate CA success in TX, FL, IL; boost NE marketing
Margin Control	Monitor low-margin large accounts (flag <36%)

**Presentation Highlights**

See Business project.pptx for a story-driven walkthrough:

Problem framing & stakeholder mapping

Clean visuals of trends, product/channel performance

Actionable, data-driven strategies

**For Collaboration**

Open to ideas, questions, or potential improvements in:

RFM-based customer segmentation

Automated insights via Python

🔗 **Let's Connect**
If this project interests you, feel free to:

**Star the repo**

Fork & extend the dashboard

Reach out for data analytics collaboration!

Author: Pragadeesh Narayanasami
Contact: LinkedIn | GitHub

