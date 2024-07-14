# HR Analytics Power BI Project

This repository contains a Power BI project that analyzes three months of employee  real attendance data of a company AtliQ. The project involves data transformation in Power Query, creation of parameters and functions, and building an interactive dashboard. 

## Table of Contents

- [Project Overview](#project-overview)
- [Data Preparation](#data-preparation)
  - [Loading Data](#loading-data)
  - [Data Transformation](#data-transformation)
  - [Creating Parameters and Functions](#creating-parameters-and-functions)
  - [Invoking Functions](#invoking-functions)
- [Building the Dashboard](#building-the-dashboard)
  - [Key Metrics](#key-metrics)
  - [Visualizations](#visualizations)
- [Screenshots](#screenshots)
- [Conclusion](#conclusion)

## Project Overview

The goal of this project is to create an HR Analytics dashboard that provides insights into employee attendance over a three-month period. The dashboard includes key metrics such as Present Rate, Work From Home (WFH) Rate, and the distribution of attendance statuses.

## Data Preparation

### Loading Data

1. **Import Data**: Import the three months of employee attendance data from an Excel workbook into Power Query.

### Data Transformation

2. **Transform Data**: Perform necessary data transformations on the template to clean and structure the data. This includes:
   - Each date were having different columns, Converterted data from report format to unpivoted format
   - Removing unnecessary columns that were showing summary
   - Renaming columns for consistency 
   - Promoting headers
   - Converting data types
   - Handling missing values
   - Creating calculated columns

### Creating Parameters and Functions

3. **Create Parameter**: Create a parameter to dynamically handle different data inputs.
   - Go to the "Home" tab and select "Manage Parameters" -> "New Parameter".
   - Name the parameter (p1) , and set the data type and allowed values.

4. **Create Function**: Create a function from the template that uses the parameter.
   - Go to the "Home" tab and select "Advanced Editor".
   - Write a function that takes the parameter as input and applies the necessary transformations.

### Invoking Functions

5. **Invoke Function**: Use the created function to process each month's data.
   - Add a custom column in the workbook.
   - Invoke the function with the parameter for each row in the custom column.

## Building the Dashboard

### Key Metrics

6. **Calculate Key Metrics**: Calculate important metrics such as:
   - Total Employees in the organisation
   - Present Rate of employees
   - WFH Rate of employees
   - Total Working Days of the office
   - Total Days Off of the office

### Visualizations

7. **Create Visuals**: Build the following visuals to display the data:
   - Line chart showing total Employees Present in the Office over time
   - Pie chart showing Employees Attendance Status Distribution
   - Tables showing wfh rate and presence raate by day
   - Table showing full form of each attendance status
   - Line chart showing Sick Leave trends
   - Card Visuals showing some import key  matrices
   - Month filter allowing us to see these these insights of a particular month.

## Screenshots


![Screenshot 2024-07-14 113529](https://github.com/user-attachments/assets/aaead78f-8d6d-4069-9c65-2e521a5ef03c)

*Figure 1: HR Analytics Dashboard*

![Screenshot 2024-07-14 114011](https://github.com/user-attachments/assets/35eac9b4-9208-4897-8e9b-6d66d7aa3d45)

*Figure 2: Data Model*

### Key Visuals Description

- **Line Chart (Employees Presence in the 
ffice)**: Displays the number of employees present in the office over the three-month period.
- **Pie Chart (Attendance Status Distribution)**: Shows the distribution of various attendance statuses (Present, WFH, Leave, etc.).
- **Tables (Daily Rates)**: Show the daily present rate and WFH rate for each day of the week.
- **Line Chart (Sick Leave)**: Tracks the trend of sick leave taken by employees.

## Conclusion

This HR Analytics Power BI dashboard provides a comprehensive view of employee attendance over three months. By following the steps outlined in this README, you can replicate the process and create similar dashboards for other datasets.

For any questions or further assistance, feel free to open an issue in this repository.
