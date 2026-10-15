**Project:** Excellent Stores — Sales Analytics Dashboard
**Tool:** Microsoft Power BI
**Focus Areas:** Data Cleaning, Data Modeling, DAX, KPI Reporting, Sales Analysis, and Interactive Visualization

## Project Overview

This project analyzes sales performance for **Excellent Stores**, a supermarket chain operating across multiple cities in the United States. The Power BI dashboard helps management understand sales turnover across locations and evaluate product profitability.

## Objectives

- Monitor total sales, net sales, costs, net profit, and profit percentage.
- Compare sales and profitability across regions, states, categories, sub-categories, products, and customer segments.
- Compare current sales with previous-year performance and evaluate sales targets.
- Identify top-performing products and their contribution to overall sales.
- Analyze trends using average sales, moving averages, cumulative sales, and year-to-date/month-to-date measures.

## Tools and Technologies

- **Power BI Desktop** — Dashboard development and data modeling
- **Power Query** — Data cleaning, transformation, and combining yearly sales files
- **DAX** — Calculated measures, time intelligence, rankings, and target calculations
- **Interactive Visualizations** — Slicers, drill-down hierarchies, bookmarks, What-if parameters, and page navigation

## Data Preparation and Modeling

The project uses customer, product, people, and regional dimension data, yearly sales transaction files, and sales returns data.

Key data preparation steps include:

- Combined yearly sales transaction files into a single `SalesRecords` table.
- Removed rows with null Order IDs from `SalesRecords` and null Customer IDs from the Customers table.
- Promoted the appropriate headers in the product table.
- Removed null rows and columns from the People table.
- Integrated sales return information into `SalesRecords` and replaced null return flags with `False`.
- Created a dedicated `MyMeasures` table to organize DAX measures.
- Created a DAX calendar table containing dates, years, months, and month names.
- Configured month sorting and data model relationships as specified in the project requirements.
  
## Key DAX Measures

The dashboard includes the following measures and calculations:

- Total Sales, Net Sales, Net Cost, Net Profit, and Profit %
- Average Sales and Moving Average Sales
- Last Year Sales and cumulative sales comparisons
- Top 3 Products Total Sales and Top 3 Share
- Year-to-Date (YTD) and Month-to-Date (MTD) Sales
- Top 3 Customer Sales
- Target Sales based on a user-selected percentage

## Dashboard Pages

### 1. Sales and Profitability Overview

- Total profit by geographic location with drill-down capabilities.
- Total sales and profit percentage by customer segment.
- Total profit by category, sub-category, and product.

### 2. Sales Trends and Shipping
- Average sales by date.
- Moving average sales to identify underlying trends.
- Profit distribution by shipping mode.
- Profit percentage by sub-category.

### 3. Sales Performance
- KPI cards for total sales, total cost, and profit percentage.
- Current-month sales compared with last-year sales.
- Sales distribution by category and region.
- Monthly sales versus previous-year sales.

### 4. Top Products Analysis
- Total sales and overall sales share of the top three products.
- Top 10 products ranked by sales.
- Bookmark-based views for Top 5, Top 8, and Top 12 products.

### 5. Sales Target Analysis
- Monthly sales and target sales comparison.

### 6. Customer Segment Analysis - Consumer
- KPI cards for total sales, total cost, and profit percentage.
- Current-month sales compared with last-year sales.
- Sales distribution by category and region.
- Monthly sales versus previous-year sales.

### 7. Customer Segment Analysis - Corporate Sales
- KPI cards for total sales, total cost, and profit percentage.
- Current-month sales compared with last-year sales.
- Sales distribution by category and region.
- Monthly sales versus previous-year sales.

### 6. Customer Segment Analysis - Home Office
- KPI cards for total sales, total cost, and profit percentage.
- Current-month sales compared with last-year sales.
- Sales distribution by category and region.
- Monthly sales versus previous-year sales.

## Interactive Features
- Year, Region, and Category slicers across report pages.
- Synchronized filtering between pages.
- Drill-down functionality for geographic and product analysis.
- Bookmarks for switching between Top 5, Top 8, and Top 12 product views.
- What-if parameters for dynamic sales target analysis.
- Navigation icons for Home, Previous, and Next pages.

## Business Value
The dashboard consolidates sales, profitability, regional performance, product contribution, and target comparisons into an interactive reporting solution. It enables users to explore trends, compare performance, identify profitable product categories, and support data-driven business decisions.
