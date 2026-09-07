# Cyber Incident Analytics | Power BI

## Project Overview

Cyber Incident Analytics is an interactive Power BI project designed to analyze global cyber incidents,
 attack patterns, affected entities, receiver information, attribution, and incident impact.

The dashboard helps identify cyber risk trends, high-impact incidents, targeted entities,
 and attribution patterns through interactive visualizations and KPIs.

## Tools & Technologies

- Power BI
- Power Query
- DAX
- SQL
- Excel
- Data Modeling

## Project Structure

```text
Cyber_Incident_Analytics_project
│
├── Raw_Data
│   ├── eurepoc_attribution_dataset_1.3.csv
│   ├── eurepoc_dyadic_dataset_0_1.csv
│   ├── eurepoc_global_dataset_1_3.csv
│   └── eurepoc_receiver_dataset_1.3.csv
│
├── Data_Cleaning
│   └── Power_query_steps.md
│
├── Data_Model
│   └── Data_Model.png
│
├── Dax
│   └── Measure.md
│
├── screenshots
│   ├── Executive Cyber Risk Dashboard.png
│   ├── Cyber Attack & Trend Analysis.png
│   ├── Receiver Analysis.png
│   └── Attribution Analytics.png
│
└── README.md 

## Key KPIs

- Total Incidents
- Incidents with Parsed Start Date
- Incidents Having Receiver Data
- Distinct Receiver Entities
- Average Impact Score
- High Impact Incidents
- Attributed Incidents
- Attribution %

## Dashboard Analysis

### Executive Cyber Risk Dashboard

Provides an overview of overall cyber incident activity, impact levels, and key risk indicators.

![Executive Cyber Risk Dashboard](screenshots/Executive%20Cyber%20Risk%20Dashboard.png)

### Cyber Attack & Trend Analysis

Analyzes incident trends, attack patterns, operation types, and changes over time.

![Cyber Attack & Trend Analysis](screenshots/Cyber%20Attack%20%26%20Trend%20Analysis.png)

### Receiver Analysis

Analyzes targeted receiver entities and the distribution of incidents across affected entities.

![Receiver Analysis](screenshots/Receiver%20Analysis.png)

### Attribution Analytics

Analyzes incident attribution patterns and the availability of attribution information.

![Attribution Analytics](screenshots/Attribution%20Analytics.png)

## Data Cleaning & Transformation

Data was cleaned and transformed using Power Query. Key steps included:

- Promoting headers
- Changing data types
- Parsing date fields
- Handling missing values
- Validating incident IDs
- Standardizing columns
- Preparing tables for data modeling

Detailed transformation steps are documented in:

`Data_Cleaning/Power_query_steps.md`

## Data Model

The project uses a relational Power BI data model connecting incident data with receiver, attribution, 
impact, and other analytical datasets.

![Power BI Data Model](Data_Model/Data_Model.png)

## DAX Measures

DAX measures were created to calculate key incident and risk metrics, including Total Incidents, 
High Impact Incidents, Average Impact Score, Attributed Incidents, and Attribution %.

Detailed measures are documented in:

`Dax/Measure.md`

## Business Insights

- Identified trends in global cyber incident activity.
- Analyzed high-impact cyber incidents.
- Evaluated targeted receiver entities.
- Analyzed incident attribution patterns.
- Used KPIs and interactive filters to support cyber risk analysis.

## Project Outcome

This project demonstrates practical skills in Power BI, Power Query, DAX, data modeling, data cleaning, 
and business-oriented cyber incident analysis.

## Author

**Sanket V Shingney**

Data Analyst | Power BI | SQL | Excel | DAX | Power Query