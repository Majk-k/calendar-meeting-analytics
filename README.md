# Calendar Meeting Analytics Dashboard (PBIP Project)

This repository contains a Power BI Project (PBIP) used for analyzing
organizational meeting patterns.\
The report helps understand meeting sizes, frequency, duration,
organizational structure involvement, and behavioral clusters.

------------------------------------------------------------------------

##  Dashboard Preview
![Dashboard Overview](docs/dashboard.png)\
![Model Diagram](docs/model.png)\
![Filters View](docs/filters.png)

------------------------------------------------------------------------

##  Key Features

-   Monthly meeting duration trend\
-   Breakdown by meeting size (small / medium / large)\
-   Distribution of meetings across organizational levels\
-   Behavioral clusters for deeper insights\
-   Fully interactive layout and filters\
-   Clean and optimized semantic model

------------------------------------------------------------------------

##  Architecture

This PBIP project follows a standard Power BI development flow:

    Data Source
        ↓
    Semantic Model (TMDL – tables, relationships, formatting)
        ↓
    Report Layer (PBIR – pages, visuals, layout, filters)
        ↓
    End Users (Power BI Service)

------------------------------------------------------------------------

## Directory Structure

    calendar-meeting-analytics/
    │
    ├─ Calendar Analysis Report.pbip
    │
    ├─ Calendar Analysis Report.SemanticModel/
    │   ├─ .pbi/
    │   ├─ definition/
    │   │   ├─ database.tmdl
    │   │   ├─ model.tmdl
    │   │   ├─ relationships.tmdl
    │   │   └─ tables/*.tmdl
    │   └─ cultures/en-US.tmdl
    │
    ├─ Calendar Analysis Report.Report/
    │   └─ definition/
    │       ├─ report.json
    │       ├─ pages/*.json
    │       └─ visuals/*.json
    │
    └─ docs/
        ├─ dashboard.png
        ├─ model.png
        └─ filters.png

------------------------------------------------------------------------

## How to Use

### **Open the project**

1.  Clone the repo:

        git clone <repository-url>

2.  Open `Calendar Analysis Report.pbip` in Power BI Desktop.

### **Refresh the data**

-   Connect your dataset\
-   Update data source paths if required

------------------------------------------------------------------------

## Motivation

This project was created to analyze and optimize the calendar of executive manager.\
It provides visibility into:
 - how much meeting time teams spend
monthly, 
- how meeting sizes evolve, 
- which org levels participate the
most, 
- opportunities to reduce unnecessary meeting load.

------------------------------------------------------------------------

##  Tech Stack

-   Power BI Desktop\
-   JSON report definitions\
-   Star-schema modeling

------------------------------------------------------------------------

## .gitignore (recommended)

    # Power BI PBIP project
    *.abf
    *.pbi
    *.tmp
    *.cache
    .pbi/
    **/.pbi/
    **/*.lock.json
    **/Backup/
    **/Temp/

------------------------------------------------------------------------

## License

Released under the MIT License.\
You are free to use, modify, and distribute this project.

------------------------------------------------------------------------
