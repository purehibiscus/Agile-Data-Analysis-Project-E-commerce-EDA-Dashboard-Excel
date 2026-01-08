# Agile-Data-Analysis-Project-E-commerce-EDA-Dashboard-Excel


**Agile Data Analytics Project – Excel Sales Performance Dashboard**

**Project Overview**


This project demonstrates an **end-to-end Agile data analytics workflow**, from project planning and backlog management in **Trello**, through **data cleaning, EDA, dashboard wireframing, development, review, and approval**, using **Microsoft Excel and Power Query.**

The objective was to analyze a transactional sales dataset and deliver **actionable business insights** via a stakeholder-ready dashboard, while strictly following **Agile project management practices.
**

**Agile Project Management Approach**

The project followed a **Scrum-style Agile framework** implemented in Trello, with the following workflow:

**Product Backlog → Sprint Backlog → To Do → In Progress → Review → Done**

Each card represented a deliverable (EDA, data cleaning, KPI design, dashboard visuals, validation), with:

1. Clearly defined acceptance criteria
2. Checklists tracked only during In Progress
3. Review gate for validation before approval


**Dataset & Tools**

**Dataset:** CSV (20,000 transactional rows)
**Tools Used:**

1. Microsoft Excel
2. Power Query
3. Pivot Tables
4. Excel Formulas
5. Trello (Agile Project Management)

**Data Preparation & Governance
**

1. Imported CSV into Excel and validated 20,000 rows
2. Converted numeric fields to correct data types (currency, numeric, date)
3. Validated and standardized:

i. Sales amounts
ii. Ratings (converted from text to numeric, 1 decimal)
iii. Date fields
4. Identified no duplicate records

**Missing Data Handling**

Add-ons Purchased column had **27% missing values**
Addressed using **Power Query Fill Down**, chosen to:

1. Preserve hierarchical relationships
2. Avoid manual data distortion
3. Enable scalable grouping, sorting, and joins


**Feature Engineering**

Derived and validated new columns:
- Date_Year
- Date_Quarter (prefixed with “Q”)
- Date_Month

**Category Transformation**
1. Duplicated Add-ons Purchased column
2. Split text using delimiter in Power Query
3. Removed suffixes and normalized categories
4. Renamed transformed column to Category

**Transaction Value Calculation**

1. Created Order Value per Transaction
2. Formula includes:

  - Total Price + Add-on Total
3. Validated for completeness, accuracy, and governance compliance

**Descriptive Statistics Summary**

Analyzed:
1. Age
2. Total Price
3. Quantity

Metrics included:

1. Mean, Median, Mode
2. Standard Deviation & Variance
3. Skewness & Kurtosis
4. Z-score analysis for distribution understanding

**Exploratory Data Analysis (EDA)**

1. Overall Business Performance
  i. Total Revenue: $64.8M
  ii. Total Orders: 20,000
  iii. Unique Customers: 6,637
  iv. Average Order Value (AOV):
  v. Avg Unit Price: $578.63
  vi. Avg Transaction Value: $3,180.13
2. Order Status Impact:
i. Completed: 13,432 orders | $43.4M
ii. Cancelled: 6,568 orders | $21.3M

2. Time-Series Analysis
  i. Monthly revenue trends (Jan–Sep > $6M/month)
  ii. Quarterly analysis:
  iii. Q1–Q3 contributed 85%+ of revenue
  iv. Q4 significantly underperformed
3. Identified peak and lowest revenue months

3. Product Performance
- Top Revenue Product: Smartphone ($21.8M, 33% of revenue)
- Followed by:
  i. Smartwatch ($14M)
  ii. Laptop ($12M)
  iii. Tablet ($11M)
  iv. Headphones ($4M)

4. SKU-level quantity analysis (>10,000 units per group)
5. Product-level AOV analysis
6. Identified low-performing products for optimization

**4. Customer Behavior Analysis**

  i. Repeat purchase customers: 12,127
  ii. Repeat purchase rate: 16%
  iii. Top 5 customers contributed up to $35K each
  iv. Loyalty vs Non-loyalty comparison:
    - Loyal customers: $13.9M revenue | AOV $3.2K
    - Non-loyal customers: $50.9M revenue | AOV $3.2K

**5. Payment & Order Behavior**

  i. Revenue by payment method:
    - PayPal & Credit Card: ~$19M each
    - Bank Transfer: ~$12M
ii. Shipping preference:
  - Standard shipping most preferred (>6.7K orders)
  - Order completion vs cancellation impact quantified

**6. Pricing, Quantity & Add-on Analysis**

i. Transaction value segmentation:
  - High (> $8K)
  - Medium ($4K–$8K)
  - Low (< $4K)
ii. Quantity grouped into 10 bands
iii. Add-on revenue contribution:
  - Impulse items led add-on revenue ($425K)
  - Strong correlation with high-value orders

**7. Data Quality Validation**
i. Missing values handled
ii. Duplicate checks performed
iii. Pricing validation
iv. Outliers and anomalies reviewed
v. Dataset confirmed analysis-ready

**Dashboard Design & Development**

1. KPI-driven layout
2. Business-question-first design
3. Interactive filters:
  - Date, Product, Loyalty, Order Status
4. Excel visuals:
  - KPI cards
  - Trend charts
  - Category and product comparisons
5. All KPIs validated against EDA outputs

**Review & Approval**

1. KPIs reconciled with source data
2. Filters tested
3. Visuals validated
4. Stakeholder acceptance simulated

Project status: **DONE**
