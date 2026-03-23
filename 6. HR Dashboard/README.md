# HR Data Insights Dashboard

## Overview
In today’s fast-changing workplace, organisations face ongoing challenges in understanding and managing their workforce effectively. HR teams are expected to closely monitor key workforce metrics such as headcount, retention, and turnover. Without clear visibility into these areas, businesses may face higher recruitment costs, reduced employee morale, and critical talent gaps.

# Workforce Retention Recommendations

- **Reduce Customer Service turnover to lower replacement costs**  
  With Customer Service turnover at 36.4%, the business should compare the cost of replacing staff against the cost of targeted retention initiatives.

- **Stabilise management to avoid productivity losses**  
  Manager turnover of 32.8% may create hidden costs through weaker supervision, disrupted workflows, and lower team performance.

- **Focus on retention where voluntary turnover is high**  
  Since 81% of exits are voluntary, improving employee value propositions may be more cost-effective than repeated recruitment and onboarding.

- **Assess remote work through a cost–benefit lens**  
  With 80% of employees working remotely, the organisation should review whether remote arrangements are improving retention while also reducing operating costs.

- **Continue investing in strategies with proven long-term value**  
  Since retention stayed above 90% and rose to 97.3% in 2019, management should identify which practices most effectively reduced turnover and continue supporting those that generated the greatest long-term value through lower replacement costs, stronger productivity, and better workforce stability.

## Objective
This project aims to build an intuitive and interactive **Power BI dashboard** that provides HR professionals with instant visibility into workforce dynamics. The goal is to support better decision-making around staffing, employee engagement, and retention strategies.

## Dataset
The dashboard is built using the following datasets:

### People Employment History
- Employee ID  
- First name  
- Last name  
- Department  
- Sub-department  
- First-level manager  
- Second-level manager  
- Third-level manager  
- Fourth-level manager  
- Job level  
- Salary  
- Hire date  
- Termination date  
- Termination reason  

### People Data
- Employee ID  
- Gender  
- Race  
- Birth date  
- Education  
- Location  
- City  
- Marital status  
- Employment status

### Dates
- Date  
- Year  
- Month  
- Day  
- Weekday  
- Other related calendar fields  

## Data Preparation (Power Query)
The data was cleaned and transformed in **Power Query** through a range of preparation steps, including:

- Merging queries  
- Removing unnecessary columns  
- Eliminating duplicates  
- Filtering rows  
- Unpivoting and splitting columns  
- Standardising fields  

To support analysis, I developed **one people fact table** and **eight dimension tables**:

- Demographic  
- Department  
- Education  
- Job Level  
- Location  
- Manager  
- Marital  
- Termination  

## Dashboard Structure

### 1. Cover Page
The cover page introduces the purpose of the dashboard and provides clear navigation to the three main sections:

- Headcount  
- Retention  
- Turnover  

![this is image](https://github.com/tuenguyen1508-lang/Power-BI-Projects/blob/11632df6a995548675eff2a5a63f7e74ea845197/6.%20HR%20Dashboard/Dataset/images/Screenshot%202026-03-13%20163022.png)

### 2. Headcount Analysis
This section helps users understand workforce composition through breakdowns by department, job level, location, and demographics such as gender, age, race, education, and marital status. Custom slicers allow flexible exploration of employee attributes, while a tooltip feature highlights the **Top 20 highest and lowest earners** for salary analysis.

**Reporting period:** 2013–2019

#### Key Insights
- Total headcount reached **2,796 employees in 2019**  
- The **Software** department recorded the highest number of employees at **543**  
- **80% of employees worked remotely**  
- **Individual Contributors** represented the largest job group with **2,094 employees**  
- **Male employees** accounted for **61%** of headcount  
- Employees aged **43** had the highest count at **146**  
- **Caucasian employees** represented **74.71%** of headcount  
- Employees with a **Bachelor’s degree** and those who were **single** formed the majority

![this is image](https://github.com/tuenguyen1508-lang/Power-BI-Projects/blob/11632df6a995548675eff2a5a63f7e74ea845197/6.%20HR%20Dashboard/Dataset/images/Screenshot%202026-03-13%20163135.png)

![this is image](https://github.com/tuenguyen1508-lang/Power-BI-Projects/blob/11632df6a995548675eff2a5a63f7e74ea845197/6.%20HR%20Dashboard/Dataset/images/Screenshot%202026-03-13%20163153.png)

![this is image](https://github.com/tuenguyen1508-lang/Power-BI-Projects/blob/11632df6a995548675eff2a5a63f7e74ea845197/6.%20HR%20Dashboard/Dataset/images/Screenshot%202026-03-13%20163240.png)

### 3. Retention Insights
Retention analysis goes beyond measuring how many employees stay — it helps explain where retention is strongest and where improvement may be needed. This section tracks year-over-year retention trends and allows comparison across job levels, departments, and education groups.

**Reporting period:** 2013–2019

#### Key Insights
- Overall employee retention was **83.6%**  
- Starting headcount was **409**  
- Ending headcount was **342**  
- Annual retention remained **above 90%** throughout the period  
- Retention peaked at **97.3% in 2019**  
- **Team Leads** recorded the highest retention at **91.8%**  
- The **Operations** department recorded the strongest departmental retention at **89.2%**  
- The most significant retention changes were observed in the **Other gender group**, employees with an **Associate degree**, and the **60–69 age group**
 
![this is image](https://github.com/tuenguyen1508-lang/Power-BI-Projects/blob/11632df6a995548675eff2a5a63f7e74ea845197/6.%20HR%20Dashboard/Dataset/images/Screenshot%202026-03-13%20163638.png)

### 4. Turnover Analysis
Employee turnover can be costly, making it essential for organisations to understand how often employees leave, where turnover is highest, and why exits occur. This section answers questions around annual turnover rates, turnover by department and job level, voluntary versus involuntary exits, and the most common reasons for leaving.

**Reporting period:** 2013–2019

#### Key Insights
- Overall employee turnover was **28.5%**  
- This was based on **457 departing employees**  
- The average workforce size was **1,602 employees**  
- Turnover declined gradually from **2014 to 2019**  
- **Managers** had the highest turnover by job level at **32.8%**  
- **Customer Service** experienced the highest departmental turnover at **36.4%**  
- **81% of turnover was voluntary**  
- The most common reasons for leaving were **better benefits flexibility** and **better career opportunities**

![this is image](https://github.com/tuenguyen1508-lang/Power-BI-Projects/blob/11632df6a995548675eff2a5a63f7e74ea845197/6.%20HR%20Dashboard/Dataset/images/Screenshot%202026-03-13%20164126.png)

## Tools Used
- **Excel** — Downloading and reviewing the dataset  
- **Power BI** — Data modelling, visualisation, interactivity, and navigation  
- **Power Query** — Data cleaning and transformation  
- **Data Modelling** — Star-schema style modelling using fact and dimension tables  

## Notes
The dashboard was designed to be clear, intuitive, and accessible for both technical and non-technical stakeholders. Its focus is on delivering actionable insights, enabling easy exploration, and supporting practical HR decision-making.
