# Excel Salary Dashboard

![DashboardGIF.gif](Resources/DashboardGIF.gif)

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

<img src="Resources/Dashboard4.jpg" alt="Salary Dashboard Chart1">

- 🛠️ **Excel Techniques:** Built a horizontal bar chart with tailored formatting to present salary figures more intuitively.
- 🎨 **Design Thinking::** Selected a horizontal layout to simplify the comparison between different job titles.
- 📉 **Data Organization:** Arranged job titles in order from the highest to the lowest salary to make key differences immediately visible.
- 🔍 **Key Observations:** Emphasizes that technical and leadership positions consistently lead the salary ranges, while analyst roles tend to fall lower on the scale.

#### 🗺️ Country Median Salaries - Map Chart

![Dashboard5.jpg](/Resources/Dashboard5.jpg)

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

![Dashboard2.jpg](Resources/Dashboard2.jpg) 

📉 Dashboard Implementation:

![Dashboard3.jpg](Resources/Dashboard3.jpg)

### ❎ Data Validation

#### 🔍 Filtered List

- 🔒 **Enhanced Data Validation:** A filtered list is applied as a validation rule for Job Title, Country, and Type selections, ensuring:
    - 🎯 User inputs are limited to approved and consistent values
    - 🚫 Invalid or inconsistent entries are automatically prevented
    - 👥 Dashboard usability remains streamlined and error-resistant
    - 🛡️ The worksheet is protected to safeguard validation rules and maintain the structural integrity of the dashboard.

## Conclusion

This dashboard provides a clear view of the demand for each data-related career path. Through the use of dynamic filters, users can instantly explore salary levels, job availability, and employment types across different countries and roles. It allows for quick comparisons between job titles, highlights regional salary variations, and helps identify the most promising opportunities within the field of data science. The interactive layout ensures a smooth user experience, making it easy to spot trends and make informed career decisions at a glance.
