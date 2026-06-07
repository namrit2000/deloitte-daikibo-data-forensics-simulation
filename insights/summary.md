# Project Summary

This simulation involved two main analytics tasks for Daikibo Industrials: factory telemetry analysis and forensic technology analysis.

## Telemetry Analysis

I used Tableau to analyze machine health telemetry from four Daikibo factory locations. The goal was to identify which factory had the highest machine downtime and which device types contributed most to downtime.

I created a calculated field where every unhealthy machine status represented 10 minutes of potential downtime. Then, I built a dashboard with two charts:

* Down Time per Factory
* Down Time per Device Type

The dashboard allowed factory level filtering, so selecting a factory showed only the device type downtime for that location.

## Forensic Technology Analysis

I used Excel to classify gender pay equality scores across factory locations and job roles. The dataset included factory name, job role, and equality score.

I created a new column called Equality class and classified each score using conditional logic:

* Fair: score between -10 and +10
* Unfair: score less than -10 or greater than +10
* Highly Discriminative: score less than -20 or greater than +20

## Tools Used

* Tableau
* Microsoft Excel

## Key Takeaway

This project helped turn raw operational and compensation data into clear business insights. Tableau was used to identify downtime patterns, while Excel was used to classify equality risk levels across job roles.
