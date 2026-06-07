# Deloitte Australia Data Analytics Job Simulation

This repository contains my completed work for the Deloitte Australia Data Analytics Job Simulation on Forage. The simulation focused on using data analysis, Tableau, and Excel to support business decision making for Daikibo Industrials.

## Project Overview

Daikibo Industrials collected operational and employee data from multiple factory locations. The project had two main parts:

1. Analyze machine telemetry data to identify factory downtime.
2. Classify gender pay equality scores using Excel.

The goal was to turn raw data into clear insights that could help the business understand operational issues and employee compensation patterns.

## Business Questions

The project focused on answering the following questions:

* Which factory location had the highest machine downtime?
* Which machine types contributed most to downtime in that location?
* Which job roles showed fair, unfair, or highly discriminative gender pay equality scores?

## Task 1: Telemetry Data Analysis

Daikibo collected telemetry data from four factory locations:

* Daikibo Factory Meiyo, Tokyo, Japan
* Daikibo Factory Seiko, Osaka, Japan
* Daikibo Berlin, Berlin, Germany
* Daikibo Shenzhen, Shenzhen, China

Each factory had multiple machine types sending telemetry messages every 10 minutes. I used Tableau to analyze machine status and identify downtime patterns.

### Tableau Work Completed

* Imported the telemetry JSON file into Tableau.
* Created a calculated field called `Unhealthy`.
* Assigned 10 minutes of downtime to every unhealthy machine status.
* Built a bar chart showing downtime by factory.
* Built a second bar chart showing downtime by device type.
* Created an interactive dashboard where selecting a factory filters the device type downtime chart.

### Key Insight

The dashboard helped identify the factory with the highest downtime and the machine types that contributed most to operational issues.

## Task 2: Forensic Technology Analysis

The second task focused on gender pay equality across job roles and factory locations.

The Excel file contained:

* Factory
* Job Role
* Equality Score

I created a fourth column called `Equality class` to classify each score.

### Classification Logic

| Equality Score                    | Equality Class        |
| --------------------------------- | --------------------- |
| Between -10 and +10               | Fair                  |
| Less than -10 or greater than +10 | Unfair                |
| Less than -20 or greater than +20 | Highly Discriminative |

### Excel Formula Used

```excel
=IF(ABS(C2)<=10,"Fair",IF(ABS(C2)<=20,"Unfair","Highly Discriminative"))
```

This formula classified each job role based on how far the equality score was from zero.

## Tools Used

* Tableau
* Microsoft Excel
* JSON data analysis
* Data visualization
* Calculated fields
* Excel formulas

## Skills Demonstrated

* Data analysis
* Dashboard creation
* Business intelligence reporting
* Excel based classification
* Data cleaning and transformation
* Forensic data review
* Business insight generation

## Repository Contents

```text
deloitte-daikibo-data-forensics-simulation/
│
├── README.md
├── dashboard/
│   └── daikibo_tableau_dashboard.png
├── excel/
│   └── equality_table_completed.xlsx
└── insights/
    └── summary.md
```

## Project Summary

This simulation helped me practice analyzing business data and communicating insights through dashboards and structured Excel analysis. The Tableau dashboard supported operational decision making by showing machine downtime patterns, while the Excel classification task supported a forensic review of gender pay equality.

## Note

This project was completed as part of the Deloitte Australia Data Analytics Job Simulation on Forage. The original task materials and datasets belong to Forage and Deloitte. This repository is intended to showcase my completed analysis, dashboard, and learning outcomes.
