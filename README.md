# zomato-dashboard-power-bi
![Zomato Dashboard Power BI](https://raw.githubusercontent.com/Mothilragav05/Mothilragav05-zomato-dashboard-power-bi/c2770fa65a0fc1e3f3b3d1204b1500b62188532b/Dashboard-image.png)

## Table of Content
• [Introduction](#introduction)  
• [Dashboard Requirements](#dashboard-requirements)  
• [Installation / Usage](#installation--usage)  
• [DAX Formulas Used in Measures](#dax-formulas-used-in-measures)  
• [Bug / Feature Request](#bug--feature-request)  
• [Authors](#authors)  

## Introduction
• This project focuses on developing a Power BI Dashboard to analyze and generate insights from the Zomato restaurant dataset.

• The dataset is available at the following link: [Zomato Dataset](https://www.kaggle.com/datasets/rajeshrampure/zomato-dataset).

## Dashboard Requirements
📊 Primary KPIs Section (Top Row Cards)
Total Restaurants → Show total number of restaurants listed in the dataset.

Total Aggregate Rating → Sum or average of all ratings across restaurants (e.g., 5.19K).

Count of City → Number of unique cities where restaurants are available.

📈 Average Cost Gauge (Middle Center)
Count of Average Cost for Two → Use a half-donut gauge to display the average cost for two people, comparing actual value vs. maximum in dataset (e.g., 1408 out of 2816).

📌 Filters (Left Section)
Price Range → Checkbox filter (1 to 4) for restaurant pricing categories.

Has Table Booking → Checkbox to filter restaurants by whether they offer table booking.

Has Online Delivery → Checkbox filter for availability of online delivery.

📋 Top Restaurants Table (Middle Bottom)
Restaurant Name vs Aggregate Rating Table → A sortable table displaying restaurants and their ratings (like "#Dilliwaala6", 3.7 rating).

Enables users to view and rank restaurants based on popularity and rating.

📍 City-Based Analysis (Right Center)
Count of Restaurant Name by City → Horizontal bar chart showing number of restaurants in each city (e.g., New Delhi, Gurgaon, etc.).

Highlights which cities dominate the restaurant listings.

🌐 Country-Based Distribution (Bottom Right Donut Chart)
Count of Restaurant Name by Country → Donut chart displaying distribution of restaurants by country (India leading with 1.11K out of 1.19K).

📉 Restaurant Frequency by Name (Top Right Chart)
Count of Restaurant ID by Restaurant Name → Bar chart to show how frequently a restaurant appears (good for franchises or chain analysis).

🔄 Country Dropdown Filter (Top Right Corner)
Enables the user to filter entire report based on selected country.

## Installation / Usage
•Install Power BI Desktop from the [Official Power BI Download Site](https://www.microsoft.com/en-us/download/details.aspx?id=58494).

•Download data files from link given in Introduction

•Download this repository to your local machine

•Open Dashboard report file (Road Accidents Dashboard.pbix) in Power BI Desktop, to access the dashboard's interactivity

## DAX Formulas Used in Measures
1.Total Restaurants
  •Total Restaurants = DISTINCTCOUNT('zomato'[Restaurant Name])

2.Total Aggregate Rating
  •Total Aggregate Rating = SUMX('zomato', VALUE('zomato'[Aggregate Rating]))
  
3.Total Countries 
  •Total Countries = DISTINCTCOUNT('zomato'[Country Code])

## Bug / Feature Request   
- If you encounter any bugs (e.g., the dashboard produces undesired results), please open an issue [here](https://github.com/Mothilragav05/Mothilragav05-zomato-dashboard-power-bi/issues) and include:
  - Your search query
  - The expected result

- If you'd like to request a new feature, feel free to open an issue [here](https://github.com/Mothilragav05/Mothilragav05-zomato-dashboard-power-bi/issues). Please include:
  - Sample queries
  - The corresponding expected results
## Authors
[Mothilragav](https://github.com/Mothilragav05)
