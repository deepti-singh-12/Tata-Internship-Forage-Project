# Tata-Internship-Forage-Project
Power BI- Tata Internship Forage Project

## OVERVIEW:
The objective of this project is to analyze the online retail store’s data to identify the key factors contributing to revenue performance. Using data-driven techniques, the analysis focuses on sales trends, product performance, customer purchasing behavior, and retention patterns to generate actionable insights that support strategic planning and performance optimization for the upcoming year. Creating the Visualization for Senior Management (CEO and CMO).

## TOOLS USED: 
- Power BI for Visualization
- Power Query Editor to clean up the Data
- DAX for creating Columns and Measures

## DATA CLEANUP:
- The data contains some returns to the store which are provided in negative quantities and there are unit prices which were input in error. So, we must fix these errors before creating visuals:
    - a.	I have filtered out the negative quantities using power Query Editor as they are returned products
    - b.	To check for erroneous unit prices in the data by creating a calculated column using a DAX formula. Formula Used: UnitPrice Check = IF ( Online_Retail[UnitPrice] >= 0, "Valid", "Invalid" )
    - c.	We have calculated the revenue using Dax formula. Formula Used: Revenue = IF(Online_Retail[UnitPrice Check]= "Valid", Online_Retail[UnitPrice]* Online_Retail[Quantity], 0).

## BUSINESS QUESTIONS & VISUALS:
- **Q1. Revenue 2011:** Analysed monthly revenue patterns to identify seasonality and fluctuations, supporting demand forecasting and planning.
- **Q2. Top 10 Countries** (Excluding UK as per Client’s request): Identified the highest-contributing international markets by revenue and sales Quantity to highlight potential expansion opportunities.
- **Q3. Top 10 Customers:** To highlight the highest-value customers to support retention initiatives and targeted marketing strategies.
- **Q4. Product Demand by Region**(Excluding UK as per Client’s request): Visualized regional demand using a geographic map to help leadership prioritize high-demand markets and allocate resources effectively.

## OUTCOMES:
- Developed interactive Power BI dashboards as part of the Tata Forage simulation.
- Built data models and created DAX measures to track key KPIs including revenue, customer segmentation, seasonal trends and transaction trends.
- Translated business requirements into stakeholder-ready visualizations to support executive decision-making.

## DELIVERABLES:
- Tata Internship.pbix: Power BI report file containing all Visuals (.pbix)
- Certificate: From Forage Website.
