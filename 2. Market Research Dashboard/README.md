# MarketMindz Marketing & Sales Dashboard (Food & Beverage)

## Overview
This project was completed at **MarketMindz**, a market research firm collaborating with a retail vendor that specializes in **food and beverage products**. The goal is to build an interactive dashboard that explains performance clearly and supports practical business decisions.

---

## Business Questions
The dashboard answers four core questions:

1. **How are our six most recent marketing campaigns performing?**  
2. **How are our products performing?**  
3. **Who are our customers?**  
4. **What factors influence campaign performance and buyer decision-making?**

---

## Financial Recommendations (Top Takeaways)
- **Protect and grow Wine sales:** Wine is the strongest sales driver, so keep it visible, well-stocked, and consistently promoted—especially in the best-performing campaigns.  
- **Scale what worked in Campaign 6, while monitoring profitability:** Campaign 6 generated the most purchases, and Campaigns 5–6 delivered the most revenue. Reuse the same approach (timing, offer, audience), but watch discount levels so revenue growth does not reduce profit.  
- **Use strong in-store performance to support online sales:** Since most purchases occur in-store, encourage repeat and online buying (e.g., QR codes on receipts, “buy online next time” offers, or web-only bundles).  
- **Target offers to reduce wasted spend:** Buying patterns vary by age, income, and household size, so tailor messaging (e.g., wine-focused offers for older customers) to improve campaign efficiency.  
- **Increase revenue per purchase with bundles and cross-sell:** Pair best-sellers (wine) with complementary products (meat or other popular items) to increase average basket size.  
- **Strengthen loyalty for stable repeat revenue:** With a large base of older, educated, mostly married customers, retention tactics (member pricing, points, personalised follow-ups) can support consistent revenue over time.

---

## Dataset
- **Rows:** 2,241 (including headers)  
- **Columns:** 28  
- **Key fields:**  
  - Customer ID  
  - Year of Birth  
  - Education  
  - Marital Status  
  - Income  
  - Campaign Acceptance  
  - Product Purchase Amounts  

---

## Data Preparation (Power Query)
I cleaned and reshaped the data in **Power Query**, then created three supporting tables from the main dataset:

- **Campaign**: (ID, campaign, Accepted_Ind)  
- **Products**: (ID, product, total sales)  
- **Platform**: (ID, platform, quantity)  

---

## Dashboard Structure
The report contains **three pages**:

### 1) Campaign Performance
**Key insights:**
- **Wine** has the highest total sales, followed by **meat**.  
- **Campaign 6** drives the highest purchase volume.  
- **Campaigns 5 and 6** generate the most revenue.  
- Wine remains the most popular product across campaigns.  
- **In-store purchases dominate** overall (~13K purchases), followed by web purchases.

<img width="608" height="340" alt="image" src="https://github.com/user-attachments/assets/446d9960-1864-4849-9eab-42b52a7e50c1" />

### 2) Buyer Composition
**Key insights:**
- **2,000+ customers**, average age **57**, average income **~$52K**.  
- Most customers completed **college/university**.  
- Majority are **married**.  
- More than half have **0 kids and 0 teens at home**.  
- As customers get older: **Wine share increases**, while **meat share decreases**.

<img width="605" height="341" alt="image" src="https://github.com/user-attachments/assets/7c7712aa-2fbd-437c-a7e9-cf54bbbd9e24" />

### 3) Purchase Driver
Users can explore what drives results by selecting:
- One or more **campaigns**
- One or more **products**

Using filters such as:
- Income, age, country, education, marital status  
- Number of kids at home, number of teens at home  
- Web visits last month  

The dashboard shows:
- **Likelihood of campaign acceptance**, and/or  
- How **average total sales** change when product levels increase/decrease, broken down by the same customer factors.

<img width="605" height="341" alt="image" src="https://github.com/user-attachments/assets/bcd26686-c39d-4445-aa7b-6b203b74bc0f" />

---

## Tools Used
- Power BI  
- Power Query (data cleaning and reshaping)  

---

## Notes
This dashboard is designed to be easy to interpret for both technical and non-technical stakeholders, focusing on clear insights, actionable trends, and practical recommendations.

