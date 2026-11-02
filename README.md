# Supermart-Grocery-Sales-Dashboard
Interactive Excel dashboard analysing Supermart grocery sales (2015–2018): sales trends, product performance, profit vs discount and city-level insights. Built with Pivot Tables, PivotCharts and Slicers.
# Supermart Grocery Sales Dashboard

An interactive Excel dashboard that helps management understand sales, profit, products, discounts and geographic performance in one place.

![Dashboard](screenshots/dashboard.png)

## Project Overview
Supermart's management team wanted a simple dashboard to answer key business questions without going through the full dataset. This project cleans the sales data, analyses it with Pivot Tables, and presents the findings in an interactive dashboard with slicers.

## Business Objectives
| # | Objective | Business Question |
|---|-----------|-------------------|
| 1 | Overall Sales Performance | How is the overall grocery business performing? |
| 2 | Product Performance | Which products and categories drive sales and profit? |
| 3 | Profit and Discount | How are discounts and profit related? |
| 4 | Geographic Performance | Which locations contribute most to the business? |

## Dataset
- **Rows:** 9,994 orders | **Period:** 2015–2018
- **Columns:** Order ID, Customer Name, Category, Sub Category, City, Order Date, Region, Sales, Discount, Profit, State
- **Coverage:** 7 categories, 23 sub-categories, 24 cities, 5 regions, 1 state (Tamil Nadu)

## Tools Used
Microsoft Excel: Pivot Tables, PivotCharts, Slicers, SUMIFS, CORREL, GETPIVOTDATA, Conditional Formatting.

## Method
1. Imported the CSV and fixed mixed `Order Date` formats (dd-mm-yyyy and mm/dd/yyyy) into real Excel dates.
2. Added helper columns: Year, Month, Profit Margin %, Discount Band.
3. Built one analysis sheet per objective (`Obj_1` to `Obj_4`) using Pivot Tables.
4. Combined KPIs and charts into a single interactive `Dashboard` sheet with Region, Category and Year slicers.

## Key KPIs
| KPI | Value |
|---|---|
| Total Sales | ₹1,49,56,982 |
| Total Profit | ₹37,47,121 |
| Profit Margin | 25.05% |
| Total Orders | 9,994 |
| Avg Order Value | ₹1,496.60 |

## Key Findings
- **Growth:** Sales grew 67% from ₹29.76L (2015) to ₹49.78L (2018), with growth accelerating after 2016.
- **Categories:** All seven categories contribute almost equally (13.6%–15.2%). Eggs, Meat & Fish leads with 15.2%.
- **Regions:** West (32%) and East (28%) generate about 60% of sales and profit. The North region has only one order.
- **Products:** Health Drinks (₹10.51L) and Soft Drinks (₹10.34L) are the top sub-categories. Soft Drinks, Cookies, Masalas, Spices, Cakes and Biscuits sell above average but earn below the overall 25.05% margin.
- **Discounts:** The correlation between discount and profit is about 0 (0.00002). Average margin stays between 24.8% and 25.6% in every discount band.
- **Cities:** Kanyakumari (₹7.07L) is the top city. Tenkasi, Kanyakumari, Salem, Coimbatore, Cumbum and Tirunelveli have high sales but below-average margins.

## Recommendations
1. Review pricing and costs for high-selling, low-margin sub-categories (Soft Drinks, Cookies, Masalas, Spices, Cakes, Biscuits).
2. Avoid blanket deep discounts; test targeted offers instead, since discount shows no clear link with profit.
3. Keep investing in West and East, and look for growth in South and Central.
4. Learn from high-margin cities (Karur, Bodi) and apply it in weaker ones (Tenkasi, Kanyakumari, Salem).

## Data Notes
- The dataset contains only one state, Tamil Nadu, so geographic analysis is done at city level.
- The North region has just one order.
- "Products" are analysed at sub-category level because the dataset has no product name column.
- Profit Margin = Profit ÷ Sales.

## How to Use
1. Download `Supermart_Grocery_Sales_Dashboard.xlsx`.
2. Open it in **Excel desktop** (slicers and PivotCharts need it) and go to the `Dashboard` sheet.
3. Use the Region, Category and Year slicers to filter all charts.

## Author
[@ravijisharma765-sudo](https://github.com/ravijisharma765-sudo)
