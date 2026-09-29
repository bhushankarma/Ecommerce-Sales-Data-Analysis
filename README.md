# E-Commerce Sales Data Analysis

## Project Overview

This project focuses on analyzing e-commerce sales data to understand business performance, sales trends, profitability, and product performance.

The project started with the original **Superstore.csv** dataset. Initial data exploration and analysis were performed on the original dataset. After that, the dataset was modified and additional useful fields were created, resulting in the final **superstore_modified_dataset.csv** dataset.

The final dataset was then used for detailed analysis and an interactive Power BI dashboard.

Python and Pandas were used for data preparation and analysis, Matplotlib was used for visualization, and Microsoft Power BI with DAX was used to create the interactive dashboard.

---

## Project Objectives

* Analyze sales and profit performance
* Understand sales trends over time
* Compare performance across categories and regions
* Analyze segment and sub-category performance
* Identify top-selling products
* Identify loss-making products
* Create interactive business dashboards
* Generate meaningful business insights from data

---

## Technologies Used

### Python

* Pandas
* Matplotlib

### Data Visualization & BI

* Microsoft Power BI
* DAX

### Data Format

* CSV

---

## Project Workflow

```text
Original Superstore.csv
          ↓
Initial Data Exploration & Analysis
          ↓
Dataset Modification
          ↓
Feature Creation
          ↓
superstore_modified_dataset.csv
          ↓
Data Analysis
          ↓
Power BI Dashboard
          ↓
DAX Measures / KPIs
          ↓
Interactive Analysis
          ↓
Business Insights
```

---

## Dataset

### Original Dataset

The project initially used the original **Superstore.csv** dataset for data exploration and analysis.

### Modified Dataset

After the initial analysis, the dataset was modified and additional analytical fields were created.

The final dataset is:

**`superstore_modified_dataset.csv`**

The final dataset contains:

* **9,994 records**
* **26 columns**

Additional fields created during data preparation include:

* Shipping Days
* Year
* Month
* Quarter
* Month Name

---

## Data Preparation & Validation

The dataset was checked and prepared before performing the final analysis.

The following checks were performed:

* Checked dataset structure and columns
* Checked data types
* Checked missing values
* Checked duplicate records
* Validated Sales values
* Validated Quantity values
* Validated Shipping Days
* Created additional analytical fields

### Data Quality Results

* Duplicate records: **0**
* Invalid Sales values: **0**
* Invalid Quantity values: **0**
* Invalid Shipping Days: **0**

Negative Profit values were retained because they represent actual business losses and are important for profitability analysis.

---

## Power BI Dashboard

The final dataset was imported into Microsoft Power BI to create an interactive dashboard.

The dashboard contains three pages:

### 1. Overview

The Overview page provides a high-level summary of business performance.

Key KPIs:

* Total Sales
* Total Profit
* Total Orders
* Total Quantity
* Profit Margin %

Visualizations:

* Sales Trend Over Time
* Sales by Category
* Profit by Region

---

### 2. Detailed Analysis

This page provides a more detailed analysis of sales and profitability.

Visualizations:

* Sales by Segment
* Profit by Sub-Category
* Top 10 Products by Sales
* Loss-Making Products

---

### 3. Interactive Analysis

This page allows users to interactively filter the dashboard.

Slicers:

* Year
* Region
* Category
* Segment
* Ship Mode

Key KPIs:

* Total Sales
* Total Profit
* Total Orders
* Profit Margin %

Visualizations:

* Sales by Category
* Profit by Category

The slicers dynamically update the KPIs and visualizations based on the selected filters.

---

## DAX Measures

The following DAX measures were created in Power BI.

### Total Sales

```DAX
Total Sales = SUM('superstore_modified_dataset'[Sales])
```

### Total Profit

```DAX
Total Profit = SUM('superstore_modified_dataset'[Profit])
```

### Total Quantity

```DAX
Total Quantity = SUM('superstore_modified_dataset'[Quantity])
```

### Total Orders

```DAX
Total Orders = DISTINCTCOUNT('superstore_modified_dataset'[Order ID])
```

### Profit Margin %

```DAX
Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)
```

### Average Order Value

```DAX
Average Order Value = DIVIDE([Total Sales], [Total Orders], 0)
```

---

## Key Business Insights

### Category Performance

* Technology generated the highest sales among the three categories.
* Technology also generated the highest profit.
* Furniture generated substantial sales but comparatively lower profit.

### Regional Performance

* The West region generated the highest profit.
* The Central region generated the lowest profit.

### Sub-Category Performance

* Copiers generated the highest profit among the sub-categories.
* Tables had the highest loss.
* Bookcases and Supplies also showed negative profit.

### Top-Selling Products

The **Canon imageCLASS 2200 Advanced Copier** had the highest sales among the analyzed top 10 products.

### Loss-Making Products

The **Cubify Cubex 3D Printer Double Head Print** had the highest loss among the analyzed loss-making products.

---

## Project Outcome

This project helped analyze e-commerce sales and profitability from multiple business perspectives, including:

* Categories
* Regions
* Segments
* Sub-Categories
* Products
* Time periods

The interactive Power BI dashboard makes it easier to explore business performance using different filters and KPIs.

The analysis identified high-performing categories and regions, top-selling products, and loss-making products.

---

## Future Improvements

Possible future improvements include:

* Add advanced time-series analysis
* Analyze the relationship between discounts and profit
* Add customer-level analysis
* Add forecasting features
* Add more detailed profitability analysis
* Add drill-through analysis

---

## Author

**Bhushan Karma**

B.Tech Computer Science & Engineering Student

Interested in Data Analytics, Business Intelligence, and Data Science.
