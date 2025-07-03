# Palmora-Group Analysis
This project was done as a final project as part of my final assessment for the Data Analysis course for Data Skillup Africa by The Incubator Hub.
This is a documentation of a data analysis project. This explores the salary structure and gender-based pay disparities of Palmora Group using Power BI. The analysis uses a dataset simulating employee records across departments and regions. 

## Project Topic:Palmora Group HR Analysis

### Project Overview
The Palmora Group, a prominent manufacturing company in Nigeria, recently faced scrutiny for gender inequality across its regional operations. In response to a public backlash and internal concern, the company’s leadership launched an initiative to assess and address gender-related issues within its workforce.
This project involved analyzing the company's HR dataset using Power BI to uncover actionable insights focused on gender equality, pay equity, and regulatory compliance.

### Data Source
The primary data source used for this project is 

### Objectives
- Analyze HR data to identify gender-related discrepancies within the company.
- Allocate the annual bonus pay to employees based on the performance rating.
 
### Tools Used
- Ms Excel for preliminary data exploration, data collection and data cleaning.
- Power BI for data cleaning, data modelling and visualization.
- DAX (Data Analysis Expressions): Measures and calculated columns.

### Power BI Data Cleaning and Preparation
  - Reassigned non-disclosed gender entries as "Undisclosed"
  - Removed:
    -  Employees with missing salary data (no longer with the company).
    -  Entries with NULL department values.
  - Merged two tables "Palmora Group emp-data" and "bonus mapping"
  - Created a conditional column "Salary Range"
  - Created custom columns "Annual Bonus" and "Total Bonus Salary"
   
### Exploratory Data Analysis
This involved exloring of the data to analyze the following:
- Gender Distribution Analysis
   - Overall distribution of gender.
   - Breakdown by location and department.
- Performance Rating by Gender
- Salary Structure & Gender Pay Gap
  - Identify departments and locations with significant gaps.
- Evaluate adherence to the minimum salary requirement of $90,000.
  - Salary band analysis in $10,000 increments, visualized by region.
- Bonus Pay Allocation

### Data Analysis
This includes some basic lines on how I created the custom colums;
- Annual Bonus
``` =[Salary]*[Bonus Rate] ```
- Total Bonus Salary
```=[Salary]+[Annual Bonus] ```

### Power BI Dashboard
You can download the full `.pbix` file here: [https://github.com/Nissi-Olugbode/Palmora-Group-HR-Analysis/blob/main/Palmora%20Group%20project.pbix]

The analysis includes a interactive Power BI dashboard with the following visualizations;
- Gender distribution by location
- Ratings based on Gender
- Average salary based on gender
- Gender distribution by department
- Salary distribution ranges in all location
- Salary distribution range by gender
- Average bonus salary by location
- Employees with >$90,000 or <$90,000 salary

### Insights
- There is no significant gender paygap seen in the dataset.
- There is a gender paygap of $2.65k across all departments and regions with 465 male employee and 441 female employee.
- 654 employees (69% OF EMPLOYEES) fall below the required $90,000 minimum salary.


