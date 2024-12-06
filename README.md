# Data Analysis of Kansas City Crime Data

In this notebook, I will focus on geospatial techniques using crime data from Kansas City, MO. While the dataset offers extensive opportunities for analysis, this notebook will remain concise, providing a snapshot of key insights. The primary goal is to demonstrate proficiency with tools such as Folium, Plotly, Pandas, and NumPy.

[View the Interactive HTML in Github](kansas-city-crime-geospatial-analysis.html)

or

[View in NBViewer](https://nbviewer.org/github/AnalyzerArik/Kansas-City-Missouri-2024-Crime-Data-Analysis-/blob/main/kansas-city-crime-geospatial-analysis.html)


## **About the Data: Kansas City Police Department (KCPD) Crime Data**

This dataset contains detailed information about reported crimes in Kansas City, Missouri, for the year 2024. It is designed to support geospatial, temporal, and categorical analyses of crime patterns. You may notice that the data markers center on the right side of Kansas City with a clear distinction. This is because Kansas City sits on the border of Kansas and Missouri and there is a separate Police Department for Kansas City, Kansas. This data is only the Missouri statistics. The data includes information on the type of crimes, their locations, involved individuals, and temporal details. This is real-world data that is updated on a weekly basis, available at https://data.kcmo.org/Crime/KCPD-Crime-Data-2024/isbe-v4d8/about_data.

## Data Overview
- **Dataset:** Kansas City Police Department (KCPD) Crime Data  
- **Rows:** 95932  
- **Columns:** 24 (e.g., Report_No, Offense, Address, Description, Firearm Used Flag)  
- **Source:** [KCPD Open Data Portal](https://data.kcmo.org/Crime/KCPD-Crime-Data-2024/isbe-v4d8/about_data).

## Methodology
- 1. Data preprocessing and cleaning to handle null values and format datetime fields.
- 2. Exploratory Data Analysis (EDA) focusing on categorical, and geospatial trends.
- 3. Geospatial visualization of crime hotspots using Folium maps.
- 4. Categorization and summary of crime types with statistical insights.

## Key Findings
- Crime rates exhibit distinct peaks during evening hours and weekends.
- Certain patrol districts and neighborhoods have significantly higher crime concentrations.
- Domestic violence incidents often cluster within specific geographic areas.
- Firearm-related crimes constitute a notable percentage of violent offenses.

## Tools and Libraries Used
- Python Libraries: Pandas, NumPy, Matplotlib, Seaborn, Folium, Plotly.
- Tools: Jupyter Notebook.
