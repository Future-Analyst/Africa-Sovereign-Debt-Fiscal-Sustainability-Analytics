# Unraveling Africa's Sovereign Debt Crisis: Pathways to Sustainability

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black)
![Data Analysis](https://img.shields.io/badge/Focus-Economic%20%26%20Fiscal%20Analysis-2E8B57)
![Status](https://img.shields.io/badge/Status-Completed-blue)

![Dashboard Overview](Templates/dashboard%20overview.jfif)
## Project Overview

Why has sovereign debt become a major challenge for African economies, and what can historical economic data reveal about the path towards fiscal sustainability?

This project explores approximately 60 years of African economic and fiscal data to investigate the evolution of sovereign debt, examine the fiscal pressures associated with rising debt, and compare economic conditions across countries.

Using Microsoft Power BI, I transformed raw economic data into an interactive analytical report focused on debt trends, government revenue and expenditure, economic growth, inflation, and international trade.

The goal is to move beyond simply identifying countries with high debt and examine the broader fiscal and economic conditions that shape their capacity to manage public debt sustainably.

**Read the accompanying analysis:** [I Analysed 60 Years of African Economic Data: Here's What I Found About the Debt Crisis](https://medium.com/@achinikechigozie22/i-analysed-60-years-of-african-economic-data-heres-what-i-found-about-the-debt-crisis-621afe9c10b3)

## Project Objectives

- Examine the long-term evolution of sovereign debt across African countries.
- Identify countries experiencing rapid debt accumulation.
- Investigate the relationship between government revenue, expenditure, and fiscal deficits.
- Explore how economic growth and inflation relate to debt sustainability.
- Compare countries using fiscal and macroeconomic indicators.
- Develop evidence-based recommendations for strengthening public finance and debt management.

## Key Business Questions

1. How has sovereign debt evolved across African countries over time?
2. Are governments generating sufficient revenue to support public expenditure and manage debt?
3. How do economic growth, inflation, and trade performance relate to sovereign debt sustainability?
4. What fiscal and economic measures could support more sustainable debt management?

## Dataset

The analysis uses a historical dataset containing fiscal and economic observations for African countries.

| Field | Description |
|---|---|
| Country | Country associated with the observation |
| Country Code | Standardized country identifier |
| Indicator | Fiscal or economic metric |
| Source | Institution providing the data |
| Unit | Measurement unit |
| Currency | Currency associated with the observation |
| Frequency | Reporting frequency |
| Time | Observation date or period |
| Amount | Numeric observation |
| Value | Additional numeric or source-provided value |

The dataset includes indicators relating to government debt, revenue, expenditure, fiscal balance, GDP, inflation, VAT, imports, and exports.

The analysis uses the available historical coverage of each indicator. Data availability may differ across countries, indicators, and years.

## Tools and Technologies

- **Microsoft Power BI** — dashboard development, data visualization, and interactive analysis.
- **Power Query** — data cleaning, transformation, standardization, and preparation.
- **DAX** — analytical measures, year-over-year changes, growth rates, and fiscal comparisons.
- **Data Modeling** — fact and dimension tables organized using a star schema.

## Data Preparation and Modeling

Before building the report, the dataset was prepared for consistent analysis.

Key preparation steps included:

- Standardizing country names, country codes, indicator labels, and reporting periods.
- Checking missing values, duplicate observations, data types, and inconsistencies.
- Converting time fields into appropriate date formats.
- Separating descriptive attributes from numerical observations.
- Creating dimension tables for countries, indicators, dates, and data sources.
- Building a central fiscal fact table linked to the dimensions.
- Reviewing currencies and measurement units to ensure meaningful comparisons.

### Data Model

The model follows a star-schema structure, with FactFiscal connected to descriptive dimension tables.

- **FactFiscal:** numerical observations and foreign keys.
- **DimCountry:** country names and country codes.
- **DimIndicator:** indicator names and analytical categories.
- **DimDate:** dates and calendar attributes.
- **DimSource:** data providers.
- **DimUnit:** measurement units, where required.

Monetary indicators reported in different currencies or units must be standardized before being combined. Percentage indicators and monetary values are analyzed separately where their units differ.

## Power BI Dashboard

The report is organized into four analytical pages.

### 1. Sovereign Debt Landscape

**Business question:** How has sovereign debt evolved across African countries?

This page examines debt levels, historical trends, annual changes, and differences between countries.

Key analysis:
- Sovereign debt trends over time.
- Year-over-year debt growth.
- Country-level debt comparisons.
- Government debt in relation to GDP, where comparable data is available.

### 2. Fiscal Performance and Debt Drivers

**Business question:** Are government revenues sufficient to cover public expenditure?

This page investigates the fiscal conditions that can contribute to borrowing requirements.

Key analysis:
- Government revenue versus expenditure.
- Fiscal balance and budget deficits.
- Revenue and expenditure trends.
- VAT and domestic revenue indicators.

### 3. Economic Conditions and External Trade

**Business question:** How do economic growth, inflation, and trade conditions relate to debt sustainability?

This page examines the broader economic environment surrounding sovereign debt.

Key analysis:
- Real GDP and GDP growth.
- GDP per capita.
- Inflation and food inflation.
- Imports versus exports.
- Trade performance across countries.

### 4. Country Benchmarking and Sustainability Pathways

**Business question:** What distinguishes countries with improving debt outcomes from those facing increasing fiscal pressure?

This page brings together debt, fiscal, and economic indicators to support country comparisons and policy-relevant conclusions.

Key analysis:
- Comparative fiscal and debt indicators.
- Debt growth alongside revenue and economic growth.
- Country-level fiscal vulnerabilities.
- Potential pathways towards sustainable debt management.

## Key Analytical Measures

The report uses measures designed to compare fiscal performance over time and across countries.

| Measure | Purpose |
|---|---|
| Total Government Debt | Measures the recorded debt amount within the selected context |
| Year-over-Year Change | Measures the change from the previous comparable year |
| Debt Growth Rate | Tracks the percentage change in debt |
| Fiscal Balance | Compares government revenue with expenditure |
| Revenue Growth | Tracks changes in government revenue |
| Expenditure Growth | Tracks changes in government expenditure |
| Debt-to-GDP Ratio | Relates debt to the size of the economy, where compatible data is available |

**Important:** Debt stocks, annual fiscal flows, percentages, and values expressed in different currencies must not be added together as if they were the same measure.

## Key Findings

The findings from the historical analysis are documented in the accompanying article.

The main areas of investigation include:

- The long-term trajectory of sovereign debt across African economies.
- Differences in debt accumulation between countries.
- The relationship between fiscal deficits and government borrowing.
- The role of revenue generation and economic growth in debt sustainability.
- The influence of inflation and external trade conditions on fiscal pressures.

The interpretation of these patterns considers differences in country coverage, reporting periods, currencies, and indicator definitions.

For the detailed findings and supporting discussion, read the [full Medium article](https://medium.com/@achinikechigozie22/i-analysed-60-years-of-african-economic-data-heres-what-i-found-about-the-debt-crisis-621afe9c10b3).

## Policy Implications

The analysis provides a basis for exploring several pathways towards stronger debt sustainability:

1. **Strengthen domestic revenue mobilization:** Improve revenue collection and broaden the tax base, including through effective tax administration.
2. **Improve public expenditure efficiency:** Direct public resources towards productive investments and essential development priorities.
3. **Strengthen debt management:** Improve borrowing transparency, debt monitoring, and the assessment of repayment obligations.
4. **Support sustainable economic growth:** Encourage economic activity that can strengthen the government's long-term revenue capacity.
5. **Improve external resilience:** Strengthen export capacity and monitor exposure to external economic shocks.

These are policy directions to assess against the evidence; they are not automatic conclusions for every country.

## Limitations

- Historical data coverage varies by country, indicator, and year.
- Missing observations may affect country comparisons and trend calculations.
- Currency conversion and differences in measurement units can affect monetary comparisons.
- Aggregate debt amounts do not, by themselves, measure debt sustainability.
- Debt-to-GDP ratios, debt servicing capacity, borrowing costs, and the structure of debt provide additional context where available.
- Observed relationships between economic indicators do not establish causation.

## Repository Contents

```text
africa-sovereign-debt-analysis/
├── README.md
├── data/
│   └── dataset_reference.md
├── powerbi/
│   └── africa_sovereign_debt_analysis.pbix
├── screenshots/
│   ├── executive_overview.png
│   ├── fiscal_performance.png
│   ├── economic_trade_analysis.png
│   └── sustainability_pathways.png
└── docs/
    └── project_report.md
```

*This is the proposed repository structure. Include only files that are actually present in the repository. If the dataset is licensed or restricted, provide its source and access instructions rather than uploading it.*

## How to Explore the Project

1. Read the [accompanying Medium article](https://medium.com/@achinikechigozie22/i-analysed-60-years-of-african-economic-data-heres-what-i-found-about-the-debt-crisis-621afe9c10b3).
2. Open the Power BI report, if the `.pbix` file is available.
3. Explore the four report pages.
4. Use the country, year, and indicator filters to investigate differences across countries and periods.

## Conclusion

Africa's sovereign debt challenge cannot be understood through debt totals alone. Fiscal balances, revenue capacity, economic growth, inflation, and external trade all provide important context for understanding how governments manage their financial obligations.

By examining historical economic data through Power BI, this project aims to make complex fiscal patterns easier to explore, compare, and communicate.

The broader objective is to support a more informed discussion of sovereign debt sustainability and the policies that can help African economies balance development needs with responsible public finance.

## Author

**Achinike Chigozie**

Data Analyst | Economic and Fiscal Data Analysis | Power BI

- [Medium: Read the full analysis](https://medium.com/@achinikechigozie22/i-analysed-60-years-of-african-economic-data-heres-what-i-found-about-the-debt-crisis-621afe9c10b3)

---

*This project is intended for analytical and educational purposes. Findings should be interpreted in light of the dataset's coverage, definitions, and limitations.*
