# BlinkIT-Sales-Analysis
Data Analytics project analyzing BlinkIT sales using Excel, Power BI, and DAX to uncover sales drivers, outlet performance, customer trends, and actionable business insights through interactive dashboards.

## Project Overview

This project focuses on analyzing BlinkIT sales performance using Excel and Power BI to identify key business drivers and generate actionable recommendations for improving sales performance.

The analysis covers outlet performance, item categories, pricing patterns, visibility impact, outlet size, and location-based sales trends.

## Business Problem

BlinkIT operates through multiple outlet formats across different locations and sizes.

The objective of this project is to analyze:

- Which outlet types generate the highest sales
- Which product categories perform best
- Which outlet tiers contribute maximum revenue
- Which pricing ranges drive the most sales
- How outlet size impacts performance
- Areas where business improvements can be made

## Dataset Information

- **Dataset Source:** Tableau Public Dataset
- **Rows:** 8,525
- **Columns:** 12
- **Industry:** E-commerce / Retail

### Important Features

| Column Name | Description |
|-------------|-------------|
| Item_Type | Product category |
| Item_MRP | Product price |
| Item_Visibility | Product visibility |
| Outlet_Type | Type of store |
| Outlet_Size | Store size |
| Outlet_Location_Type | Tier location |
| Outlet_Establishment_Year | Store establishment year |
| Item_Outlet_Sales | Sales generated |

## Tools Used

### Excel
- Data Cleaning
- Missing Value Handling
- Flash Fill
- Conditional Formatting
- INDEX + FILTER
- XLOOKUP
- INDEX MATCH

### Power BI
- KPI Cards
- DAX Measures
- Data Modeling
- Slicers
- Drill Through
- Bookmarks
- Interactive Dashboard
- Data Visualization.

## Data Cleaning Process

The following preprocessing steps were performed in Excel:

### Missing Values Handling

#### Outlet Size
Missing values were filled by identifying patterns between:

- Outlet Type
- Tier Location

Using repeated combinations to infer the most suitable store size.

Example:

- Grocery Store → Small
- Supermarket Type 1 + Tier 2 → Small

A total of multiple combinations were explored.

#### Item Weight

Missing item weights were handled using Item Identifier logic.

Since each product identifier should ideally have a fixed weight, the following formula was used:

```excel
=INDEX(FILTER(B:B,(A:A=A2)*(B:B<>"")),1)
```

If an item identifier contained only blank values, average imputation was applied.

#### Standardization

Values in Outlet Size were standardized:

```text
High → Big
```

for better readability and consistency.

## Key KPIs

| KPI | Value |
|------|------|
| Total Sales | ₹18.59M |
| Total Items | 8.52K |
| Total Outlets | 10 |
| Average Sales | ₹1.86M |

## Dashboard Visualizations

The dashboard contains:

- KPI Cards
- Line & Clustered Column Charts
- Pie Charts
- Treemap
- Clustered Column Charts
- Interactive Tables
- Slicers

### Key Analysis Areas

- Outlet Type Performance
- Tier-wise Sales
- Store Size Analysis
- Product Fat Content
- Sales by Establishment Year
- Price Range Contribution
- Product Category Demand

## Key Insights

### Outlet Performance
- Supermarket Type 3 generated the highest average sales.
- Supermarket Type 1 contributed the highest total sales.
- Grocery Stores generated the lowest sales contribution.

### Tier Analysis
- Tier 3 locations generated the highest total sales.

### Outlet Size
- Small outlets generated the highest total sales.
- Medium outlets showed stronger average sales efficiency.

### Product Pricing
- Products in the ₹150–₹200 range contributed the highest revenue.

### Customer Preference
- Low-fat products demonstrated stronger purchasing demand.

### Product Demand
High-demand categories include:

- Seafood
- Breakfast
- Starchy Foods

## Business Recommendations

### Store Expansion Strategy
Focus expansion on high-performing outlet formats such as:

- Supermarket Type 2
- Supermarket Type 3

especially in Tier 2 and Tier 3 regions.

### Inventory Optimization
Increase inventory for high-demand categories:

- Seafood
- Breakfast
- Starchy Foods

### Pricing Strategy
Prioritize inventory around products in the ₹150–₹200 MRP segment.

### Outlet Performance Review
Conduct deeper profitability analysis for low-performing grocery outlets before expansion decisions.

## Skills Demonstrated

- Data Cleaning
- Data Transformation
- Exploratory Data Analysis
- Business Intelligence
- Dashboard Design
- Data Visualization
- Business Recommendation
- Power BI
- Excel Analytics
- DAX

## Future Improvements

- Add SQL-based analysis
- Perform visibility vs sales correlation analysis
- Add profit analysis
- Add forecasting model
- Create customer segmentation

## Author

**Vignesh Tripathi**

Aspiring Data Analyst passionate about data visualization, business analytics, and problem solving.

Connect with me on LinkedIn.
www.linkedin.com/in/vigneshtripathi

Snapshot of project : ![Dashboard Preview].(https://github.com/Vignesh-hub107/BlinkIT-Sales-Analysis/blob/main/Images/Full_img.png).
