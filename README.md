# Dynamic.-Retail-Dashboard
The Dynamic Retail Dashboard is an interactive and data-driven tool built in Excel to visualize and analyze retail data. It connects to datasets hosted on GitHub, uses Power Query for data transformation, and presents insights through dynamic charts and KPIs. The dashboard solves key business questions, enabling informed decision-making.

# Dynamic Excel Dashboard Repository

##  Project Overview

This repository contains a **dynamic Excel dashboard** designed to analyze and visualize sales, returns, and regional data. The dashboard provides insightful metrics and interactive elements to assist in decision-making.

##  Datasets Used

### 1. Orders Table

Contains details of customer orders, including product, shipping, and financial metrics.

#### Sample Data:

| Order ID       | Returned | Order Date | Ship Date  | Ship Mode    | Customer Name | Segment   | Country       | Market | Sales   | Profit  | Discount |
| -------------- | -------- | ---------- | ---------- | ------------ | ------------- | --------- | ------------- | ------ | ------- | ------- | -------- |
| CA-2012-124891 | No       | 31-07-2020 | 31-07-2020 | Same Day     | Rick Hansen   | Consumer  | United States | US     | 2309.65 | 762.18  | 0        |
| IN-2013-77878  | Yes      | 05-02-2021 | 07-02-2021 | Second Class | Justin Ritter | Corporate | Australia     | APAC   | 3709.40 | -288.77 | 0.1      |
| IN-2013-71249  | No       | 17-10-2021 | 18-10-2021 | First Class  | Craig Reiter  | Consumer  | Australia     | APAC   | 5175.17 | 919.97  | 0.1      |

### 2. Returns Table

Tracks orders that have been returned, along with the associated markets.

#### Sample Data:

| Returned | Order ID        | Market        |
| -------- | --------------- | ------------- |
| Yes      | MX-2013-168137  | LATAM         |
| Yes      | US-2011-165316  | LATAM         |
| Yes      | ES-2013-1525878 | EU            |
| Yes      | CA-2013-118311  | United States |

### 3. People Table

Contains details about sales representatives and their respective regions.

#### Sample Data:

| Person            | Region  |
| ----------------- | ------- |
| Anna Andreadi     | Central |
| Chuck Magee       | South   |
| Kelly Williams    | East    |
| Matt Collister    | West    |
| Deborah Brumfield | Africa  |

##  Problem Statements Solved with Steps

### 1. Key Performance Indicators (KPIs)

**Objective:** Calculate and display Total Sales, Total Profit, Total Quantity, Number of Orders, and Profit Margin dynamically.

**Steps:**

- Import the Orders Table into Excel using Power Query.
- Create calculated columns:
  - Profit Margin = Profit / Sales.
  - Total Orders = Count of Order ID.
- Use Excel formulas:
  - Total Sales = `=SUM(Sales)`.
  - Total Profit = `=SUM(Profit)`.
  - Total Quantity = `=SUM(Quantity)`.
- Build a dynamic KPI table and enhance visual appeal with symbols.
![image](https://github.com/user-attachments/assets/6436773f-b20f-44b4-956f-db46e1ed0c3f)

### 2. Sales and Profit Analysis

**Objective:** Visualize sales and profit trends over time.

**Steps:**

- Create a Pivot Table with Order Date grouped by Year and Month.
- Add Sales and Profit as values.
- Create a Line Chart to display trends.
- Apply slicers for filtering by category, market, or region.
- ![image](https://github.com/user-attachments/assets/b6520cf0-8697-4a8a-9a5e-fee9d8b6c609)


### 3. Category-Wise Profit

**Objective:** Analyze profitability across product categories.

**Steps:**

- Create a Pivot Table using Category as rows and Profit as values.
- Sort the table in descending order of Profit.
- Create a Bar Chart.
- Add slicers for interactivity.
- ![image](https://github.com/user-attachments/assets/25b98465-a03c-4a7b-8832-6d88441e9f42)
![image](https://github.com/user-attachments/assets/72886a77-c133-4139-94ff-cbad0644767a)


### 4. Segment-Wise Sales Share (%)

**Objective:** Display the proportion of sales for each customer segment.

**Steps:**

- Create a Pivot Table with Segment as rows and Sales as values.
- Calculate percentage share using `=Sales / Total Sales * 100`.
- Create a Pie Chart or Donut Chart.
- Add dynamic labels.
- ![image](https://github.com/user-attachments/assets/8a252a56-1469-420b-9e71-6ce32e0d8407)


### 5. Sales by Country

**Objective:** Analyze sales performance by country.

**Steps:**

- Create a Pivot Table with Country as rows and Sales as values.
- Sort the table in descending order of Sales.
- Use conditional formatting or a Heatmap to highlight top-performing countries.
- ![image](https://github.com/user-attachments/assets/ce09c824-31bb-4f17-b538-09d38f0ced2b)


### 6. Top 5 Subcategories

**Objective:** Identify the top 5 performing subcategories.

**Steps:**

- Create a Pivot Table with Sub-Category as rows and Sales as values.
- Sort the table in descending order of Sales.
- Filter to display the top 5 Sub-Categories.
- Use a Column Chart to visualize results.
- ![image](https://github.com/user-attachments/assets/5aac1def-0cbf-4ecd-9c81-a31f3a8ce9ba)


##  Dynamic Features

The dashboard includes:

- **Dynamic Charts:** Updates in real-time based on slicer inputs.
- **Power Query Integration:** Automates data cleaning and transformation.
- **KPI Table:** Highlights critical metrics at a glance.
- ![image](https://github.com/user-attachments/assets/db87e472-b1d0-4207-8dc2-37865c30f991)


##  Next Steps for Extension

Additional insights to enhance the dashboard:

- **Return Analysis:** Investigate return rates by market or product category.
- **Top and Bottom Customers:** Identify most and least profitable customers.
- **Market Analysis:** Compare performance across different markets.
- **Product Analysis:** Evaluate individual product contributions.

##  Significance

This dashboard empowers retail businesses to:

- Track performance through KPIs.
- Understand category, segment, and geographic trends.
- Make data-driven decisions to optimize operations.
- ![image](https://github.com/user-attachments/assets/af621c91-2852-42a0-9027-5a02e2c66d59)






