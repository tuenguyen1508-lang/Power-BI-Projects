# Power BI Sales Analysis Interactive Dashboard

## Overview
This project is an **interactive Sales Analysis dashboard built in Microsoft Power BI**, designed with an app-like user experience and a scalable report structure. The report combines **advanced navigation**, **bookmark-driven views**, and a **star-schema data model** to help managers explore performance across key sales metrics.

## Key Features (UX + Report Engineering)
- **Layer grouping + naming conventions** for clean and maintainable report structure
- **Advanced bookmarking** to support multiple views within the same page
- Custom **navigation pane** and **interactive buttons** for guided exploration
- Report **backgrounds designed in PowerPoint**, with consistent layout using:
  - Alignment tools
  - Resizing tools (PowerPoint + Power BI)
- **Advanced slicer integration** for intuitive filtering
- **Drillthrough pages** for deeper detail without cluttering the main page
- **Tooltip pages** to provide context on hover
- Customisation of visuals (Cards, Charts, Sparklines, Tables, etc.)
- **Custom Power BI theme**
- Use of **icons / animated icons** to improve readability and engagement
- Applied **web/app-style layout principles** (home/help pages, headers, footers)

# Dataset and Data Preparation

## Dataset
The dataset contains two core tables:
- **Sales**
- **Managers**

## Data Preparation (Power Query)
The data was cleaned and reshaped in **Power Query** using transformations such as:
- Removing unnecessary columns  
- Grouping rows  
- Replacing values  
- Adding calculated columns  

To support reporting and analysis, I created:
- **Fact Sales** (main fact table)
- **Dim Managers** (dimension table built from the Managers table)
- **Dim Date** (date dimension derived from date fields in the fact table)

---

# Data Model

## Star Schema Design
The dashboard follows a **star schema** structure, with **Fact Sales** at the center connected to supporting dimensions.

### Fact Table
**Fact Sales**
- Core sales data for analysis  
- Includes fields such as: `YearMonth`, `Segment`, `Country`, `Product`, `DiscountBand`, etc.

### Dimension Tables
**Dim Managers**
- Includes: `ManagerID`, `Name`, `ImageURL`, etc.

**Dim Date**
- Includes: `ReportingPeriod`, `Year`, `Month`, `Quarter`

### Measures Table
A dedicated **Measures** table stores all **DAX measures** used across the report to keep calculations centralized and easy to maintain.

---

## Relationships
- **Fact Sales** connects to:
  - **Dim Date** (time-based analysis)
  - **Dim Managers** (manager-level analysis)

## Report Pages
Pages created in the report:
- **Home**
- **Sales Analysis**
- **Help**
- **Units Sold** (detail)
- **Net Sales** (detail)
- **Net Profit** (detail)
- **Cost of Goods (COGS)** (detail)
- **Tooltip: Units Sold**
- **Tooltip: Net Sales**
- **Tooltip: Net Profit**
- **Tooltip: COGS**

### Navigation Behavior
- Only **Home** and **Sales Analysis** are visible by default
- All other pages are **hidden** and accessible via **interactive buttons** from the main pages

## Page Details

### Home Page
- High-level KPI summary:
  - Units Sold
  - Net Sales
  - Cost of Goods (COGS)
  - Net Profit
- Button-based navigation to detailed pages
<img width="602" height="339" alt="image" src="https://github.com/user-attachments/assets/23843ff3-d3b8-4dc4-b1b4-51de433c6dcc" />

### Sales Analysis Page
- Detailed performance views for:
  - Units Sold
  - Net Sales
  - Cost of Goods (COGS)
  - Net Profit
- Breakdown by:
  - Period
  - Segment
  - Country
  - Product
- User filters:
  - Manager selection
  - Discount band selection (`High`, `Medium`, `Low`, `None`)

<img width="603" height="338" alt="image" src="https://github.com/user-attachments/assets/036b0a78-93e5-4b2b-bc3d-6c1cfc18b2f2" />
<img width="607" height="340" alt="image" src="https://github.com/user-attachments/assets/8ec44c5c-8d94-4bea-8a0d-8fc1f7755e7e" />
<img width="604" height="341" alt="image" src="https://github.com/user-attachments/assets/6c52da4e-c463-4616-87a7-050801928104" />
<img width="608" height="341" alt="image" src="https://github.com/user-attachments/assets/d579b447-50da-4297-ba4b-ead67e3338e1" />
<img width="608" height="339" alt="image" src="https://github.com/user-attachments/assets/958cd4c2-6c13-4e36-ae60-f9e8a7c42bfb" />

### Help Page
- A guidance page to support users/managers, including:
  - Report overview
  - Navigation instructions
  - How-to-use guidance

<img width="605" height="340" alt="image" src="https://github.com/user-attachments/assets/cf7df3c0-3b5a-47c1-af6c-1a829254902b" />

### Detail Pages (Units Sold / Net Sales / Net Profit / COGS)
- Accessible via **drillthrough** from the Sales Analysis page
- Allows managers to drill into a selected product for deeper insights

<img width="605" height="338" alt="image" src="https://github.com/user-attachments/assets/b1f3fd9d-96ed-4fa3-9aee-a8aaea827da6" />
<img width="606" height="338" alt="image" src="https://github.com/user-attachments/assets/a7b40af8-16a3-4e4e-9691-829b6acde81b" />
<img width="608" height="340" alt="image" src="https://github.com/user-attachments/assets/d62adedb-dcfb-4838-af98-def67e12e517" />
<img width="605" height="341" alt="image" src="https://github.com/user-attachments/assets/a9039741-28aa-45c1-affd-8a3cce1008ed" />

### Tooltip Pages
- Dedicated tooltips for each metric:
  - Units Sold
<img width="272" height="162" alt="image" src="https://github.com/user-attachments/assets/5360ea81-258a-4410-b58c-45c5c3202cea" />

  - Net Sales
<img width="275" height="163" alt="image" src="https://github.com/user-attachments/assets/aea0708e-cad6-4184-9af8-f118c72d4eb5" />

  - Net Profit
<img width="268" height="158" alt="image" src="https://github.com/user-attachments/assets/608325fd-746b-48cb-8c18-5bf37f2aa7ee" />

  - COGS
<img width="268" height="159" alt="image" src="https://github.com/user-attachments/assets/b0bcd49e-daa4-40d8-873f-871141b56050" />

- Shows **Top 5 managers** for the selected metric
- Appears when hovering over any data point on the Sales Analysis page

### Tools Used
- Excel (used to download and review the dataset)
- Power BI (data model, visuals, interactions)
- Power Query (data cleaning and reshaping)  
- Data modelling (Star Schema): Fact Sales + Dim Manager, Dim Date

## Notes
This README describes the report structure, modelling approach, and navigation experience. The Power BI file contains the full implementation (data model, DAX measures, report pages, bookmarks, tooltips, and drillthrough).

