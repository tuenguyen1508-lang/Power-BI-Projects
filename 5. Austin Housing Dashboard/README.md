## Austin Housing Data Insights

### Financial Recommendations
Based on the listing patterns and feature/price relationships in this dataset, here are practical, non-technical recommendations for buyers and renters comparing options:

- **Use the median price as your main “typical price” benchmark.** Medians are less affected by very expensive homes, so they often reflect the market more realistically than averages.
- **Compare homes by “space for the price,” not just total price.** Check living area (sq ft) and lot size together—two homes with similar prices can offer very different value depending on size.
- **If you want to keep costs down, treat premium features as optional.** Homes with features like **Spa** and **View** tend to be priced higher, so excluding these can widen your affordable choices.
- **Prioritize what matters most: schools vs. commute vs. features.** If school quality is important, focus on high-rated school zones first, then use the map and filters to balance distance and price.
- **Use filters to avoid “nice-to-have” extras inflating your shortlist.** Narrow by essentials (beds, baths, parking, HOA) before comparing homes—this helps keep comparisons fair and focused.
- **For high-end listings, don’t rely on descriptions alone.** Words like *room, living, pool, kitchen, private* are common in $2M+ listings, so use the metrics and features to confirm what’s truly included.

> Note: These recommendations are meant for general decision support and should be combined with personal budget, inspections, and local advice.

---

### Overview
This project delivers a comprehensive, interactive view of the Austin, Texas real estate market. Built in **Power BI**, the dashboard enables users to explore current listings, assess market patterns, compare school quality, and understand which home features most influence listing prices.

The report is organized into **four core sections**:
- **Summary View:** High-level snapshot of pricing, lot size, and living area metrics.
- **Location View:** Interactive map to explore listings geographically, supported by filters.
- **School View:** Insights into nearby school ratings, sizes, and how they shape housing decisions.
- **Features View:** Analysis of how property features (garage, heating, spa, views, etc.) impact prices.

---

### Dataset
- **Rows:** 15,172 (including headers)  
- **Columns:** 47  

**Key fields include:**
- Zpid
- City
- Street address
- Description
- Home features

---

### Data Preparation (Power Query)
The dataset was cleaned and reshaped in **Power Query** through steps such as merging queries, removing unnecessary columns, removing duplicates, filtering rows, unpivoting and splitting columns, and standardizing fields.

To support analysis, I built a **housing fact table** and **six dimension tables**:
- Location
- Schools
- Description
- Features
- House
- Feature Pivot

---

### Dashboard Structure

#### 1) Cover Page
Provides the dashboard purpose and a clear navigation overview for: **Summary**, **Location**, **School**, and **Features** views.

<img width="1223" height="687" alt="Screenshot 2026-02-23 110633" src="https://github.com/user-attachments/assets/0d0c401c-1189-4b27-8805-c741385f0d9f" />

#### 2) Summary Page — Austin Housing Market Insights
Key insights include:
- **Median Home Price:** $405,000
- **Median Living Area:** 1,975 sq ft
- **Median Lot Size:** 8,276 sq ft
- **Single-family homes** make up the majority of listings.
- **Median vs. average prices differ noticeably** across home types, indicating that a smaller number of higher-priced homes can skew averages.
- **Most properties were built in 2006**, suggesting a large portion of supply comes from the same development era.
- **Cooling and heating are common** across listings, making them baseline expectations rather than differentiators.

<img width="1221" height="683" alt="Screenshot 2026-02-23 110655" src="https://github.com/user-attachments/assets/fe07f5fc-86de-4327-9195-612a1994a6c9" />

#### 3) Location Page — Explore Properties on the Map
The interactive map allows users to:
- Filter by **price range, lot size, living area, home type, and amenities**.
- Identify clusters of listings across Austin neighborhoods.

<img width="1215" height="681" alt="Screenshot 2026-02-23 111007" src="https://github.com/user-attachments/assets/0626986d-b4e0-4d8a-a7d4-55523d37b1a7" />

#### 4) Location Filter Panel — Refine Your Search
A detailed filter panel supports more specific selection by:
- Bedrooms, bathrooms, parking
- HOA presence, view, spa, and other key amenities
- Exact feature combinations that match user preferences

<img width="1213" height="683" alt="Screenshot 2026-02-23 111019" src="https://github.com/user-attachments/assets/43d61677-5d90-437c-b065-5032d57b9557" />

#### 5) School Page — Find Family-Friendly Communities
Key highlights:
- **Average School Rating:** 5.8
- **Average School Size:** 1,239 students
- **Median Student–Teacher Ratio:** 14.8
- Mapped high-rated school zones, with filters for **rating, size, and students per teacher** to guide home buying decisions.

<img width="1217" height="686" alt="Screenshot 2026-02-23 113411" src="https://github.com/user-attachments/assets/5e92e136-142e-4bca-84eb-38c581d6ad58" />

#### 6) Features Page — What Drives Home Prices?
Key observations:
- Homes with **Spa** and **View** features tend to have significantly higher listing prices.
- Larger **lot sizes**, more **bathrooms**, and more **stories** are strongly associated with higher prices.
- AI-driven **key influencer** insights highlight the top drivers of high-priced listings.
- For properties **$2M+**, the five most common agent keywords are: **room, living, pool, kitchen, private**.

<img width="1220" height="679" alt="Screenshot 2026-02-23 113423" src="https://github.com/user-attachments/assets/7844608c-3c0f-4b90-a60e-87a35f5a48c5" />

---

### Tools Used
- **Excel:** Downloading and reviewing the dataset  
- **Power BI:** Data model, visuals, interactivity, navigation  
- **Power Query:** Data cleaning and reshaping  
- **Data Modeling:** Star-schema style modeling (fact + dimension structure)  

---

### Notes
The dashboard is designed to be clear and user-friendly for both technical and non-technical stakeholders, emphasizing actionable insights, easy exploration, and practical decision support.
