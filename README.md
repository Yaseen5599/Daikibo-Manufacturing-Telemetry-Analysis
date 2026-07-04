# Daikibo Manufacturing Telemetry Analysis

## Overview

This project analyzes industrial IoT telemetry collected from four Daikibo manufacturing facilities during May 2021.

The objective was to identify:

- Which factory experienced the highest machine downtime.
- Which machine categories contributed most to downtime within that factory.

The dashboard was developed using Tableau.

---

## Dataset

The dataset contains telemetry messages generated every 10 minutes from machines across four manufacturing plants:

- Tokyo, Japan
- Osaka, Japan
- Berlin, Germany
- Shenzhen, China

Each location contains nine machine categories.

---

## Problem Statement

Daikibo wanted to monitor factory performance using telemetry collected from manufacturing equipment.

Business Questions:

1. Which factory experienced the highest downtime?
2. Which machine categories contributed most to downtime in that factory?

---

## Methodology

### Data Import

- Imported JSON telemetry data into Tableau.

### Data Transformation

Created a calculated field:

**Unhealthy**

IF [Status] = "unhealthy" THEN 10 ELSE 0 END


Each unhealthy message represents approximately 10 minutes of downtime.

### Dashboard Development

Built two interactive visualizations:

- Factory Downtime
- Machine Type Downtime

Implemented dashboard actions allowing users to select a factory and automatically filter the machine-level analysis.

---

## Dashboard Features

- Interactive filtering
- Factory comparison
- Machine category comparison
- Clear business-focused KPIs
- Simple navigation

---

## Tools Used

- Tableau
- JSON
- Data Visualization
- Calculated Fields

---

## Key Insights

- Identified the factory with the highest accumulated downtime.
- Identified machine categories responsible for the largest share of downtime.
- Demonstrated how telemetry data can support predictive maintenance and operational monitoring.

---

## Future Improvements

- Failure frequency analysis
- Mean Time Between Failures (MTBF)
- Predictive maintenance dashboard
- Time-series trend analysis
- Maintenance cost estimation
