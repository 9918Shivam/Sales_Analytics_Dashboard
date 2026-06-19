# 📊 Sales Analytics Dashboard — India (2024)

An end-to-end Sales Analytics project covering **3 Indian states**, **10 products**, and **a full year (Jan–Dec 2024)** of transactional data. Raw Excel data was cleaned and transformed, then visualized through an interactive **Power BI dashboard** that enables regional, product-level, and time-based sales analysis.

---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Dashboard Visuals](#dashboard-visuals)
- [Key Metrics](#key-metrics)
- [Key Insights & Findings](#key-insights--findings)
- [Getting Started](#getting-started)
- [Results Summary](#results-summary)
- [Future Scope](#future-scope)
- [Contact](#contact)

---

## Project Overview

This project analyzes retail sales performance across **Delhi**, **Rajasthan**, and **West Bengal** for the year 2024. The goal is to uncover which products, categories, cities, and time periods are driving the most revenue and profit — and where opportunities for growth exist.

**Business Questions Answered:**
- Which product categories and individual products generate the most profit?
- How do the three states compare in terms of sales and profitability?
- Which cities are the top contributors to total profit?
- What are the seasonal demand trends across the year?
- Where do upsell and cross-sell opportunities exist?

---

## Dataset Description

The dataset spans three separate Excel files — one per state — each following the same schema.

| Attribute | Details |
|-----------|---------|
| Files | `Delhi.xlsx`, `Rajasthan.xlsx`, `West_Bengal.xlsx` |
| Total Records | 2,532 orders |
| Time Period | January 2024 – December 2024 |
| States Covered | Delhi, Rajasthan, West Bengal |
| Cities Covered | New Delhi, Gurgaon, Jaipur, Udaipur, Kolkata, Howrah |
| Products | 10 unique products |
| Categories | Appliances, Electronics, Accessories |
| Missing Values | None |

### Column Reference

| Column | Description |
|--------|-------------|
| `Order_ID` | Unique identifier for each transaction |
| `Order_Date` | Date of the order (YYYY-MM-DD) |
| `First_Name` / `Last_Name` | Customer name |
| `State` | State where the order was placed |
| `City` | City where the order was placed |
| `Product, Category` | Product name and its category (comma-separated) |
| `Quantity` | Number of units ordered |
| `Unit_Price` | Price per unit in INR |
| `Profit` | Net profit earned from the order in INR |

### Products & Categories

| Category | Products |
|----------|---------|
| **Appliances** | Air Conditioner, Refrigerator, Washing Machine |
| **Electronics** | Laptop, Tablet, Monitor, Mobile |
| **Accessories** | Smart Watch, Headphones, Keyboard |

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| **Microsoft Excel** | Raw data storage and initial structuring |
| **Python (Pandas)** | Data merging, cleaning, EDA, and validation |
| **Power BI Desktop** | Interactive dashboard design and visualization |

---

## Project Structure

```
sales-analytics-dashboard/
│
├── data/
│   ├── Delhi.xlsx               # Delhi state sales data (856 records)
│   ├── Rajasthan.xlsx           # Rajasthan state sales data (817 records)
│   └── West_Bengal.xlsx         # West Bengal state sales data (859 records)
│
├── reports/
│   └── Sales_Analytics_Dashboard.pbix   # Power BI dashboard file
│
├── screenshots/
│   └── dashboard_preview.png    # Dashboard screenshot
│
└── README.md
```

---

## Dashboard Visuals

The Power BI dashboard is built with an interactive layout featuring state-level slicers, a city filter, and a full-year date range slider.

| Visual | Description |
|--------|-------------|
| **KPI Cards** | Total Orders, Total Quantity, Total Profit, Total Sales — at a glance |
| **Total Profit by Category** | Bar chart comparing Appliances, Electronics & Accessories |
| **Total Profit by City** | Donut chart showing profit share across 6 cities |
| **Total Profit by Product** | Bar chart ranking all 10 products by profit contribution |
| **Total Profit by State** | Area/line chart comparing Delhi, Rajasthan & West Bengal |
| **Total Sales by Product** | Horizontal bar chart ranking products by total sales volume |

**Interactive Filters:**
- State slicer — Delhi / Rajasthan / West Bengal
- City dropdown — All or specific city
- Date range slider — Jan 01, 2024 to Dec 31, 2024

---

## Key Metrics

| Metric | Value |
|--------|-------|
| Total Orders | 2,532 |
| Total Units Sold | 13,842 |
| Total Sales | ₹339.72M |
| Total Profit | ₹67.43M |
| Overall Profit Margin | 19.85% |
| Average Order Value | ₹1,34,169 |

---

## Key Insights & Findings

### 🏆 Category Performance
- **Appliances lead** with ₹33.98M in profit (50.4% of total), narrowly beating Electronics (₹30.3M / 44.9%)
- Accessories trail significantly at ₹3.15M — just 4.7% of total profit
- All three categories share a near-identical profit margin of ~20%, meaning volume, not margin, is the differentiator

### 📦 Product-Level Analysis

| Rank | Product | Profit | Sales |
|------|---------|--------|-------|
| 1 | Laptop | ₹14.51M | ₹72.55M |
| 2 | Air Conditioner | ₹13.79M | ₹70.85M |
| 3 | Refrigerator | ₹12.09M | ₹61.40M |
| 4 | Washing Machine | ₹8.10M | ₹39.37M |
| 5 | Tablet | ₹6.41M | ₹32.08M |
| 6 | Monitor | ₹4.98M | ₹25.36M |
| 7 | Mobile | ₹4.40M | ₹21.91M |
| 8 | Smart Watch | ₹2.12M | ₹11.03M |
| 9 | Headphones | ₹0.71M | ₹3.52M |
| 10 | Keyboard | ₹0.33M | ₹1.66M |

> **Laptop + Air Conditioner** together contribute **₹28.3M** — nearly **42% of all profit** from just 2 products.

### 🗺️ State-Level Performance
- All three states perform with remarkable consistency:
  - West Bengal — ₹22.67M
  - Delhi — ₹22.42M
  - Rajasthan — ₹22.34M
- The gap between the highest and lowest state is less than **₹0.33M** — indicating stable, evenly distributed demand across regions, not a single dominant market.

### 🏙️ City-Level Profit Breakdown

| City | State | Profit |
|------|-------|--------|
| Howrah | West Bengal | ₹11.83M (17.54%) |
| New Delhi | Delhi | ₹11.53M (17.09%) |
| Udaipur | Rajasthan | ₹11.33M (16.80%) |
| Jaipur | Rajasthan | ₹11.01M (16.34%) |
| Gurgaon | Delhi | ₹10.89M (16.15%) |
| Kolkata | West Bengal | ₹10.84M (16.08%) |

> All six cities contribute within a **1.5% range of each other** — a sign of healthy geographic distribution with no over-reliance on a single city.

### 📅 Monthly Profit Trends

| Month | Profit | Observation |
|-------|--------|-------------|
| July | ₹6.31M | 🔼 Peak month — summer appliance demand |
| April | ₹6.29M | 🔼 Pre-summer buying surge |
| September | ₹6.19M | 🔼 Festive season early demand |
| June | ₹4.82M | 🔽 Lowest month of the year |

> **Q1 (Jan–Mar)** is the steadiest quarter. **Q2 (Apr–Jun)** sees a dip mid-quarter before recovery. **Q3 (Jul–Sep)** is the strongest overall, driven by seasonal appliance sales.

### 💡 Strategic Observations
1. **Accessories are underperforming** — Headphones (₹0.71M) and Keyboard (₹0.33M) despite high unit volumes suggest low average order sizes; a bundling or upsell strategy could unlock hidden revenue.
2. **High-ticket items drive disproportionate profit** — Laptop and Air Conditioner each sell at high unit prices and consistently lead profit charts.
3. **Monitor has the highest unit volume (1,492 units)** yet ranks 6th in profit — pointing to thinner margins or lower unit price relative to other products.
4. **No regional outliers** — the business has achieved a well-balanced geographic distribution, which reduces concentration risk.


## Results Summary

| Dimension | Top Performer | Value |
|-----------|--------------|-------|
| Category | Appliances | ₹33.98M profit |
| Product (Profit) | Laptop | ₹14.51M |
| Product (Sales) | Laptop | ₹72.55M |
| State | West Bengal | ₹22.67M |
| City | Howrah | ₹11.83M |
| Month | July | ₹6.31M |
| Profit Margin | Uniform across categories | ~20% |

---

> ⭐ If you found this project helpful or insightful, consider starring the repo and sharing your feedback!
