# 💧 Water Consumption Analysis - Power BI Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Measures-4479A1?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

A Power BI portfolio project analysing household water survey activity patterns, recorded amounts, zones, and reported household characteristics.

---

## 📑 Table of Contents

- [Project Overview](#-project-overview)
- [Project Objectives](#-project-objectives)
- [Business Problem](#-business-problem)
- [Dashboard Preview](#-dashboard-preview)
- [Key Performance Indicators](#-key-performance-indicators-kpis)
- [Key Features](#-key-features)
- [Dashboard Pages](#-dashboard-pages--analysis)
- [Tools & Technologies](#-tools--technologies-used)
- [Dataset Information](#-dataset-information)
- [Data Cleaning & Transformation](#-data-cleaning--transformation)
- [Data Analysis & Insights](#-data-analysis--insights)
- [Business Insights & Findings](#-business-insights--findings)
- [Project Folder Structure](#-project-folder-structure)
- [How to Run This Project](#-how-to-run-this-project)
- [Installation & Usage](#-installation--usage-instructions)
- [Future Improvements](#-future-improvements)
- [Skills Demonstrated](#-skills-demonstrated)
- [Author Information](#-author-information)
- [Connect With Me](#-connect-with-me)

---

## 🎯 Project Overview

**Water Consumption Analysis** is an interactive Microsoft Power BI report built for exploring survey records related to household water use. The report compares water-use activities, zones, and reported household fields, with an emphasis on transparency around data validity and the meaning of the recorded values.

The project contains four report pages:

1. **Water Analysis Dashboard**
2. **Activity Distribution and Detailed Analysis**
3. **Household and Children Analysis**
4. **Overview**

> **Important:** The dashboard identifies `Recorded Amount` values, but the units and time basis are undocumented. These values must not be interpreted as litres or litres per day.

---

## 🎯 Project Objectives

- Explore survey records across water-use activities.
- Compare average recorded amounts between activities.
- Analyse recorded amounts across zones and reported household fields.
- Examine the relationship between the reported children field and recorded amounts.
- Distinguish survey records from valid activity records.
- Provide interactive filtering for activity and zone-level analysis.
- Present documented data limitations clearly within the report.

---

## 🧩 Business Problem

Water-use survey data can be difficult to interpret when activities, household characteristics, record validity, and measurement definitions are not presented consistently. This report addresses that problem by organising the available data into interactive views that allow users to:

- Compare activities through a common dashboard interface.
- Separate overall survey records from valid activity records.
- Explore zone and household patterns.
- Review distribution and detailed record-level behaviour.
- Avoid unsupported conclusions about consumption totals or measurement units.

---

## 📸 Dashboard Preview

> **Screenshot status:** No dashboard screenshots are currently available in this repository. The preview sections below are intentionally not populated with fake images.

To complete this section, open the report in **Power BI Desktop**, export one PNG for each relevant page, and place the files in the [`screenshots/`](screenshots/) folder.

| Suggested Screenshot | Recommended Filename |
|---|---|
| Water Analysis Dashboard | `screenshots/water-analysis-dashboard.png` |
| Activity Distribution and Detailed Analysis | `screenshots/activity-detail.png` |
| Household and Children Analysis | `screenshots/household-children.png` |
| Overview | `screenshots/overview.png` |

---

## 📊 Key Performance Indicators (KPIs)

The following KPIs and measures are explicitly used in the report:

| KPI / Measure | Purpose | Report Usage |
|---|---|---|
| **Survey Records** | Counts survey rows across all activities | KPI card, children distribution |
| **Valid Activity Records** | Counts valid records for the selected activity | KPI card, activity distribution |
| **Valid Records by Activity (All Activities)** | Counts valid records for each activity | Activity donut chart |
| **Average Recorded Amount** | Calculates the average of the recorded amount field | Zone/activity matrix and household comparison |
| **Average Recorded Amount by Activity (All Activities)** | Compares mean recorded amounts across activities | Bar chart and line chart |
| **Zone Count** | Displays the number of zones represented | Overview |

The project does not contain enough source metadata to publish numeric KPI values or calculate a water-consumption total.

---

## 🔑 Key Features

- Interactive activity slicers with a default **Cooking** selection.
- Zone-level filtering.
- Household and reported children-field analysis.
- Survey-record and valid-record KPI cards.
- Mean recorded amount comparisons.
- Recorded amount distribution using 50-unit bins.
- Zone-by-activity matrix.
- Scatter analysis by survey row, activity, reported children field, and recorded amount.
- Detailed record table for the selected activity.
- Explicit dashboard data caveats.

---

## 🗂️ Dashboard Pages / Analysis

| Page | Name | Confirmed Analysis |
|---|---|---|
| 1 | **Water Analysis Dashboard** | Activity comparison, household field comparison, children distribution, zone comparison, detailed records, and KPI cards |
| 2 | **Activity Distribution and Detailed Analysis** | Activity filtering, 50-unit recorded amount distribution, detailed records, and activity-average comparison |
| 3 | **Household and Children Analysis** | Household field comparison, reported children distribution, zone/activity matrix, and children vs. recorded amount scatter |
| 4 | **Overview** | Overall survey and valid-record KPIs, zone and activity counts, activity comparisons, and valid-record distribution |

### Common Report Slicers

- **Activity**
- **Zone**
- **Reported children field**
- **Reported household field**

---

## 🛠️ Tools & Technologies Used

| Technology | Usage |
|---|---|
| Microsoft Power BI | Report development and interactive visualisation |
| DAX | Report measures and calculated metrics |
| Power Query | Transformation details are not available in the extracted report definition |
| JSON report definition | Page, visual, slicer, and report metadata |

> Microsoft Excel, SQL, and external source datasets are not confirmed as part of this repository and have not been listed as project technologies.

---

## 📁 Dataset Information

No standalone `.csv`, `.xlsx`, `.xls`, `.json`, or source-query files are present in the repository folder. The data is embedded in the extracted Power BI model, represented here by the `DataModel` file.

Confirmed model fields and entities:

| Item | Confirmed Fields |
|---|---|
| `WaterUse` | Activity, zone, children, household, Recorded Amount, Recorded Amount Bin, Survey Row |
| `ActivityList` | Activity |

Additional dataset metadata such as source system, survey date, data owner, record count, region coverage, and unit definitions is not available.

---

## 🔄 Data Cleaning & Transformation

The report uses derived concepts such as:

- A **Recorded Amount Bin** field for distribution analysis.
- **Valid Activity Records** as a separate record count.
- Activity and zone dimensions for filtering and grouping.
- A reported **children** field and reported **household** field.

The original Power Query steps, source transformations, and DAX expressions are not included as separate, readable files in this extracted project format. Therefore, no specific cleaning steps or DAX formulas are claimed here.

---

## 🔍 Data Analysis & Insights

The report provides analysis through:

- Cross-activity comparisons of average recorded amounts.
- Cross-zone and cross-activity mean comparisons.
- Distribution of records across 50-unit recorded amount bins.
- Distribution of survey records by reported children field.
- Comparison of recorded amounts by reported household field.
- Scatter analysis between reported children field and recorded amount.
- Drillable detailed-record views.

Because source metadata and published numeric results are unavailable, this README does not state rankings, averages, or conclusions that could not be verified.

---

## 💡 Business Insights & Findings

No final business findings are claimed because the repository does not include an exported dashboard or source data that would allow independent verification of the visual results.

The report itself documents two important analytical constraints:

- Recorded amount units are undocumented.
- Recorded amounts may not be combined into a valid water-consumption total.

Potential findings should be described only after confirming units, time basis, valid-record rules, and source quality.

---

## 📂 Project Folder Structure

```text
Water_Consumption_Analysis.pbix/
├── README.md
├── .gitignore
├── [Content_Types].xml
├── DataModel
├── DiagramLayout
├── Metadata
├── SecurityBindings
├── Settings
├── Version
├── Report/
│   └── definition/
│       ├── report.json
│       ├── version.json
│       └── pages/
│           ├── pages.json
│           ├── Water_Analysis_Dashboard/
│           ├── Activity_Detail/
│           ├── Household_Children/
│           └── Overview/
└── screenshots/
    └── README.md
```

This is an extracted Fabric/Power BI report project structure. The source `.pbix` package is not present as a standalone file.

---

## ▶️ How to Run This Project

1. Download or clone this repository.
2. Open Microsoft **Power BI Desktop**.
3. Open a valid `.pbix` file if provided.
4. Select or refresh the report data source when prompted.
5. Use the activity, zone, household, and children slicers to explore the report.
6. Review the on-report caveats before interpreting recorded amounts.

> The current repository contains an extracted report definition and embedded model metadata, not a standalone `.pbix` file.

---

## ⚙️ Installation / Usage Instructions

### Requirements

- Microsoft Power BI Desktop
- Access to the original report data source, if refresh or edits are required
- A Power BI account for publishing or online sharing

### Usage

- Navigate between the four report pages.
- Use **Activity** to apply a single-activity comparison filter.
- Use **Zone** to review zone-specific patterns.
- Use **Household** or **Children** filters where available.
- Hover over visuals for tooltips and underlying values.
- Keep units and time basis in mind before presenting findings.

---

## 🚀 Future Improvements

- Add dashboard screenshots for all four report pages.
- Restore or document the standalone `.pbix` file.
- Add the original dataset or a clearly documented, privacy-safe sample.
- Document data sources and refresh frequency.
- Define the units and time basis for `Recorded Amount`.
- Define valid-record and invalid-record rules.
- Add data quality and missing-value metrics.
- Publish verified business findings and KPI targets.
- Add year, date, or period fields if available.
- Add a data dictionary and transformation documentation.

---

## 🧠 Skills Demonstrated

- Power BI report development
- Interactive dashboard design
- Data model field selection
- DAX measure usage
- Slicer and filter design
- Water-use survey analysis
- Chart selection and visual storytelling
- Data limitation and caveat communication
- Report metadata and documentation review

---

## 👨‍💻 Author Information

**Rahul Sharma**

- **Role:** CSE (Data Science) Student | Aspiring Data Analyst
- **Relevant Skills:** Power BI, Data Analysis
- **GitHub:** [@Rahulsharma2006](https://github.com/Rahulsharma2006)

---

## 🤝 Connect With Me

[![GitHub](https://img.shields.io/badge/GitHub-Rahulsharma2006-181717?style=for-the-badge&logo=github)](https://github.com/Rahulsharma2006)

If you review this project or have suggestions for improving the analysis, feel free to connect with me on GitHub.
