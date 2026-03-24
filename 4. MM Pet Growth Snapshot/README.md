# MM PET Growth Snapshot  
## Product & Sales Performance (2024–2025)

## Summary
This Power BI dashboard analyses MM PET’s sales and product performance across 2024 and 2025. It is designed to help stakeholders understand overall business performance, identify key revenue and order drivers, evaluate product trends, and investigate why Sydney remains the strongest yet most important focus market.

The dashboard is divided into four main pages:

- Home
- Sales Analysis
- Product Analysis
- Sydney Deep Dive

---

## Dataset & Model (Star Schema)
 - **Fact_Transactions:** 413,530 rows × 9 columns (transaction id, transaction date, product id, customer id, location id, channel id, quantity, discount pct, order status, revenue,...)
- **Dimensions:**
  - Dim_Channel (8 × 4) (channel id, channel type, platform, payment method)
  - Dim_Customer (2,177 × 6) (customer id, gender, age band, member types, signup date, active)
  - Dim_Location (16 × 4) (location id, country, region, city, store type)
  - Dim_Product (48 × 11) (product id, sku, product name, pet type, category, sub category, brand,...)
  - Dim_Date: Built from Transaction Date + **Year / Month / Month Name** for time-intelligence

---

## Business Questions Covered

### Home Page
- What is the purpose of this dashboard?
- What areas of business performance are being analysed?
- Which pages should users explore for sales, product, and city-level insights?
- What is the main business issue identified across the dashboard?

### Sales Analysis
- How did sales performance change from 2024 to 2025?
- Did revenue growth keep pace with order growth?
- Which cities generated the highest revenue and order volume?
- Which product categories contributed the most to revenue and orders?
- Where are the main opportunities to improve sales performance?

### Product Analysis
- Which brands are the strongest revenue and order drivers?
- Which pet types contribute the most to overall performance?
- Is product growth driven by higher value or only by higher order volume?
- Which product segments are underperforming?
- Where are the best opportunities for bundling, upselling, or product focus?

### Sydney Deep Dive
- Why did Sydney’s revenue underperform despite strong order growth?
- Is the issue caused by lower demand or lower average order value?
- Which brands, categories, and sub-categories are driving revenue decline in Sydney?
- Which products and pack sizes show the greatest revenue leakage?
- What actions can improve revenue quality in Sydney?
---

## Dashboard Structure

## 1. Home Page

### Purpose
The Home page provides a high-level introduction to the dashboard and acts as the main navigation hub. It helps users understand the dashboard’s business objective and move easily to the detailed analysis pages.

<img width="2014" height="1130" alt="image" src="https://github.com/user-attachments/assets/26bbe1f0-e083-4a20-a9e6-876840fb1777" />

---

## 2. Sales Analysis

### Purpose
The Sales Analysis page evaluates overall business performance across time, city, and category. It helps track revenue, orders, customers, and average order value, while also showing where growth is happening and where improvement is needed.

<img width="2008" height="1128" alt="image" src="https://github.com/user-attachments/assets/f44833fc-7806-441f-a702-b9fb328d91f6" />

### Key Insights
- Orders increased significantly in 2025 compared with 2024, while revenue also increased but at a slower rate.
- Sydney was the top-performing city in both revenue and order volume.
- Auckland followed as the second strongest city, while Christchurch recorded the lowest revenue.
- Food was the strongest category, contributing the highest revenue and order count.
- Health generated fewer orders than Toy but achieved stronger value per order.
- Sales patterns suggest that 2025 growth came mainly from increased order quantity rather than stronger revenue per transaction.

### Recommendations
- Improve basket size through bundles and cross-sell strategies.
- Focus on Food as the core revenue-driving category.
- Review pricing, discounts, and product mix in lower-performing cities such as Christchurch.
- Prepare earlier for peak season demand.
- Reduce over-reliance on Sydney by strengthening other city markets.

---

## 3. Product Analysis

### Purpose
The Product Analysis page explores performance by brand, pet type, category, product, and pack size. It is intended to show which products are driving sales, which segments are underperforming, and whether growth is sustainable in value terms.

<img width="2012" height="1132" alt="image" src="https://github.com/user-attachments/assets/ce5acb2a-8f9a-40fd-83eb-2da540d71f6a" />

### Key Insights
- The business has a broad product portfolio across brands, categories, sub-categories, products, and pack sizes.
- Revenue grew in 2025, but order growth was much stronger than revenue growth.
- Average order value declined, reinforcing the pattern of volume-led growth.
- Top-performing brands included PawGear, HealthPet, and PawLife.
- Dog products contributed the highest revenue, followed by Cat products.
- Small Animal products generated reasonable order volume but weaker revenue contribution.

### Recommendations
- Invest more in leading brands such as PawGear, HealthPet, and PawLife.
- Continue prioritising Dog and Cat product segments, as they are the strongest revenue contributors.
- Explore bundling and upselling opportunities for Small Animal products.
- Monitor not just product volume growth, but also value growth to protect overall profitability.
  
---
## 4. Sydney Deep Dive

### Purpose
The Sydney Deep Dive page investigates why Sydney’s revenue weakened in 2025 despite higher order volume. It breaks performance down from brand to category, sub-category, product, and pack size to identify where revenue loss is occurring.

<img width="2014" height="1130" alt="image" src="https://github.com/user-attachments/assets/228d0ffa-9907-4dcb-a3b3-3ded4462e8c0" />

### Key Insights
- Sydney remained the strongest city overall, but revenue declined relative to expectations because average order value fell.
- Orders increased across leading brands, but revenue performance weakened due to lower basket value.
- Food was the biggest revenue drag, despite continuing to generate strong order volume.
- Weakness was also observed in selected sub-categories such as dry food, wet food, food mix, leash, vitamins, and interactive toys.
- At the product and pack-size level, several specific items showed declining revenue caused by lower value per order.
- The main issue in Sydney was not demand, but declining order quality and lower revenue per transaction.

### Recommendations
- Focus on recovering average order value in Sydney rather than only driving more orders.
- Prioritise top brands and Food-related products because of their strong impact on total revenue.
- Improve low-performing products using bundle offers, premium trade-up strategies, and checkout add-ons.
- Set performance targets that balance both order growth and order value improvement.
- Use Sydney as a priority market for revenue-quality improvement strategies.

---
## Final Summary
This dashboard shows that MM PET achieved stronger business activity in 2025, but most of the growth came from higher order volume rather than improved order value. While cities such as Sydney continue to lead performance, deeper analysis shows that lower basket value is limiting revenue potential. Across both sales and product performance, the business opportunity is not simply to increase transactions, but to improve the quality and value of each order.

The most important next step is to strengthen average order value through better product mix, smarter promotions, bundling strategies, and targeted action in the areas with the greatest revenue leakage.

---
## Tools Used

- **Power Query + Excel** (data viewing, cleaning and shaping)  
- **Microsoft Power BI** (data model, visuals, interactions)  
- **DAX** (measures for AoV, YoY %, total orders, total revenue)  
- **Star Schema modelling** (Fact + Dimensions)

---
## Note
Please refer to the detailed slide deck for the full dataset overview and cleaning process, business questions and analysis goals, dashboard build methodology and key techniques, as well as the complete insights and recommendations: https://drive.google.com/file/d/1o-zMOMz2_RaXZmP6SHwR7Mgos3lOZybX/view?usp=sharing. 


