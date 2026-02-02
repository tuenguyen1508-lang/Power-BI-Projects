# MM PET Growth Snapshot  
## Product & Sales Performance (2024–2025)

## Summary
This dashboard reviews MM PET’s product and sales performance across 2024–2025, covering growth trends, customer activity, category/brand performance, and city-level results. It also includes practical recommendations based on the findings.

<img width="603" height="338" alt="image" src="https://github.com/user-attachments/assets/084e38f1-e842-4c48-99da-58651b194735" />

---

## Recommendations 
- Increase basket value (not just orders): Use bundles and add-ons (especially Food + Health) to lift AOV.
- Protect the #1 revenue driver (Food): Keep Food highly visible and consistently in stock—small gains here move total results.
- Scale winning brands: Prioritise PawGear, HealthPet, PawLife with stronger promotion and inventory support.
- Lift low-value areas: Improve Christchurch + Small Animal performance via pricing review, premium options, and multi-buy offers.
- Plan earlier for peak season: 2025 peaked in December, so prepare campaigns and stock ahead of Q4.
- Reduce dependence on Sydney: Strengthen Auckland and other cities to spread growth risk.

---

## Key Insights
- 2024: 121K orders | $1.4M revenue
- 2025: 157K orders | $1.6M revenue
- Customers: 2,172 unique
- Overall AOV: $11.4 per order
- YoY (2025 vs 2024): Revenue +13.8%, Orders +29.8%, AOV −12.3% (growth is volume-led)

---

## Dataset & Model (Star Schema)
 - **Fact_Transactions:** 413,530 rows × 9 columns (transaction id, transaction date, product id, customer id, location id, channel id, quantity, discount pct, order status, revenue,...)
- **Dimensions:**
  - Dim_Channel (8 × 4) (channel id, channel type, platform, payment method)
  - Dim_Customer (2,177 × 6) (customer id, gender, age band, member types, signup date, active)
  - Dim_Location (16 × 4) (location id, country, region, city, store type)
  - Dim_Product (48 × 11) (product id, sku, product name, pet type, category, sub category, brand,...)
  - Dim_Date 
- **Date table:** Built from Transaction Date + **Year / Month / Month Name** for time-intelligence

---

## Business Questions Covered

### Sales Analysis
- KPI overview (Orders, Customers, Revenue, AOV)
- Time trends (monthly revenue/orders)
- City performance (best vs worst)
- Category performance (best vs worst)
 
### Product Analysis
- Product performance (Revenue, Orders, AOV, YoY revenue/order)
- Product range overview (counts by category/brand/pack size)
- Brand performance (Revenue & Orders)
- Pet type performance (Revenue & Orders)
---

## Sales Trends & Performance

### Time Trends
- 2025: Drop Jan–Apr, rebound May–Jul, fluctuate Jul–Sep, climb Oct–Dec, peak ~$234K (Dec)
- 2024: Stable through mid-year, peak ~$234K (Oct), slight year-end dip

### Order Peaks
- 2025: Peak orders in Jan (15,670)
- 2024: Peak orders in Aug (15,430)

### Geography
- Sydney leads (~$775K revenue, ~58K orders)
- Christchurch lowest (~$139K) despite similar orders (~20K) → lower AOV/value mix

### Category Performance
- Food dominates: 169K orders | $1.5M revenue
- Toy: lowest revenue (~$400K)
- Health: lowest orders (~47K) but higher revenue than Toy → higher value per order

<img width="604" height="340" alt="image" src="https://github.com/user-attachments/assets/dbb47f1c-1f9f-43d1-95fb-dfcfd5801b46" />

---

## Product Analysis Highlights
- Product range: 15 brands | 4 categories | 25 subcategories | 45 products | 24 pack sizes
- Top brands: PawGear, HealthPet, PawLife lead in both revenue and orders (and all improved in 2025)
- Pet type: Dogs lead (then cats). Small animals have orders but low revenue per order

<img width="606" height="341" alt="image" src="https://github.com/user-attachments/assets/74de8de3-a0dc-4554-a9db-6a3c8a9bc4a7" />

---

## What’s Next
### Next Steps: Digging Into the “Why”
In the next presentation, I’ll use a deep-dive analysis hierarchy to explain why Sydney’s revenue was higher in 2024, even though Sydney’s orders were higher in 2025.


