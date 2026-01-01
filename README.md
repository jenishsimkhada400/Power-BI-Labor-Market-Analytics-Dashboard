# Unemployment Rate Analysis Dashboard (Power BI)

## Project Overview
This project is an interactive **Power BI dashboard** designed to analyze unemployment trends over time across different **geographic regions, industries, and demographic groups**. The goal of this project is to demonstrate strong **data modeling, analytical thinking, and data storytelling skills** using a star-schema-based semantic model.

The dashboard allows users to explore how unemployment rates change by year and understand the relationships between economic indicators and population characteristics.

---

## 🎯 Objectives
- Analyze unemployment trends over multiple years  
- Enable filtering by **date, geography, industry, and demographics**  
- Demonstrate proper **fact and dimension modeling** in Power BI  
- Provide clear insights through clean and intuitive visualizations  

---

## Data Model Overview
The project follows a **star schema** design for performance and clarity.

### Fact Table
**`unemployment_statistics_FactTable`**
- Core measurements:
  - `unemployment_rate`
  - `employed`
  - `unemployed`
  - `labor_force`
  - `participation_rate`
  - `employment_population_ratio`
- Foreign keys linking to dimension tables:
  - `date_id`
  - `geography_id`
  - `industry_id`
  - `demographic_id`

This table serves as the central source of numerical data for all visuals.

---

### Dimension Tables
- **Date**
  - Enables time-based analysis (Year, Quarter, Month)
- **Geography**
  - Allows comparison across states, counties, regions, and metro areas
- **Industry**
  - Breaks unemployment data down by industry sector and wage levels
- **Demography**
  - Supports demographic analysis such as age group, education, gender, and race/ethnicity

Each dimension has a **one-to-many relationship** with the fact table.

---

## Dashboard – Page 1 Explanation
### “Unemployment Rate by Year”
- Displays unemployment trends over time
- Uses `full_date (Year)` on the X-axis
- Uses aggregated `unemployment_rate` on the Y-axis
- Helps identify economic shifts such as recessions or recoveries

This page is designed to give users a **high-level macro view** before drilling into specific groups.

---

## Key Insights
- Unemployment rates fluctuate significantly during major economic periods
- Time-based analysis helps highlight recovery trends after economic downturns
- The model structure allows seamless drill-down into demographic or industry-specific unemployment patterns

---

## Tools & Technologies
- **Power BI Desktop**
- **DAX** (for measures and aggregations)
- **Star Schema Data Modeling**
- **Interactive Visualizations**

---

## 📁 Repository Structure
