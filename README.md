# IBM HR Attrition Analysis

This repository contains a Jupyter Notebook and a cleaned version of the IBM HR dataset, which is a fictional dataset created by IBM data scientists. The goal is to analyze the factors that contribute to employee attrition and prepare the data for visualization in Tableau.

## Description of the Project

The purpose of this project is to understand what variables influence employee attrition and to prepare a clean, structured dataset suitable for data storytelling and dashboard creation. The analysis is focused on cleaning, selecting relevant features, and renaming variables to ensure clarity when visualizing the data.

## Repository Contents

- HR_IBM.ipynb: Jupyter Notebook containing the analysis and data cleaning steps.
- HR_cleaned_for_tableau.csv: Final cleaned dataset ready for import into Tableau.
- README.md: This documentation file.

## Steps Performed

1. Inspected the structure and data types of the dataset.
2. Verified the presence of missing values and found none.
3. Dropped the following non-informative or redundant columns:
   - EmployeeNumber: only an ID.
   - StandardHours, EmployeeCount, Over18: contain constant values.
   - DailyRate, HourlyRate, MonthlyRate: less relevant due to redundancy with MonthlyIncome.
4. Renamed several variables for clarity and better integration with Tableau.
5. Exported the final version of the dataset in CSV format for use in Tableau.

## Dataset Information

The dataset includes demographic, satisfaction, performance, and compensation information for employees. Key variables include:
- Attrition (whether the employee left the company)
- MonthlyIncome
- JobRole
- WorkLifeBalance
- EnvironmentSatisfaction
- Education
- PerformanceRating

All numeric categorical variables have been kept in numeric form but are interpreted using a predefined scale (e.g. 1 = Low, 4 = Very High).

## Next Steps

The cleaned dataset is ready to be loaded into Tableau to build visualizations that explore questions such as:
- Which roles or departments have the highest attrition?
- Is there a link between monthly income and attrition?
- Does work-life balance influence an employee's decision to leave?

## Accessibility

This repository does not require any API authentication. All necessary files are included and can be downloaded directly from GitHub.
