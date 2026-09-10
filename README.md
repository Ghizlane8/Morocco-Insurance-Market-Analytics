# 🇲🇦 Morocco Insurance Market Analytics

> Interactive Power BI dashboard for analyzing the Moroccan non-life insurance market between 2022 and 2024.

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi)
![DAX](https://img.shields.io/badge/DAX-Measures-1E88E5?style=for-the-badge)
![Power Query](https://img.shields.io/badge/Power%20Query-ETL-217346?style=for-the-badge)
![Data](https://img.shields.io/badge/Data-Morocco%20Open%20Data-0D6ABF?style=for-the-badge)

---

## 📌 Project Overview

**Morocco Insurance Market Analytics** is an interactive Power BI project focused on the analysis of the Moroccan **non-life insurance market** over the period **2022–2024**.

The objective is to transform publicly available insurance data into a clear and interactive analytical dashboard that helps understand:

- the evolution of insurance premiums;
- the evolution of benefits and related expenses;
- the contribution of each insurance branch;
- the evolution of key technical ratios;
- the position of the automobile insurance branch;
- the main trends and business insights emerging from the market.

The project is designed as a **Data Analytics / Business Intelligence portfolio project**, combining data preparation, DAX modeling, visualization and business interpretation.


---

## 🔎 Key Findings

Based on the 2022–2024 market data:

- Total non-life insurance premiums increased from **MAD 29.1 billion in 2022** to **MAD 32.5 billion in 2024**.
- The automobile branch (`Véhicules terrestres à moteur`) generated **MAD 15.2 billion in premiums in 2024**.
- Automobile insurance represented approximately **46.7% of total non-life premiums in 2024**.
- Total benefits and expenses paid reached **MAD 20.9 billion in 2024**.
- The dashboard also tracks the evolution of benefits/premiums and charges/premiums ratios.
  
---

## 🎯 Business Question

> **How did the Moroccan non-life insurance market evolve between 2022 and 2024, and which insurance branches contributed most to this evolution?**

A specific focus is also dedicated to the **automobile insurance branch**, one of the most significant branches in the analyzed market.

---

## 📊 Dashboard Structure

The report is organized into four analytical pages.

### 01 — Market Overview

Provides a high-level view of the Moroccan non-life insurance market.

Main elements include:

- Total premiums
- Total benefits
- Total charges
- Benefits / premiums ratio
- Charges / premiums ratio
- Market evolution from 2022 to 2024
- Premium distribution by insurance branch
- Top branches
- Market growth indicators
- Ratio evolution over time
- Number of analyzed insurance branches

This page provides the overall market perspective before moving into more detailed analysis.

---

### 02 — Branch Analysis

Provides a detailed comparison between the different insurance branches.

Features include:

- Branch ranking
- Indicator selector
- Premiums
- Benefits
- Charges
- Benefits / premiums ratio
- Charges / premiums ratio
- Branch evolution from 2022 to 2024
- Dynamic Top 5 / Top 10 / all branches selection
- Market share analysis
- Focus indicators for the leading branches

The indicator selector allows the same analytical framework to be used for different measures.

---

### 03 — Automobile Focus

A dedicated analysis of the branch:

> **Véhicules terrestres à moteur**

The page analyzes:

- Automobile premiums
- Automobile benefits
- Automobile charges
- Benefits / premiums ratio
- Charges / premiums ratio
- Evolution from 2022 to 2024
- Evolution of automobile technical ratios
- Automobile contribution to the overall market
- Key automobile insights

The page allows the user to explore the automobile branch while keeping the historical 2022–2024 perspective.

---

### 04 — Insights & Key Takeaways

The final page translates the analysis into business-oriented conclusions.

It contains four main sections:

#### Résumé des performances

- Premium growth
- Benefits growth
- Charges growth
- Benefits / premiums ratio
- Charges / premiums ratio

#### Les messages clés

The main conclusions derived from the market analysis, including:

- overall market growth;
- evolution of benefits and charges;
- importance of the automobile branch;
- dynamics of the most active branches;
- importance of monitoring technical indicators.

#### Perspectives

The dashboard highlights four areas of strategic attention:

- **Poursuite de la digitalisation des processus et de la relation client**
- **Renforcement de la prévention et de la maîtrise des sinistres**
- **Développement de nouveaux produits et services innovants**
- **Amélioration de l'expérience client et de la satisfaction**

#### Définition des indicateurs

The main indicators are documented directly in the dashboard:

- **Primes** — total amount of premiums issued by insurance companies.
- **Prestations** — total amount of benefits/indemnifications paid to policyholders.
- **Charges** — total amount of technical charges related to benefits.
- **Ratio Prestations / Primes** — benefits divided by premiums.
- **Ratio Charges / Primes** — charges divided by premiums.

---

## 📈 Key Indicators

The dashboard uses several core KPIs.

### Total Premiums

Measures the total premiums generated by the non-life insurance market.

### Total Benefits

Measures the total benefits paid by the market.

### Total Charges

Measures the total charges related to benefits.

### Benefits / Premiums Ratio

```text
Benefits / Premiums
```
This indicator helps monitor the relationship between benefits paid and premiums generated.

### Charges / Premiums Ratio
```text
Charges / Premiums
```
This indicator provides an additional view of the relationship between technical charges and premiums.

### Market Share

The project also calculates the contribution of each insurance branch to total market premiums.

---

## 🔄 Data Preparation

The source datasets were transformed using **Power Query**.

The main preparation steps were:

1. Import the three Morocco Open Data datasets.
2. Remove total rows where required.
3. Promote the correct headers.
4. Standardize column names.
5. Transform yearly columns into rows.
6. Convert the year into an integer.
7. Convert numerical values using the appropriate locale.
8. Handle unavailable values represented by -.
9. Merge premiums, benefits and charges.
10. Match records using:
   - Insurance branch
  - Year
11. Validate the resulting dataset.
12. Load the final analytical table into Power BI.

The resulting analytical structure contains:
```text
Branche
Année
Primes
Prestations
Charges
```

---

## 🗂️ Data Model

The main analytical table used by the report is:
```text
Insurance_Market
```

with the following fields:

| Field       | Description      |
| ----------- | ---------------- |
| Branche     | Insurance branch |
| Année       | Year             |
| Primes      | Premiums         |
| Prestations | Benefits         |
| Charges     | Charges          |

Additional supporting tables/measures are used for:

- indicator selection;
- automobile analysis;
- dynamic Top N selection;
- dashboard calculations.


## 🛠️ Technologies Used
**Power BI**

Used for:

- dashboard development;
- interactive visualizations;
- KPI cards;
- slicers;
- charts;
- analytical storytelling.
  
**Power Query**

Used for:

- data cleaning;
- transformation;
- reshaping;
- merging datasets;
- preparation of the analytical model.

**DAX**

Used for:
- calculated measures;
- growth calculations;
- ratios;
- rankings;
- market shares;
- dynamic selections;
- automobile analysis.

---

## 🎨 Dashboard Design

The dashboard follows a consistent visual identity inspired by the Moroccan insurance context.

**Main design elements**
- 🇲🇦 Moroccan flag
- Dark navy navigation sidebar
- Blue and turquoise analytical palette
- White KPI cards
- Rounded visual containers
- Consistent typography
- Interactive filters
- Insurance-related icons
- Moroccan skyline illustration

The objective was to combine business readability with a professional Power BI portfolio aesthetic.

---

## 📊 Data Sources

This project uses three official datasets from the Moroccan Open Data platform (`data.gov.ma`), covering the non-life insurance market for 2022–2024.

### 🇲🇦 Morocco Open Data — Premiums

**Évolution des primes émises en assurance non-vie — 2022–2024**

Source: Morocco Open Data

[View dataset](https://www.data.gov.ma/data/dataset/evolution-des-primes-emises-en-assurance-non-vie)

---

### 🇲🇦 Morocco Open Data — Benefits

**Évolution des prestations et frais payés en assurance non-vie — 2022–2024**

Source: Morocco Open Data

[View dataset](https://www.data.gov.ma/data/dataset/evolution-des-prestations-et-frais-payes-en-assurance-non-vie)

---

### 🇲🇦 Morocco Open Data — Charges

**Évolution des charges de prestations en assurance non-vie — 2022–2024**

Source: Morocco Open Data

[View dataset](https://www.data.gov.ma/data/dataset/evolution-des-charges-de-prestations-en-assurance-non-vie)

---

### Data Coverage

The three datasets provide aggregated market-level information by insurance branch for:

- **2022**
- **2023**
- **2024**

The analysis combines these datasets using:

- **Insurance branch (`Branche`)**
- **Year (`Année`)**

The resulting analytical table contains:

| Field | Description |
|---|---|
| `Branche` | Non-life insurance branch |
| `Année` | Year |
| `Primes` | Premiums issued |
| `Prestations` | Benefits and expenses paid |
| `Charges` | Benefits-related charges |

> **Note:** The analysis is based exclusively on these three public datasets. No customer-level, policy-level, company-level, regional, or guarantee-level data is used.

---

## 💡 Key Takeaways

The dashboard provides a structured view of the Moroccan non-life insurance market and highlights:

- the evolution of premiums between 2022 and 2024;
- differences between premiums, benefits and charges;
- the relative contribution of insurance branches;
- the importance of the automobile branch;
- the evolution of benefits/premiums and charges/premiums ratios;
- branches showing stronger growth dynamics.

The automobile branch receives particular attention because of its significant contribution to the overall non-life insurance market.

---

## ⚠️ Limitations

This project is based on aggregated public market data covering only three years (2022–2024).

The available datasets do not provide:

- Customer-level information
- Individual policy data
- Insurance company-level data
- Regional or city-level breakdowns
- Individual claim records
- Guarantee-level breakdowns within the automobile branch

Therefore, the dashboard focuses on **market-level analysis by insurance branch and year**.

The automobile analysis is based on the aggregate branch **“Véhicules terrestres à moteur”** and does not provide a breakdown by individual guarantees such as RC, dommages or assistance.


---
## 🚀 Potential Future Improvements

The project could be extended with additional datasets to enable:

- analysis by insurance company;
- regional analysis;
- claims frequency and severity;
- automobile guarantee-level analysis;
- customer segmentation;
- fraud detection;
- forecasting;
- predictive analytics;
- interactive scenario analysis;
- automated data refresh.

## 📁 Repository Structure

A recommended GitHub repository structure is:

```text
Morocco-Insurance-Market-Analytics/
│
├── 📊 Morocco Insurance Market Analytics.pbix
│
├── 📁 data/
│   ├── primes_non_vie.xlsx
│   ├── prestations_non_vie.xlsx
│   └── charges_non_vie.xlsx
│
└── README.md
```

---

## 🧩 What I Built

This project demonstrates the ability to:

- Build an analytical data model from multiple datasets
- Perform ETL transformations with Power Query
- Create reusable DAX measures
- Implement dynamic KPI calculations
- Build dynamic Top N analysis
- Calculate market shares and technical ratios
- Design interactive Power BI dashboards
- Translate quantitative results into business insights

---

## 👩‍💻 Author

**Ghizlane Baali**

Data Analytics | Power BI | DAX | Power Query | Python

📧 **Email:** [baali.ghizlane2@gmail.com](mailto:baali.ghizlane2@gmail.com)

💼 **LinkedIn:** [linkedin.com/in/ghizlane-baali-a42505267](https://www.linkedin.com/in/ghizlane-baali-a42505267/)

---

<div align="center">

⭐ **If you find this project interesting, feel free to explore the dashboard and the analytical approach.**

</div>
