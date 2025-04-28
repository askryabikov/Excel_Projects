# Excel Salary Dashboard

![1_Salary_Dashboard.png](/0_Resources/Images/1_Salary_Dashboard_Final_Dashboard.gif)

## Introduction

This data jobs salary dashboard was created to help job seekers investigate salaries for their desired jobs and ensure they are being adequately compensated. 

The data contains detailed information on job titles, salaries, locations, and essential skills that are presented here.

### Dashboard File
My final dashboard is in [LB_Salary_calculator_project1.xlsx](LB_Salary_calculator_project1.xlsx).

### Excel Skills Used

The following Excel skills were utilized for analysis:

- **📉 Charts**
- **🧮 Formulas and Functions**
- **❎ Data Validation**

### Data Jobs Dataset

The dataset used for this project contains real-world data science job information from 2023. It includes detailed information on:

- **👨‍💼 Job titles**
- **💰 Salaries**
- **📍 Locations**
- **🛠️ Skills**

## Dashboard Build

### 📉 Charts

#### 📊 Data Science Job Salaries - Bar Chart

<img src="/0_Resources/Images/1_Salary_Dashboard_Chart1.png" width="850" height="550" alt="Salary Dashboard Chart1">

- 🛠️ **Excel Techniques:** Built a horizontal bar chart with tailored formatting to present salary figures more intuitively.
- 🎨 **Design Thinking::** Selected a horizontal layout to simplify the comparison between different job titles.
- 📉 **Data Organization:** Arranged job titles in order from the highest to the lowest salary to make key differences immediately visible.
- 🔍 **Key Observations:** Emphasizes that technical and leadership positions consistently lead the salary ranges, while analyst roles tend to fall lower on the scale.

#### 🗺️ Country Median Salaries - Map Chart

![1_Salary_Dashboard_Chart2.png](/0_Resources/Images/1_Salary_Dashboard_Country_Map.gif)

- 🛠️ **Excel Techniques:** Applied Excel’s map chart to translate country-based salary data into a visual format.
- 🎨 **Design Thinking::** Used color intensity to instantly reflect variations in median salaries across different countries.
- 🗺️ **Data Mapping:** Each country with available data is shaded based on its median salary, making regional differences easy to spot.
- 🔍 **Key Observations:** Clearly illustrates how salary levels vary globally, highlighting top-paying regions and bringing attention to salary gaps between countries.

### 🧮 Formulas and Functions

#### 🧩 Unique Job Schedule Extraction — Filter Formula

```
=FILTER(J2#,(NOT(ISNUMBER(SEARCH("and",J2#))+ISNUMBER(SEARCH(",",J2#))))*(J2#<>0))
```

- 🛠️ **Excel Techniques::** Combined FILTER() with SEARCH() and logical conditions to dynamically clean the job schedule list.
- 🧠 **Logic Behind:** Excludes any job schedule entries containing "and" or commas, which indicate multiple schedule types, and removes blank or zero entries.
- 🧹 **Data Preparation:** Ensures only clean, single-schedule types are passed forward for further use, improving the consistency of dashboard filters.
- 🔍 **Key Observations:** Helps streamline dropdown menus and slicers by presenting a validated, unambiguous list of schedule types.

🍽️ Background Table

![1_Salary_Dashboard_Screenshot1.png](/0_Resources/Images/1_Salary_Dashboard_Screenshot1.png)   - Dashboard 2

#### ⏰ Count of Job Schedule Type

```
=FILTER(J2#,(NOT(ISNUMBER(SEARCH("and",J2#))+ISNUMBER(SEARCH(",",J2#))))*(J2#<>0))
```

- 🔍 **Unique List Generation:** This Excel formula below employs the `FILTER()` function to exclude entries containing "and" or commas, and omit zero values.
- 🔢 **Formula Purpose:** This formula populates the table below, which gives us a list of unique job schedule types.

🍽️ Background Table

![1_Salary_Dashboard_Type.png](/0_Resources/Images/1_Salary_Dashboard_Screenshot2.png)    - Dashboard 3

📉 Dashboard Implementation:

<img src="/0_Resources/Images/1_Salary_Dashboard_Type.png" width="350" height="500" alt="Salary Dashboard Type">

### ❎ Data Validation

#### 🔍 Filtered List

- 🔒 **Enhanced Data Validation:** Implementing the filtered list as a data validation rule under the `Job Title`, `Country`, and `Type` option in the Data tab ensures:
    - 🎯 User input is restricted to predefined, validated schedule types
    - 🚫 Incorrect or inconsistent entries are prevented
    - 👥 Overall usability of the dashboard is enhanced

<img src="/0_Resources/Images/1_Salary_Dashboard_Data_Validation.gif" width="425" height="400" alt="Salary Dashboard Data Validation">

## Conclusion

This dashboard provides a clear view of the demand for each data-related career path. Through the use of dynamic filters, users can instantly explore salary levels, job availability, and employment types across different countries and roles. It allows for quick comparisons between job titles, highlights regional salary variations, and helps identify the most promising opportunities within the field of data science. The interactive layout ensures a smooth user experience, making it easy to spot trends and make informed career decisions at a glance.
