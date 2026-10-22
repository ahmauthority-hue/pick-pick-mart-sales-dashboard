# Pick-Pick Mart | Sales Management Dashboard

An Excel sales dashboard and insights report for **Pick-Pick Mart**, a local supermarket in Rukpokwu, Port Harcourt, Nigeria. The dashboard turns the daily point-of-sale export (`daily_sale_logs`) into a clear view of what sold, when it sold and how customers paid, so management can make decisions on staffing, stock and cash handling.

![Dashboard preview](images/PICK__PICK_PROJECT.png)

---

## Project Contents

| File | Description |
|------|-------------|
| `daily_sale_logs.xlsx` | Excel workbook with the dashboard (add your file name here) |
| `PickPickMart_Insights_and_Recommendations.pdf` | 3-page report with insights and recommendations |
| `images/PICK__PICK_PROJECT.png` | Screenshot of the dashboard |
| `README.md` | This file |

---

## Business Problem

Sales were recorded at the till and exported daily as a CSV, but the data was only used to reconcile the till. There was no combined view of sales performance. Management needed a simple, low-cost way to answer:

- What are our best-selling products and categories?
- At what times of day are we busiest?
- How do customers pay (cash or POS)?

## Dashboard Features

- **KPI cards:** Total Sales, Top Category, Top Product, Peak Hour, Payment Mix
- **Charts:** sales by category, top selling items, sales by hour of day, sales by payment type
- **Slicers:** Category, Date, Cashier, Hour (time)

**Tool used:** Microsoft Excel (data cleaning, pivot tables, charts, slicers)

---

## Key Findings

### Finding 1: Total sales

Total sales on the dashboard are **₦3,977,450**.

### Finding 2: Revenue depends on a few staple products

| Item | Revenue | Share of total |
|------|---------|----------------|
| Mama Gold Rice 5kg | ₦824,500 | 20.7% |
| Indomie Noodles (Pack of 40) | ₦446,600 | 11.2% |
| Eggs (Crate of 30) | ₦239,400 | 6.0% |
| Kings Vegetable Oil 3L | ₦194,400 | 4.9% |
| Garri (Ijebu) 1 Paint | ₦184,800 | 4.6% |
| **Top 5 combined** | **₦1,889,700** | **47.5%** |

Rice and Indomie alone make up about 32% of sales. These are bulk household staples, which suggests many customers do stock-up shopping.

**Recommendation:** Set reorder levels and safety stock for these five items. Check them before opening and again before the late-afternoon rush.

### Finding 3: Foodstuff is the leading category by a wide margin

Foodstuff is the top category, several times larger than any other. The rest, in order, are Dairy & Beverages, Household, Baby Products, Beverages, Bakery/Fresh, Toiletries, Frozen/Provisions, Bakery and Beauty. Some labels overlap (Beverages vs Dairy & Beverages, Bakery vs Bakery/Fresh).

**Recommendation:** Merge overlapping category names in Power Query. Review range and shelf placement for the thinner categories (Baby Products, Toiletries, Beauty) to reduce dependence on Foodstuff.

### Finding 4: POS is the main payment channel

| Method | Sales | Share |
|--------|-------|-------|
| POS | ₦2,750,350 | 69.2% |
| Cash | ₦1,227,100 | 30.8% |

**Recommendation:** Compare each day's POS total with the POS provider's settlement credits in the bank, and bank the cash daily.

### Finding 5: Sales follow a clear daily rhythm

- **Busiest hours:** 5 PM (peak), 8 AM, 6 PM, 1 PM
- **Quietest hours:** 7 AM, 10 AM, 11 AM, 4 PM

**Recommendation:** Put the strongest cashiers and extra help on at the busy hours, schedule restocking in the quiet hours, and run time-limited offers on slow-moving categories at 10 to 11 AM or around 4 PM.

---

## Dashboard Improvements Identified

- The chart titled "top 10 selling item" shows only 5 items, and "top 5 sales by category" shows 10 categories. Fix the title or the filter.
- Correct "perment" to "payment".
- Sort the hours chart by clock time, not by sales value.
- Show the reporting period covered by the data.
- Add KPI cards for number of transactions, average basket value and sales per cashier.

## Suggested Next Data to Capture

- Cost price per item, to measure profit and margin
- Stock on hand and reorder levels
- Expiry dates for perishable goods
- Transaction IDs, to measure basket size

---

## Limitations

- Figures were read from the dashboard screenshot. Chart labels are exact; category bar sizes and the hourly ranking were read visually.
- The number of days covered is not shown on the dashboard.
- Sales figures are revenue, not profit.

## How to Use This Project

1. Download `daily_sale_logs.xlsx` and open it in Excel.
2. Use the slicers (Category, Date, Cashier, Hour) to filter the dashboard.
3. To refresh, paste the new daily sales export into the data sheet and use **Data > Refresh All**.

## Author

**Israel Anietie Bassey**, Data Analyst, Port Harcourt, Nigeria
