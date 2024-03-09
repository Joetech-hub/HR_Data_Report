# HR_Data_Report
This report analyzes the HR data of a company, to discover trends and insights relating to the job environment.

**Documentation Outline**
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools Used](#tools-used)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Data Analysis](#data-analysis)
- [Results and Findings](#results-and-findings)

##Project Overview
This project uncovers insights from workers attributes as recorded by the human resource department

## Data Sources
---
The primary source of data is HR Data.xlsx and is sourced from the Human resource Department

## Tools used
---
powerbi (for querying, analysis and reporting)

## Data Cleaning and preparation
---
- Used first rows as headers
- Change data type of some columns
- added a conditional column from the Attrition column named 'Attrition Count'
- Changed the datatype of Attrition Count from text to whole number
  
## Data Analysis
---
  ```
  pbix
  # Total number of current employees (Retained employees):
  Retained Employee = SUM('HR data'[Employee Count]) - SUM('HR data'[Attrition Count])
  # To calculate attrition rate or the rate workers are leaving the company:
  Attrition Rate = SUM('HR data'[Attrition Count]) / SUM('HR data'[Employee Count])
  ```
