#  Pizza Sales Data Analysis
Project Overview
This project analyzes a pizza sales dataset to uncover business insights, identify top-selling products, track sales trends, and evaluate customer purchasing behavior.
## Table of Contents
1. [Problem Statement](#-problem-statement)  
2. [Dataset Overview](#-dataset-overview)  
3. [Data Cleaning & Preparation](#-data-cleaning--preparation)  
4. [Exploratory Data Analysis (EDA)](#-exploratory-data-analysis-eda)  
   - [Key Performance Indicators (KPIs)](#-key-performance-indicators-kpis)  
   - [Sales Trend Over Time](#-1-sales-trend-over-time)  
   - [Sales by Day of Week](#-2-sales-by-day-of-week)  
   - [Sales by Pizza Category](#-3-sales-by-pizza-category)  
   - [Top 10 Best-Selling Pizzas](#-4-top-10-best-selling-pizzas)  
   - [Sales by Pizza Size](#-5-sales-by-pizza-size)  
5. [Business Insights](#-business-insights)  
6. [Recommendations](#-recommendations)  
7. [Tools Used](#-tools-used)  

---

##   Problem Statement
The pizza chain is experiencing inconsistent sales performance across different days, categories, and pizza types. Management needs clear answers to:  
- Which pizzas and categories contribute most to revenue?  
- How do sales vary across weekdays and months?  
- What are the top and least performing products?  
- Which pizza sizes are most preferred by customers?  

The objective is to analyze historical sales data and create a storytelling dashboard that will guide **sales strategy, promotions, and product optimization**.

---

##   Dataset Overview
The dataset contains transactional data of pizza sales with the following fields:  

- **order_id** → Unique identifier for each order  
- **order_date** → Date the order was placed  
- **pizza_name** → Name of the pizza sold  
- **pizza_category** → Category (Classic, Supreme, Veggie, Chicken)  
- **pizza_size** → Size (S, M, L, XL, XXL)  
- **quantity** → Number of pizzas sold  
- **unit_price** → Price per unit  
- **total_price / sales** → Computed revenue (`quantity × unit_price`)  

---

##   Data Cleaning & Preparation
- Converted `order_date` into proper **datetime format** (`day-first format`).  
- Created new **time-based columns**:
  - `MonthYear` → e.g., Jan 2015  
  - `WeekdayName` → Monday, Tuesday, etc.  
  - `OrderHour` → Hour of purchase (0–23)  
- Created a `sales` column where missing (`quantity × unit_price`).  

---

##   Exploratory Data Analysis (EDA)

###  Key Performance Indicators (KPIs)
- ** Total Sales:** `$817,860`  
- ** Total Orders:** `21350`  
- ** Total Pizzas Sold:** `49574.0`  
- ** Average Order Value (AOV):** `$38.31`  

---

###   1. Sales Trend Over Time
- **Visualization:** Line chart of monthly sales.  
- **Insight:** Sales show seasonal peaks, with consistent growth in certain months.  

---

###   2. Sales by Day of Week
- **Visualization:** Bar chart (Mon–Sun).  
- **Insight:** **Friday and Saturday** are peak sales days, while **Monday** records the lowest sales.  

---

###   3. Sales by Pizza Category
- **Visualization:** Pie chart of revenue share.  
- **Insight:** **Classic pizzas** dominate revenue, while **Veggie pizzas** lag behind.  

---

###   4. Top 10 Best-Selling Pizzas
- **Visualization:** Horizontal bar chart of top 10 by revenue.  
- **Insight:** The **Barbecue Chicken** and **Classic Deluxe** pizzas are consistent best-sellers.  

---

###   5. Sales by Pizza Size
- **Visualization:** Bar chart of size vs revenue.  
- **Insight:** **Large (L)** pizzas are most popular; **XXL** contributes the least.  

---

##   Business Insights
1. **Promotions on weekends** can maximize sales when demand is naturally high.  
2. **Upselling Medium → Large pizzas** may increase revenue, given large pizzas dominate.  
3. **Menu optimization:** Consider reviewing or rebranding **low-performing pizzas**.  
4. **Focus on Classic pizzas**, since they are the backbone of sales performance.  

---

##   Recommendations
- Use **targeted discounts during weekdays** to balance sales distribution.  
- Introduce **bundle deals** (e.g., Large pizza + drink) to boost average order value.  
- Launch **limited-time offers** for underperforming categories to test market response.  
- Continue monitoring with a **Power BI storytelling dashboard** for executive decision-making.  

---

##   Tools Used
- **Python** → `pandas`, `matplotlib` (data analysis & visualization)  
  
- **Jupyter Notebook** → data exploration  

