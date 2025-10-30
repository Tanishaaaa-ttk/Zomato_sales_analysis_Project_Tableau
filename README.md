# Zomato_sales_analysis_Project_Tableau
Project report 
📊 Project Overview:-
The Zomato Sales Analysis Dashboard is an interactive data visualization project built using Tableau to analyze restaurant trends across multiple countries and cities.
The goal is to explore restaurant distribution, customer ratings, cuisines, online delivery adoption, and booking behavior — all in one visual dashboard.
By transforming raw Zomato data into meaningful visuals, this project delivers data-driven insights that help businesses and analysts understand restaurant performance and customer preferences globally.

🧩 Data Modeling Process:-
Data modeling was designed in Tableau to connect and organize relationships between multiple datasets.
Model Design:
Primary Table: Restaurant information (Restaurant ID, Name, Country, City, Cuisines, Votes, Ratings, Price Range).
Supporting Tables:
Country Table – Contains country names and codes.
Date Table – Created to support yearly, quarterly, and monthly trend analysis.
Joins & Relationships:
Linked Country Code to the Country Table.
Connected date fields for time-based trend analysis.
Calculated Fields Created in Tableau:
Average Ratings = AVG([Rating])
Total Votes = SUM([Votes])
Restaurant Count = COUNTD([Restaurant ID])
% of Online Delivery = (COUNT(IF [Has Online Delivery] = "Yes" THEN 1 END)) / COUNT([Restaurant ID])
% of Table Booking = (COUNT(IF [Has Table Booking] = "Yes" THEN 1 END)) / COUNT([Restaurant ID])
This model allows dynamic filtering and multi-level insights across years, quarters, and countries.

💡 Key Insights:-
7,424 restaurants are analyzed across 140 cities and 15 countries.
Average rating: 2.89 — indicates moderate customer satisfaction levels globally.
New Delhi leads with over 10,000+ restaurants, showing high Zomato presence in India.
North Indian, Chinese, and Fast Food cuisines are the most dominant globally.
Around 70% of restaurants do not offer online delivery, while 30% have integrated online services.
Table booking availability is low (≈16%), showing an opportunity for restaurant growth in that service area.
The highest restaurant openings are observed in Q3, indicating strong seasonal trends.

Filters Used:-
Year
Country
City
Cuisine Type
Price Range
These filters make the dashboard highly interactive and user-friendly for deep analysis.
