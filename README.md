---
title: "README - Feeding America: Food Insecurity Dashboard"
output:
  html_document:
    df_print: paged
---

# Food Insecurity Dashboard  
  
## Overview and Importance
This interactive **Food Insecurity Dashboard** visualizes key trends in food insecurity across the United States, with a focus on **Georgia counties** and the **top 10 most food-insecure states**. It utilizes **Feeding America’s Map the Meal Gap dataset** to provide insights into geographic disparities, trends over time, and the cost of meals across different regions.  

Users interacting with this dashboard will better understand how food insecurity varies throughout, and will garner better understanding of geographic disparities. By visualizing trends over time and identifying high-need areas, stakeholders and researchers can make data-driven decisions to allocate resources effectively and implement targeted interventions.

## Data Source  
The data comes from **Feeding America’s Map the Meal Gap dataset** ([available here](https://www.feedingamerica.org/research/map-the-meal-gap/by-county/)). It includes:  
  - **County-level food insecurity rates** across the U.S.  
- **Number of food-insecure individuals and children**  
  - **Meal costs per county**  
  
  Feeding America generates these estimates using **statistical modeling** based on data from:  
  - **Current Population Survey (CPS)**  
  - **American Community Survey (ACS)**  
  - **NielsenIQ food price data**  
  
The dataset covers **all U.S. counties**, with the dashboard focusing on **Georgia (for county-level analysis) and the top 10 most food-insecure states (for temporal trends from 2019-2022)**.  

## Features  
- **Trend Analysis (Plotly Line Chart):**  
  - Tracks **food insecurity rates from 2019-2022** for the **top 10 most food-insecure states**  
  - Allows users to **compare trends across states**  
  - Interactive tooltips display **specific yearly values**  
  - Users can **filter by state** to focus on specific trends  
- **Interactive Map (Leaflet):**  
  - Displays **food insecurity rates** at the **county level in Georgia**  
  - Shows **child food insecurity rates, meal costs, and the number of food-insecure individuals**  
  - Clickable counties provide detailed statistics  

  
## Technical Details  
This dashboard is built using **R Markdown** and **Flexdashboard**. Key libraries used include:  


- `ggplot2` and `plotly` for interactive visualizations  

- `leaflet` for the interactive Georgia map  

- `tigris` and `sf` for geographic counties borders

- `flexdashboard` for dashboard layout 

- `dplyr` and `tidyverse` for data processing and merging

- `openxlsx` to read in Excel sheet data

- `bslib`for theme formatting 

## Usage  
To run this dashboard locally:  
  1. Clone the repository:  
  ```sh
git clone https://github.com/your-username/food-insecurity-dashboard.git
