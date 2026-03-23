## Austin Housing Data Insights

# Housing Market Recommendations

- **Use median price as the key benchmark**  
  Median price provides a more realistic view of the market because it is less distorted by a small number of premium listings.

- **Compare homes by value, not just price**  
  Assess living area and lot size alongside price to identify which properties offer stronger value-for-money under budget constraints.

- **Focus on utility per dollar spent**  
  Prioritise properties that deliver the most practical benefit for the price, rather than paying for features that may not add equal value.

- **Treat premium features as optional cost drivers**  
  Features such as spas, scenic views, and luxury finishes often carry a price premium, so excluding them can improve affordability.

- **Use essentials-first filtering to support rational choice**  
  Narrow options by core needs such as bedrooms, bathrooms, parking, and HOA before comparing additional features.

- **Weigh school quality against opportunity cost**  
  High-rated school zones may offer stronger non-financial value, but often require trade-offs in price, size, or commute.

- **Consider substitute locations when preferred areas are too expensive**  
  If demand pushes prices too high in one suburb, compare nearby areas with similar access or amenities to find better-value alternatives.

- **Recognise that high prices often reflect supply–demand pressure**  
  Homes in desirable locations or with scarce features tend to command higher prices because demand is stronger relative to supply.

- **Do not rely on listing language alone**  
  Marketing terms in premium listings may signal exclusivity, but buyers should confirm whether the features actually justify the higher price.

- **Shortlist properties based on both affordability and long-term value**  
  A property that balances price, space, location, and essential features may provide better overall economic value than a higher-priced option with non-essential extras.

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
