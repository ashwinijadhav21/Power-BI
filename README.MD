# HR Analytics Dashboard | Power BI

An interactive HR analytics dashboard developed using Microsoft Power BI to analyze employee demographics, workforce distribution, and employee attrition.

## Project Overview

This project transforms raw HR data into an interactive dashboard that enables analysis of employee attrition across departments, job roles, age groups, gender, and locations.

The objective is to identify workforce patterns and provide insights that can support data-driven HR decision-making.

## Business Objectives

- Analyze overall employee attrition.
- Identify departments and job roles with higher attrition.
- Examine attrition patterns across demographic groups.
- Monitor key workforce metrics.
- Enable interactive exploration of HR data.

## Technology Stack

| Tool | Purpose |
|---|---|
| Power BI | Dashboard development |
| Power Query | Data cleaning and transformation |
| DAX | Measures and calculated columns |
| CSV | Data source |

## Dataset

- **Records:** 988 employee records
- **Domain:** Human Resources
- **Data includes:** Employee demographics, department, job role, salary, tenure, satisfaction ratings, hiring dates, exit dates, and attrition status.

## Data Preparation

Data preparation was performed using Power Query.

Key operations:
- Inspected data quality, missing values, and errors.
- Handled missing and invalid values.
- Replaced data errors with null values where appropriate.
- Created cleaned columns for selected numerical fields.
- Standardized data types.
- Preserved missing attrition values rather than assigning assumed outcomes.

## Dashboard Components

### Key Performance Indicators
- Total Employees
- Active Employees
- Attrition Count
- Attrition Rate
- Average Salary
- Average Age
- Average Tenure

### Analytical Visualizations
- Attrition by Department
- Attrition by Gender
- Attrition by Age Group
- Attrition by Job Role

### Interactive Filters
- Department
- Gender
- Location
- Age Group

## DAX Implementation

DAX was used to create measures and calculated columns for workforce analysis.

Example:

**Total Employees**
```dax
Total Employees =
DISTINCTCOUNT(Raw_HR_Data[Employee_ID])
```

**Attrition Count**
```dax
Attrition Count =
CALCULATE(
    COUNTROWS(Raw_HR_Data),
    Raw_HR_Data[Attrition] = "Yes"
)
```

**Attrition Rate**
```dax
Attrition Rate =
DIVIDE(
    [Attrition Count],
    CALCULATE(
        [Total Employees],
        NOT(ISBLANK(Raw_HR_Data[Attrition]))
    ),
    0
)
```

## Skills Demonstrated

- Data Cleaning and Transformation
- Exploratory Data Analysis
- Data Modeling and DAX
- KPI Development
- Data Visualization
- Dashboard Design
- Business Data Interpretation

## Project Deliverables

- Power BI interactive dashboard (`.pbix`)
- Cleaned and transformed HR dataset
- DAX measures and calculated columns

## Author

**Ashwini Jadhav**

[GitHub Profile](https://github.com/ashwinijadhav21)
