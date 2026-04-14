# Food Delivery Demand Analysis with Weather Data

DSA210 Term Project  

---

## Overview

This project analyzes how food delivery demand changes over time and how it is influenced by weather conditions.

The main objective is to examine whether variables such as temperature, precipitation, hour of the day, and day of the week have a measurable impact on order volume.

The project is structured in two main parts:
- Exploratory Data Analysis (EDA)
- Hypothesis Testing

---

## Motivation

Food delivery demand is not constant and varies depending on several factors.

In particular, demand is expected to change based on:
- Time of the day  
- Day type (weekday vs weekend)  
- Environmental conditions such as weather  

Understanding these patterns helps provide insights into customer behavior and demand fluctuations.

---

## Data

### Order Dataset
- Source: Kaggle  
- Contains approximately 21,000 records :contentReference[oaicite:0]{index=0}  
- Includes order timestamps and related features  
- Used to calculate hourly order counts  

### Weather Dataset
- Source: Open-Meteo API  
- Includes:
  - Temperature (°C)
  - Precipitation  
- Collected at hourly level and aligned with order timestamps  

---

## Methodology

### Data Preparation
- Converted timestamps into datetime format  
- Rounded both datasets to hourly level  
- Aggregated order data into hourly order counts  
- Merged datasets based on the datetime column  

---

## Exploratory Data Analysis (EDA)

EDA was conducted to explore patterns before applying statistical methods.

### Analyses Conducted:
- General overview (dataset size, missing values, summary statistics)  
- Time-based patterns:
  - Orders by hour  
  - Orders by day of the week  
- Weather relationships:
  - Temperature vs order count  
  - Precipitation vs order count  

### Observations:
- Order demand shows clear daily patterns  
- Demand varies across days of the week  
- Weather effects are less visually prominent compared to time-based patterns  

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
- Overall, demand appears to be more influenced by time than weather conditions  

---

## Project Structure

- `EDA_Food_Order_Weather_Merged.ipynb` → Exploratory Data Analysis  
- `Hypothesis.ipynb` → Hypothesis Testing  
- `order_history_kaggle_data.csv` → Order dataset  
- `weather.xlsx` → Weather dataset  

---

## AI Usage

AI tools were used for:
- Structuring and debugging code  
- Improving clarity of explanations  

All analysis steps, decisions, and interpretations were carried out independently.
