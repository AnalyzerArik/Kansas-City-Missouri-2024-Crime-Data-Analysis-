# Data Analysis of Kansas City Crime Data

---

## **Table of Contents**
1. [Introduction](#introduction)  
2. [Dataset Description](#dataset-description)  
3. [Project Objectives](#project-objectives)  
4. [Methodology](#methodology)  
5. [Key Findings](#key-findings)  
6. [Tools and Libraries Used](#tools-and-libraries-used)  
7. [Future Work](#future-work)  
8. [Acknowledgments](#acknowledgments)  

---

## **Introduction**
This project focuses on geospatial analysis of crime data from Kansas City, Missouri, for the year 2024. Using tools such as Folium, Plotly, Pandas, and NumPy, this analysis explores crime patterns and trends to provide actionable insights. While the dataset offers extensive opportunities for analysis, this project remains concise, showcasing key insights and demonstrating proficiency with geospatial techniques.

[View the Interactive HTML in Github](kansas-city-crime-geospatial-analysis.html)  
or  
[View in NBViewer](https://nbviewer.org/github/AnalyzerArik/Kansas-City-Missouri-2024-Crime-Data-Analysis-/blob/main/kansas-city-crime-geospatial-analysis.html)

---

## **Dataset Description**
- **Source**: [KCPD Open Data Portal](https://data.kcmo.org/Crime/KCPD-Crime-Data-2024/isbe-v4d8/about_data)  
- **Rows**: 95,932  
- **Columns**: 24  
  - Example columns: `Report_No`, `Offense`, `Address`, `Description`, `Firearm Used Flag`.  
- **Notes**:  
  - The data is specific to Kansas City, Missouri, excluding statistics from Kansas City, Kansas, which has a separate police department.  
  - Updated weekly with real-world crime data.  

---

## **Project Objectives**
- Identify geospatial and trending crime patterns.  
- Highlight hotspots and high-crime areas using geospatial visualization techniques.  
- Provide actionable insights into crime trends and contributing factors.  
- Demonstrate advanced proficiency with geospatial tools and techniques.  

---

## **Methodology**
1. **Data Preprocessing**:  
   - Handled null values and cleaned the dataset.  
   - Reformatted datetime fields for temporal analysis.  

2. **Exploratory Data Analysis (EDA)**:  
   - Analyzed categorical data to identify trends in offense types.  
   - Investigated geospatial trends by patrol district and neighborhood.  

3. **Geospatial Visualization**:  
   - Created interactive Folium maps to visualize crime hotspots and patterns.  
   - Used Plotly for detailed temporal and geospatial analysis.  

4. **Categorization and Summary**:  
   - Summarized crime types and patterns using statistical insights.  

---

## **Key Findings**
1. **Geospatial Concentrations**:  
   - Certain patrol districts and neighborhoods show significantly higher crime densities.  

2. **Domestic Violence**:  
   - Domestic violence incidents cluster within specific geographic areas.  

3. **Firearm-Related Crimes**:  
   - A notable percentage of violent crimes involve firearms.  

---

## **Tools and Libraries Used**
- **Programming Language**: Python  
- **Libraries**:  
  - `pandas` for data manipulation  
  - `numpy` for numerical analysis  
  - `matplotlib` and `seaborn` for visualizations  
  - `folium` for geospatial mapping  
  - `plotly` for interactive visualizations  
- **Tools**: Jupyter Notebook  

---

## **Future Work**
- Expand the analysis to include multi-year data for a longitudinal study of crime trends.  
- Incorporate machine learning models to predict crime hotspots based on historical patterns.  
- Conduct deeper analysis of specific crime categories, such as property crimes or violent offenses.  

---

## **Acknowledgments**
Special thanks to the Kansas City Police Department for providing access to open data and to the data analysis community for their continuous support and inspiration.

---

