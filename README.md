# 📊 E-Commerce Sales Analytics Dashboard (Power BI)

An interactive, single-page **Power BI** dashboard that analyzes e-commerce sales performance across products, regions, payment methods, customer satisfaction and delivery speed.

![E-Commerce Sales Dashboard](images/dashboard.png)

---

## 📌 Project Overview

This project turns a raw e-commerce transactions dataset into a clean, interactive dashboard that helps answer business questions such as:

- How much revenue is the business generating, and how is it trending over time?
- Which product categories and regions drive the most sales?
- Which payment methods do customers prefer?
- How quickly are orders delivered, and how satisfied are customers?

## 🗂️ Dataset

- **File:** `ecommerce_sales_analytics_5000.csv` (sourced from Kaggle)
- **Size:** 5,000 orders × 12 columns, no missing values or duplicates

| Column | Description |
|---|---|
| `order_id` | Unique order identifier |
| `order_date` | Date the order was placed |
| `customer_id` | Customer identifier |
| `product_category` | Beauty, Clothing, Electronics, Home |
| `region` | North, South, East, West |
| `quantity` | Units ordered (1–7) |
| `unit_price` | Price per unit |
| `discount` | Discount applied (0–35%) |
| `payment_method` | Card, COD, Wallet |
| `delivery_days` | Days taken to deliver (1–11) |
| `customer_rating` | Customer rating (1–5) |
| `revenue` | Order revenue after discount |

> **Note:** The dataset is synthetic. Order dates run one per day from Jan 2022 onward, so the date range extends well into the future. Treat the trends as illustrative rather than real-world.

## 🧮 Key Metrics (KPIs)

| KPI | Description |
|---|---|
| **Total Revenue** | Sum of revenue across all orders |
| **Total Orders** | Number of orders placed |
| **Total Customers** | Number of unique customers |
| **Average Order Value** | Total Revenue ÷ Total Orders |
| **Average Rating** | Mean customer rating |
| **Average Delivery Days** | Mean delivery time (shown as a gauge) |

## 📈 Dashboard Visuals

- **KPI cards** – Revenue, orders, customers, AOV, rating, delivery days
- **Line chart** – Monthly revenue trend (Jan–Dec)
- **Key Insights panel** – Short written takeaways from the data
- **Bar chart** – Revenue by product category
- **Column chart** – Revenue by region
- **Donut chart** – Orders share by payment method
- **Column chart** – Revenue by payment method
- **Bar chart** – Quantity sold by product category
- **Gauge** – Average delivery days
- **Slicers (dropdowns)** – Year, Region, Product Category, Payment Method

## 🔍 Highlights from the Data

- Total revenue is about **$5.1M** from **5,000 orders** and **989 unique customers**.
- Average order value is roughly **$1,022**.
- **Electronics** is the top category by revenue (~$1.83M, about 36% of the total), followed by **Clothing** (~$1.53M).
- Revenue is spread fairly evenly across regions, with **West** slightly ahead (~$1.35M).
- **Card** is the most-used payment method (~45% of orders), followed by COD (~35%) and Wallet (~19%).
- Average delivery time is **6.1 days**, about a day over the 5-day target, and the average rating is about **3.0 / 5**.

## 🛠️ Tools & Skills Used

- **Power BI Desktop**
- **DAX** – measures and a calendar table
- **Power Query** – data loading and cleaning
- **Data modeling** – relationship between the `ecommerce` fact table and a `Calendar` date table
- **Dashboard design** – layout, color theme, KPI cards, interactive slicers

## 📁 Repository Structure

```
├── PROJECT.pbix                          # Power BI dashboard file
├── ecommerce_sales_analytics_5000.csv    # Dataset
├── images/
│   └── dashboard.png                     # Dashboard screenshot
└── README.md
```

## 🚀 How to Use

1. Clone the repository
   ```bash
   git clone https://github.com/<your-username>/ecommerce-sales-analysis-dashboard.git
   ```
2. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free, Windows only).
3. Open `PROJECT.pbix`.
4. If prompted, update the data source path: **Home → Transform data → Data source settings** → point it to the local `ecommerce_sales_analytics_5000.csv`.
5. Use the slicers at the top to filter by year, region, category and payment method.

## 🔮 Future Improvements

- Add profit and margin analysis
- Add customer segmentation (e.g., new vs. returning)
- Add year-over-year comparison
- Publish to Power BI Service for easy sharing

## 👤 Author

**Arshpreet Kaur**
- GitHub: [@Arshpreet Kaur](https://github.com/arshpreetbrar127-boop/ecommerce-sales-analysis-dashboard)
 

---

⭐ If you found this project useful, consider giving it a star!
