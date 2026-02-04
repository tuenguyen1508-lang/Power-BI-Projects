# ☕ Minnie Koffee Analytics Infographic (Melbourne Stores | 2023 Mid-Year Review)

An infographic-style Power BI report that highlights performance across Minnie Koffee’s three Melbourne locations (**Fitzroy, Preston, Bentleigh**). It summarises a **2023 mid-year review** and provides an **outlook for the second half of 2023**.

![Minnie Coffee Dashboard](https://github.com/user-attachments/assets/43646bba-a8fd-43b3-b828-aa4ee9ed0924)

---

## Executive Recommendations 

- **Align store hours with demand:** Trial slightly later opens and/or earlier closes, since sales **before 7 AM and after 7 PM** contribute only **3.6%** of year-to-date revenue.  
- **Strengthen peak-hour staffing (9–11 AM):** Add coverage around the **10 AM rush** to reduce queues and capture more sales during the busiest time.  
- **Promote best-sellers by location:** Feature each store’s top-earning products through menu placement, signage, and staff prompts to maximise high-performing items.  
- **Lift Saturday revenue with simple offers:** Use targeted weekend bundles or loyalty boosts to improve the lowest-revenue day without discounting across the whole week.  
- **Grow average order size gently:** Encourage add-ons and bundles (size upgrades, snack pairings) to lift the **$4.69** average spend without relying on heavy discounts.

---

## Key Questions Answered

1. **Which products are driving revenue so far in 2023?**  
2. **When do Melbourne stores generate the most revenue (time of day + day of week)?**  
3. **Based on current performance, what are the targets and forecast for 2023?**

---

## Dataset

- **Rows:** 149,117 (including headers)  
- **Columns (11):**
  - Transaction ID  
  - Transaction Date  
  - Transaction Time  
  - Transaction Quantity  
  - Store ID  
  - Store Location  
  - Product ID  
  - Unit Price  
  - Product Category  
  - Product Type  
  - Product Detail  

---

## Data Model (Star Schema)

- **Fact table:** `Fact_Transactions`  
- **Dimension tables:**
  - `Dim_Product`
  - `Dim_Store`
  - `Dim_Date`

---

## Key Insights (2023 YTD)

- **Total sales:** **$698,812** across **149,116 transactions**  
- **Average order size:** **$4.69**
  - Fitzroy: **$4.81**
  - Preston: **$4.66**
  - Bentleigh: **$4.59**
- **Top revenue products vary by store:**
  - Overall leader: **Davy Jones’ Sustainably Grown Organic Hot Chocolate Lg**
  - Fitzroy: **Jolly Roaster’s Dark Chocolate Lg**
  - Preston: **Civet Cat**
- **Peak time:** Customer spending peaks around **10 AM**  
- **Best day:** Monday | **Lowest day:** Saturday  
- **Daily pattern:** Sales rise after **7 AM** and taper off by **8 PM**
  - Transactions before **7 AM** and after **7 PM** total **$24,836** (**3.6%** of YTD sales)

---

## Forecast & Targets (2023)

- **Base target (first-year):** **$1,409,207** across the three Melbourne stores (based on average daily sales to date).  
- **Momentum note:** Average daily sales increased from **$2,852 (Jan–Mar)** to **$4,859 (Apr–Jun)**.  
- **Stretch goal:** **$1,592,839** if the recent growth trend continues.

---

## Visuals & Methods

Built using **DAX measures** and a mix of visuals for comparisons and trends, including:
- Bar charts  
- Column charts  
- Line charts  
- Stacked column charts  
- Matrices  

---

## Tools Used

- **Microsoft Power BI** (data model, visuals, interactions)  
- **Power Query** (data cleaning and shaping)  
- **DAX** (measures for sales, transactions, average order size, time/day analysis)  
- **Star Schema modelling** (Fact + Dimensions)

---

## Notes

- All figures are **year-to-date (2023)** and reflect transactions recorded in the dataset.  
- Targets are **estimates** based on current average daily sales; results may change with seasonality, promotions, staffing, and operating hours.  
- Store performance differs, so promotions and staffing should be reviewed **per location**.

---

