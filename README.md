# 🛒 E-Commerce Sales Dashboard | Power BI

## 📌 Project Overview

The **E-Commerce Sales Dashboard** is an interactive Power BI project designed to analyze and visualize e-commerce business performance.

The dashboard provides insights into **sales, profit, orders, customers, products, regional performance, and payment methods**. It helps businesses monitor key performance indicators and make data-driven decisions.

---

# 🎯 Project Objectives

The main objectives of this project are:

* Analyze overall sales performance.
* Track monthly sales trends.
* Identify top-performing product categories.
* Analyze best-selling products.
* Understand customer purchasing behavior.
* Identify top customers based on sales.
* Analyze regional and state-level performance.
* Monitor order status and payment methods.
* Provide interactive filtering using slicers.

---

# 🛠️ Tools and Technologies Used

* **Power BI Desktop**
* **Microsoft Excel**
* **Power Query**
* **DAX (Data Analysis Expressions)**
* **Data Modeling**
* **Data Visualization**

---

# 📊 Dashboard Pages

The dashboard contains **6 interactive pages**.

## 1️⃣ Executive Overview

This page provides a high-level overview of the overall e-commerce business performance.

### KPIs

* Total Sales
* Total Profit
* Total Orders
* Total Customers

### Visualizations

* Monthly Sales Trend
* Sales by Category

### Filters

* Year
* Region
* Category

---

## 2️⃣ Sales Analysis

This page focuses on analyzing sales performance and sales trends.

### KPIs

* Total Sales
* Average Order Value

### Visualizations

* Sales by Month
* Sales by Category

### Filters

* Year
* Category
* Sales Channel

---

## 3️⃣ Product Analysis

This page provides insights into product and category performance.

### KPIs

* Best Selling Product
* Total Quantity Sold

### Visualizations

* Top 10 Products by Sales
* Sales by Category

### Filters

* Category
* Subcategory

---

## 4️⃣ Customer Analysis

This page analyzes customer behavior and customer purchasing patterns.

### KPIs

* Total Customers
* Average Sales per Customer

### Visualizations

* Top 10 Customers by Sales
* Customers by Gender

### Filters

* Region
* Gender
* City

---

## 5️⃣ Regional Analysis

This page analyzes sales performance across different regions and states.

### KPIs

* Highest Sales Region
* Total Regional Sales

### Visualizations

* Sales by State
* Sales by Region

### Filters

* Region
* State
* Year

---

## 6️⃣ Order & Payment Analysis

This page focuses on order status, sales channels, and payment methods.

### KPIs

* Delivered Orders
* Cancelled Orders

### Visualizations

* Orders by Payment Method
* Orders by Sales Channel

### Filters

* Order Status
* Payment Method
* Sales Channel

---

# 📈 Key DAX Measures

## Total Sales

```DAX
Total Sales =
SUM('Sales'[Sales])
```

## Total Profit

```DAX
Total Profit =
SUM('Sales'[Profit])
```

## Total Orders

```DAX
Total Orders =
DISTINCTCOUNT('Sales'[Order ID])
```

## Total Customers

```DAX
Total Customers =
DISTINCTCOUNT('Sales'[Customer ID])
```

## Total Quantity Sold

```DAX
Total Quantity Sold =
SUM('Sales'[Quantity])
```

## Average Order Value

```DAX
Average Order Value =
DIVIDE(
    [Total Sales],
    [Total Orders],
    0
)
```

## Average Sales per Customer

```DAX
Average Sales per Customer =
DIVIDE(
    [Total Sales],
    [Total Customers],
    0
)
```

## Delivered Orders

```DAX
Delivered Orders =
CALCULATE(
    DISTINCTCOUNT('Sales'[Order ID]),
    'Sales'[Order Status] = "Delivered"
)
```

## Cancelled Orders

```DAX
Cancelled Orders =
CALCULATE(
    DISTINCTCOUNT('Sales'[Order ID]),
    'Sales'[Order Status] = "Cancelled"
)
```

---

# 🗂️ Dataset Information

The dataset contains e-commerce transaction information, including:

* Order ID
* Order Date
* Customer ID
* Customer Name
* Gender
* City
* State
* Region
* Category
* Subcategory
* Product Name
* Quantity
* Sales
* Profit
* Payment Method
* Sales Channel
* Order Status

---

# 🧹 Data Cleaning and Transformation

The following data cleaning steps were performed using Power Query:

* Checked and corrected data types.
* Removed blank rows.
* Removed duplicate records.
* Renamed columns for consistency.
* Checked for missing values.
* Created a date table.
* Created relationships between the date table and sales data.

---

# 🔍 Key Business Insights

The dashboard helps answer important business questions such as:

* Which months generate the highest sales?
* Which product categories generate the most revenue?
* Which products are the best-selling products?
* Who are the top customers?
* Which regions generate the highest sales?
* Which states contribute the most revenue?
* Which payment methods are most frequently used?
* How many orders are delivered and cancelled?
* Which sales channels generate the highest number of orders?

---

# 📁 Project Structure

```text
E-Commerce-Sales-Dashboard
│
├── E-Commerce Sales Dashboard.pbix
├── Dataset.xlsx
├── README.md
│
└── screenshots
    ├── Page1_Executive_Overview.png
    ├── Page2_Sales_Analysis.png
    ├── Page3_Product_Analysis.png
    ├── Page4_Customer_Analysis.png
    ├── Page5_Regional_Analysis.png
    └── Page6_Order_Payment_Analysis.png
```

---

# 📸 Dashboard Preview

## Executive Overview

![Executive Overview](screenshots/Page1_Executive_Overview.png)

## Sales Analysis

![Sales Analysis](screenshots/Page2_Sales_Analysis.png)

## Product Analysis

![Product Analysis](screenshots/Page3_Product_Analysis.png)

## Customer Analysis

![Customer Analysis](screenshots/Page4_Customer_Analysis.png)

## Regional Analysis

![Regional Analysis](screenshots/Page5_Regional_Analysis.png)

## Order & Payment Analysis

![Order & Payment Analysis](screenshots/Page6_Order_Payment_Analysis.png)

---

# 🚀 How to Use This Project

1. Download or clone this repository.
2. Open the `.pbix` file using Power BI Desktop.
3. Load or refresh the dataset if required.
4. Use the slicers to filter the dashboard.
5. Explore different dashboard pages to analyze business performance.

---

# 📚 Skills Demonstrated

This project demonstrates the following skills:

* Data Cleaning
* Data Transformation
* Power Query
* Data Modeling
* DAX Calculations
* KPI Development
* Interactive Dashboards
* Data Visualization
* Business Analysis
* Sales Analysis
* Customer Analysis
* Product Analysis
* Regional Analysis

---

# 📌 Future Improvements

Possible future improvements include:

* Adding sales forecasting.
* Adding profit margin analysis.
* Adding customer segmentation.
* Adding return and refund analysis.
* Adding advanced drill-through reports.
* Adding automated data refresh.
* Adding more advanced DAX calculations.

---

# 👨‍💻 Author

**Karuppasamy R**

Aspiring Data Analyst | Computer Science Engineering Student

### Skills

* Power BI
* SQL
* Microsoft Excel
* Python
* Data Analysis

---

# ⭐ Support

If you found this project useful, please consider giving the repository a ⭐ star.

---

## 📬 Connect With Me

Feel free to connect with me and explore my other projects.
