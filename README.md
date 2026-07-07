# Tableau Marketing Performance Dashboard

## Project Overview
An end-to-end marketing analytics project demonstrating the complete Business Intelligence workflow: extracting and preparing advertising data with SQL, building an analytical dataset, and developing an interactive marketing dashboard in Tableau Public.

### About the Project

This project demonstrates the development of an interactive marketing performance dashboard in Tableau Public based on advertising campaign data from Facebook Ads and Google Ads.

The project simulates a real-world marketing analytics workflow where campaign data is stored in a relational database across multiple tables. Before building the dashboard, the data was explored, joined, cleaned, aggregated with SQL, exported as a CSV file, and then visualized in Tableau Public.

The final dashboard helps analyze advertising efficiency, campaign performance, marketing funnel effectiveness, and the relationship between advertising spend and lead generation.

---

## Dashboard Screenshot

Dashboard Preview see here  /tableau/screenshots/marketing_dashboard_overview.png

## Business Questions

The dashboard is designed to answer the following business questions:

* Which advertising campaigns generate the best marketing performance?
* How do Facebook Ads and Google Ads compare?
* How do advertising spend and lead generation change over time?
* Does increasing the advertising budget result in more leads?
* Which campaigns have the highest Return on Marketing Investment (ROMI)?
* Which campaigns are the most cost-efficient?
* How do CTR, CPC, CPM, CPL and conversion rates evolve over time?
* Which UTM campaigns contribute the most to marketing success?

---

## Tech Stack

### Database
* PostgreSQL
### Querying & Data Preparation
* SQL
* DBeaver
### Business Intelligence
* Tableau Public
### Data Processing
* CSV
### Analytics Techniques
* Data Cleaning
* Data Integration
* Marketing KPI Analysis
* LOD Expressions
* Parameters
* Dashboard Actions
* Correlation Analysis

---

## Main Features

### SQL Data Preparation
Description of the data sources for the project see: `data/README.md`

Data preparation was performed in SQL using DBeaver.

Advertising data from Facebook Ads and Google Ads was explored, joined, cleaned, standardized, and exported to a unified analytical dataset using SQL.

For a detailed description of the ETL process, see: `docs/data_preparation.md`

### Tableau Analytics

Created custom marketing metrics:

- CTR
- CPC
- CPM
- CPL
- ROMI
- Clicks-to-Leads Conversion
- Reach-to-Leads Conversion

Implemented advanced Tableau functionality:

- FIXED LOD expressions
- Dynamic parameter switching
- Correlation analysis
- Dashboard filter actions
- Interactive cross-filtering

Complete formulas are documented in: `docs/calculated_fields.md`

### Dashboard Structure

The dashboard contains:

- KPI overview
- Spend vs Leads Analysis (Dual Axis)
- Metric Trend
- Campaign Ranking
- Campaign Efficiency Analysis  (Scatter Plot)

More details: `docs/dashboard_design.md`

---

## Repository Structure
```
tableau-marketing-performance-dashboard/
│
├── README.md
├── LICENSE
│
├── sql/
│   ├── final_dataset_query.sql
│   └── data_exploration_queries.sql
│
├── data/
│   ├── marketing_ads_dataset.csv
|   ├── raw/
|   ├── processed/
|   └── README.md
│
├── tableau/
│   ├── dashboard_link.txt
│   └── screenshots/
│
└── docs/
|   ├── business_case.md
|   ├── data_preparation.md
|   ├── calculated_fields.md
|   └── dashboard_design.md
```
---

## Documentation

Additional project documentation is available in the `docs` directory.

| Document |	Description |
| :---: | :---: |
|business_case.md |	Business objectives, stakeholders, and analytical goals 
|data_preparation.md |	SQL workflow, data integration, cleaning, and transformation process |
|calculated_fields.md |	Tableau calculated fields, LOD expressions, parameters, and formulas |
|dashboard_design.md |	Dashboard layout, visualization choices, interactions, and user experience |
|insights.md |	Business insights and analytical conclusions derived from the dashboard |

---

## Skills Demonstrated

This project demonstrates practical skills in:

* SQL data preparation;
* working with relational databases;
* joining fact and dimension tables;
* data cleaning with `COALESCE`;
* UTM parameter extraction and decoding;
* CSV export for BI tools;
* Tableau Public dashboard development;
* calculated fields;
* parameters;
* FIXED LOD expressions;
* correlation analysis;
* dual-axis charts;
* scatter plot analysis;
* dashboard actions;
* interactive marketing analytics.

---

## Tools Used

* PostgreSQL
* DBeaver
* SQL
* Tableau Public
* CSV

---

## Author

Nadia Kamenski

Aspiring Data Analyst focused on Power BI, SQL, Tableau Public, marketing analytics, analytics engineering, business intelligence solutions and dashboard storytelling.
