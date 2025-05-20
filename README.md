#  Delivery Performance Insights & Forecast using Power BI

##  Project Overview

This Power BI dashboard provides a comprehensive analysis of delivery performance across different cities, time slots, vehicle types, weather conditions, and traffic scenarios. The goal is to monitor key performance indicators (KPIs), uncover factors that contribute to delivery delays, and use data-driven forecasts to improve operational efficiency.

---

##  Features

-  **Delivery Time Analysis**: Track average delivery time by city, vehicle type, and customer age group.
-  **Delay Pattern Recognition**: Identify peak hours, festival periods, and traffic/weather conditions that contribute to late deliveries.
-  **Forecasting Module**: Predict delivery volume for the next 5 weeks based on historical trends.
-  **City Performance Overview**: Compare delivery trends across metropolitan, urban, and semi-urban areas.
-  **Customer Rating Correlation**: Analyze how delivery timeliness impacts customer satisfaction.
-  **Interactive Filters & Slicers**: Drill down by city, festival period, traffic, time bucket, and vehicle type.

---

## 🛠 Tech Stack

- **Power BI Desktop** – Dashboard development and interactive visualizations  
- **Power Query** – Data transformation and cleaning  
- **DAX** – Measures, KPIs, and calculated columns  

---

##  Project Workflow

1. **Data Ingestion**  
   Loaded datasets covering order details, delivery times, vehicle information, traffic density, weather, and customer ratings.

2. **Data Cleaning & Transformation**  
   - Removed nulls and inconsistencies  
   - Parsed delivery duration  
   - Standardized city, weather, and vehicle-type fields  

3. **Data Modeling**  
   - Defined relationships between tables  
   - Created calculated columns for delay percentages and averages  

4. **Dashboard Design**  
   - Built themed, visually intuitive reports  
   - Integrated dynamic filters, charts, and KPI cards  

5. **Insight Extraction & Forecasting**  
   - Uncovered high-risk delivery patterns  
   - Applied forecasting logic to project future deliveries

---

##  Key Analysis Questions

- What is the average delivery time across cities and time segments?
- Which vehicle type performs best in various traffic and weather conditions?
- When do most delivery delays happen?
- How do customer ratings vary based on delivery timeliness?
- What does the delivery volume forecast look like for the next 5 weeks?

---

##  Dashboard Views

![image](https://github.com/user-attachments/assets/5b875aa1-391a-4bb3-8a34-62cd53d2a36e)
![image](https://github.com/user-attachments/assets/ee34fa47-a895-4d45-aa1b-83e85f613950)
![image](https://github.com/user-attachments/assets/c6815d3d-bce9-4bc0-90c7-23d949743fab)
![image](https://github.com/user-attachments/assets/b5314705-3952-4049-b074-dd1705c17684)
![image](https://github.com/user-attachments/assets/70d815db-58b0-44a4-b4fb-fe9e3f14fee6)



###  Overview Dashboard
- Total Deliveries, Average Delivery Time, Rating
- Delivery Volume by Age Group
- Orders by Time Segment (e.g., 6PM–Midnight)

###  Traffic & Timing Analysis
- Delivery Time by Traffic Density and Weather Conditions
- Delays by Time of Day

###  Delivery Partner Performance
- Performance by Vehicle Type (e.g., Scooter, Motorcycle, E-Scooter)
- Delivery Time vs Rating Correlation

#### Factors Contributing to Delays
- Festival Impact
- Traffic × Weather × Time Bucket Combinations (Top Delay Scenarios)

###  Forecast View
- Weekly Delivery Trend (Past & Next 5 Weeks)
- Expected Order Volume Stability (~2.8K/week)

>  Dynamic slicers for: City, Festival, Traffic, Weather, Vehicle Type, Time Bucket

---

##  Sample DAX Measures

``DAX
Average Delivery Time = AVERAGE('Orders'[Delivery_Time])
On-Time Percentage = DIVIDE([On-Time Orders], [Total Orders], 0)
Late Deliveries = CALCULATE([Total Orders], 'Orders'[Status] = "Late")


##  Sample Insights

-  **70.85%** of on-time deliveries receive higher customer ratings.
-  **6PM–Midnight** is the busiest delivery window and the most delay-prone.
-  Deliveries made during **Jam traffic + Foggy weather** conditions face up to a **76% delay rate**.

---

##  Limitations

- The dataset does **not include financial or operational costs**.
- Forecasting is based on **historical delivery trends**, not real-time data.
- Customer feedback is limited to **star ratings only**, lacking qualitative insights.

---

##  How to Use

1. **Clone this repository**
2. **Open** `Delivery_Performance_Dashboard.pbix` **in Power BI Desktop**
3. **Explore the dashboards** using built-in filters and slicers
4. **Customize the visuals** or connect your own dataset as needed

---


## Author
### — Sudeshna Dey
###  — Contact & Contributions

####  Email: sudeshnadey1000@gmail.com
####  LinkedIn: https://www.linkedin.com/in/sudeshna-dey-724a811a0/
 Have feedback or suggestions? I'm always open to improving and collaborating!
 
If you find this project helpful:
 Give it a star
Thanks for visiting — and happy data analyzing!
