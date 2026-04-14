# Food Delivery Demand Analysis with Weather Data

DSA210 Term Project  

---

## Overview

This project analyzes how food delivery demand changes over time and how it is affected by weather conditions.

The main objective is to understand whether variables such as temperature, precipitation, hour of the day, and day of the week have a meaningful impact on order volume.

The project is structured in two main parts:
- Exploratory Data Analysis (EDA)
- Hypothesis Testing

---

## Motivation

Food delivery demand is not constant. It changes depending on:
- Time (hour of the day)
- Day type (weekday vs weekend)
- Environmental factors (weather conditions)

Understanding these patterns can help better interpret customer behavior and demand fluctuations.

---

## Data

### Order Dataset
- Source: Kaggle  
- Contains timestamps of food delivery orders  
- Used to calculate hourly order counts  

### Weather Dataset
- Source: Open-Meteo API  
- Includes:
  - Temperature (°C)
  - Precipitation  
- Collected at hourly level  

---

## Exploratory Data Analysis (EDA)

EDA was performed to understand patterns before applying statistical tests.

### Analyses Conducted:
- General overview (shape, missing values, summary statistics)  
- Time-based patterns:
  - Orders by hour  
  - Orders by day of the week  
- Weather relationships:
  - Temperature vs order count  
  - Precipitation vs order count  

### Observations:
- Order demand shows clear daily patterns  
- Demand varies across days of the week  
- Weather effects are less visually strong compared to time-based patterns  

---

## Hypothesis Testing

Statistical tests were conducted to evaluate the relationships observed in the EDA.

### Tests Applied:
- Pearson Correlation:
  - Temperature vs Orders  
  - Precipitation vs Orders  

- Welch’s T-Test:
  - Weekday vs Weekend demand  
  - Peak vs Non-peak hours  

---

## Key Findings

- Time-related variables (hour and day type) have a strong impact on demand  
- Temperature shows a weak or moderate relationship with order volume  
- Precipitation does not show strong statistical significance  
- Overall, demand is more influenced by time than weather conditions  

---

## Project Structure

- `EDA_Food_Order_Weather_Merged.ipynb` → Exploratory Data Analysis  
- `Hypothesis.ipynb` → Hypothesis Testing  
- `order_history_kaggle_data.csv` → Order dataset  
- `weather.xlsx` → Weather dataset  

---

## AI Usage

AI tools were used for:
- Code structuring and debugging  
- Improving clarity of explanations  

All analysis and interpretations were developed independently.
