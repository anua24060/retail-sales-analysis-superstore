# Retail Sales Analysis – Superstore Dataset

## Overview
This project performs an end-to-end exploratory data analysis (EDA) on the Superstore dataset to uncover key insights about sales performance, profitability, customer behavior, shipping timelines, and regional trends.  
The goal is to identify business improvement opportunities and provide data-driven recommendations based on the observed patterns.

---

## Dataset Description
The dataset consists of three CSV files:

- **Orders** – Contains details such as Order ID, Product Category, Sales, Profit, Quantity, Discount, Segment, Region, and Shipping information.  
- **Returns** – Contains the list of returned orders.  
- **People** – Contains regional manager assignments.

The analysis was completed using Python in a Jupyter Notebook environment.

---

## Project Workflow

### 1. Data Import and Cleaning
- Imported all datasets using pandas with appropriate encoding handling (`latin1`).
- Converted date columns (Order Date, Ship Date) into proper datetime format using `dayfirst=True`.
- Removed duplicate entries and handled missing values appropriately.
- Cleaned categorical fields (city, state, region).
- Joined Returns and People datasets with the main Orders data.
- Added new calculated fields such as:
  - Shipping Time (in days)
  - Profit Margin
  - Returned Indicator

---

### 2. Exploratory Data Analysis (EDA)
The following analyses and visualizations were performed:

- Sales vs Profit scatter plot  
- Shipping time distribution  
- Returned orders percentage  
- Sales by Region  
- Monthly sales trend analysis  
- Profit by Sub-Category  
- Sales by Category  

Multiple charts were generated using Matplotlib for clear visual interpretation.

---

## Key Insights

### 1. Profit vs Sales
- Sales and profit show a generally positive correlation.
- Several high-sales transactions result in negative profit, indicating issues with pricing, discounting, or fulfillment costs.

### 2. Shipping Time
- Most orders are delivered within 4–6 days.
- Very few orders are shipped within 1 day, suggesting standard delivery is the norm.

### 3. Return Rate
- Approximately 8% of orders are returned.
- This impacts profit margins and may indicate product quality issues or customer dissatisfaction.

### 4. Regional Sales
- The West region leads in total sales, followed by the East region.
- The South region has the lowest sales performance and could benefit from increased marketing or distribution expansion.

### 5. Monthly Sales Trend
- Monthly sales fluctuate but show a clear growth trend after 2016.
- Seasonal spikes suggest opportunities for targeted promotions and better inventory planning.

### 6. Profit by Sub-Category
- Tables and Bookcases are major loss-making categories.
- Copiers, Phones, Accessories, and Binders have strong profit contributions.

### 7. Sales by Category
- Technology is the highest revenue generator among all categories.
- Office Supplies and Furniture show moderate revenue with relatively lower margins.

---

## Business Recommendations

- Re-evaluate pricing and discount strategy for loss-making categories (especially Tables).  
- Investigate causes behind returned orders to reduce the 8% return rate.  
- Increase marketing and distribution efforts in the South region to improve performance.  
- Focus more on the high-profit categories such as Copiers and Phones.  
- Use monthly sales patterns to plan inventory, staffing, and promotional activities.

---

## Technologies Used
- Python  
- Jupyter Notebook  
- Pandas  
- Matplotlib  
- NumPy  

---

## How to Run This Project

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/retail-sales-analysis-superstore.git

2. Install Required Python Libraries
   pip install pandas matplotlib numpy


   If you need Jupyter Notebook:

   pip install notebook

3. Launch Jupyter Notebook
   jupyter notebook

4. Open the Analysis Notebook
   notebooks/01_eda.ipyb

5. Run All Cells

   This will execute:

    Data cleaning

    Exploratory analysis

    Visualizations

    Insights and recommendations

## Project Structure

 retail-sales-analysis-superstore/
│
├── notebooks/
│   └── superstore_analysis.ipynb
│
├── data/
│   ├── raw/
│   └── cleaned/
│
├── images/
│
└── README.md

