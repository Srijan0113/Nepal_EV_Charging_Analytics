# Nepal EV Charging Stations — Data Quality Audit

An exploratory data audit investigating the availability, completeness, and reliability of electric vehicle (EV) charging station data in Nepal.

## 1. Project Overview

The original objective of this project was to analyze the status and geographical coverage of EV charging stations across Nepal.

To investigate this, approximately **350 EV charging station records** were collected from publicly available sources. The collected data was reviewed and cleaned as part of an initial data preparation process.

However, the audit revealed significant limitations in data completeness, geographical accuracy, and consistency across sources.

Rather than produce potentially misleading conclusions from incomplete information, the original nationwide infrastructure analysis was discontinued.

The project was retained as a data quality audit to document these challenges and highlight the need for more reliable EV infrastructure data in Nepal.

## 2. Key Findings

### 2.1 No Consistent National Station Count

Different sources reported substantially different numbers of EV charging stations in Nepal.

| Source | Reported Number |
|---|---:|
| nepalevs.com | 352+ stations |
| Nepal Electricity Authority (NEA) | 62 fast chargers |
| Ministry report | Approximately 1,000 stations |
| Media reports citing NEA | 2,300+ stations |

These figures may represent different reporting periods, definitions, and types of charging infrastructure. Therefore, they should not be treated as directly comparable.

The findings highlighted the lack of a readily accessible, comprehensive national station-level registry.

### 2.2 Significant Data Incompleteness

The collected dataset contained substantial missing information.

| Data Quality Issue | Percentage / Count |
|---|---:|
| Missing power specifications | 57% |
| Missing geographical coordinates | 60% |
| Records with sufficient information for the intended analysis | Approximately 150 (43%) |

The missing information restricted the ability to perform reliable geographical coverage and charging-capacity analysis.

### 2.3 Data Inconsistencies and Errors

Several data-quality issues were identified during the audit:

- Approximately 10 duplicate listings.
- Incorrect or repeated geographical coordinates.
- Different station records associated with identical coordinates despite representing locations in different districts.
- Older collected data containing incomplete records and mismatched location information.

These inconsistencies raised concerns about the accuracy and reliability of the available station listings.

### 2.4 Limited Station-Level Information

Many charging stations appeared to be associated with private businesses, including vehicle dealerships and hotels.

However, detailed station-level information was not consistently available.

This made it difficult to independently verify station ownership, operational status, charging capacity, and geographical location.

## 3. Why the Original Analysis Was Discontinued

Although approximately 350 records were collected, only around 150 contained sufficient information for the intended analysis.

This limited the ability to draw reliable conclusions about Nepal's nationwide EV charging infrastructure.

Several factors contributed to the decision:

- A significant proportion of records lacked essential information.
- Geographical coordinates were missing or potentially inaccurate.
- Different sources reported conflicting station counts.
- Independent verification of station-level information was difficult.
- Additional scraping and field verification would have required considerably more time and resources.

Filling missing values through assumptions or using unverified geographical information could have introduced further inaccuracies.

For these reasons, the original nationwide infrastructure analysis was discontinued.

## 4. Recommendations for Future Research

A more comprehensive assessment of Nepal's EV charging infrastructure would benefit from the following improvements:

1. **Official National Database:** Establish a centralized and regularly updated registry of EV charging stations.
2. **Private Operator Data Sharing:** Encourage charging network operators and private businesses to publish standardized station-level information.
3. **Geographical Verification:** Include accurate coordinates, administrative locations, and independent location verification.
4. **Standardized Reporting:** Maintain consistent definitions for charging stations, fast chargers, charging points, and operational infrastructure.
5. **Regular Data Updates:** Introduce a process for tracking newly installed, operational, and discontinued charging stations.

## 5. Project Outcome

The project was concluded as a **Data Quality Audit** rather than a nationwide EV charging infrastructure analysis.

Although the original research objective could not be completed, the audit highlighted important challenges associated with collecting, validating, and analyzing real-world infrastructure data.

**Key takeaway:** Reliable analysis starts with reliable data. When available information cannot adequately support a research question, recognizing its limitations is more responsible than producing unsupported conclusions.

## 6. Tools and Technologies

The project involved the following tools and concepts:

- Python
- Pandas
- CSV Data Handling
- Data Cleaning
- Data Quality Assessment
- Exploratory Data Analysis (EDA)
- Web Data Collection

## 7. Repository Structure

```text
Nepal-EV-Charging-Data-Audit/
│
├── data/
│   └── raw/
│       └── [Original CSV datasets]
├── notebooks/
│   └── requirements.txt
├── venv
│ 
├──.gitignore
└── README.md
```

**Repository note:** This repository currently contains the original collected CSV files and this documentation. The original analysis notebooks and data-cleaning scripts are not included. The findings documented here reflect the earlier audit and are not independently reproducible from the repository contents alone.

## 8. Project Status

**Status: Completed — Data Quality Audit**

The original nationwide infrastructure analysis was discontinued due to limitations in data availability, completeness, and reliability.

The project remains documented as an assessment of the challenges involved in obtaining dependable EV charging infrastructure data for Nepal.