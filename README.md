# Data-Visualisation---Jupyter
Importance of Data Visualisation Core Skill: Essential for data analysts, data scientists, and even non-professionals. Purpose: Helps interpret data, identify trends, and drive decision-making. Applications: Used in exploratory data analysis (EDA) and communicating insights effectively.


# Goals
Primary: Identify relationships between bike sharing data and weather conditions using:
Line plots
Scatter plots
Bar plots

Secondary: Understand which visualizations are appropriate for various data types (categorical, continuous, time-based).
  
# Tools Used
Jupyter Lab: IDE
Pandas: For data manipulation.
Plotly: For interactive visualizations (preferred over Matplotlib for its features and aesthetics).

# Data Overview
Dataset includes hourly bike rental data in Seoul (2017–2018).
Columns include date, time, number of rented bikes, weather conditions, etc.
Data Cleaning Steps

# Date Conversion:
Convert date strings to datetime for easier filtering and visualization.
Combine date and hour into a single datetime column using apply and lambda.

# Boolean Conversion:
Convert categorical columns like is_holiday and is_functioning to boolean (True/False) for easier filtering.

# Filter Data:
Retain only rows where the system was functioning using the query function.
Line Plot: Rentals Over Time

# Why Line Plots?:
Best for showing progression over time.

# Steps:
Visualize hourly rentals using px.line().
Add markers for weekends to highlight patterns.
Aggregate data by day to reduce noise and visualize seasonality.
Grouping by Season
Use the season column to group data and plot rentals by season.
Map season to color for better interpretability.
Scatter Plot: Weather vs. Rentals

# Purpose:
Identify relationships between two variables (e.g., temperature and rentals).

# Steps:
Filter data for a specific time (e.g., noon) to ensure fair comparisons.
Use scatter plots (px.scatter) to visualize relationships.
Key Insights
Line plots reveal seasonal trends (e.g., higher rentals in summer).
Scatter plots show correlations, such as temperature affecting bike rentals.
Data cleaning and transformation are crucial for effective visualization.
Practical Tips
Focus on realistic datasets for meaningful analysis.
Use interactive tools like Plotly to explore data in detail.
Select visualization types based on the nature of the data and the relationships being examined.
