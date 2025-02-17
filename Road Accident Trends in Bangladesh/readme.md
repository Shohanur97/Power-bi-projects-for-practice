
# Road Accident Analysis in Bangladesh (1980-2024)
![image alt](https://github.com/Shohanur97/Power-bi-projects-for-practice/blob/main/Road%20Accident%20Trends%20in%20Bangladesh/Road%20Accident%20Trends%20in%20Bangladesh.png)

## 📌 Overview
This project provides a comprehensive analysis of road accidents in Bangladesh from **1980 to 2024**. By analyzing accident trends, fatalities, and injury patterns, we aim to uncover key insights into road safety. The dataset includes details such as accident counts, fatalities, serious injuries, and other related factors.

## 📊 Key Objectives
- Identify trends in road accidents over the years.
- Make a table & pie Chart
- Analyze the fatality rate and injury severity.
- Develop a **Moving Average Chart** using DAX in Power BI to observe long-term trends.
- Provide actionable insights into road safety improvements.

## 🛠 Data Preprocessing
To ensure clean and reliable data, we performed:
- **Handling Missing Values**: Filled or removed missing records.
- **Duplicate Removal**: Eliminated duplicate entries.
- **Data Type Conversion**: Ensured consistency across numerical and date fields.

## 🔍 Exploratory Data Analysis
- **Descriptive Statistics**: Summary metrics for accidents, fatalities, and injuries.
- **Dataset Shape Analysis**: Understanding dataset structure and distributions.

## 📈 Power BI Analysis & DAX Measures
We utilized **Power BI** for visualization and implemented **DAX** formulas to extract insights:

1. **Total Accidents in a Year**  
```DAX
AccidentsInYear =  
CALCULATE(
    SUM(road_accident[Number of Accidents]),
    road_accident[Year] = SELECTEDVALUE(road_accident[Year])
)


