Weather Analytics Dashboard – Power BI
Project Overview
The Weather Analytics Dashboard is an interactive Power BI report designed to provide real-time and forecast-based weather insights for Bangalore.
This dashboard delivers a complete weather overview including temperature trends, air quality metrics, humidity, wind speed, UV index, and rainfall probability.
The goal of this project is to demonstrate:
•	Data visualization skills
•	KPI modeling using DAX
•	Interactive dashboard design
•	Real-world business-style reporting
________________________________________
Dashboard Preview
 
![Weather Dashboard](Weather_dashboard.png)
________________________________________
Key Features
Current Weather Summary
•	Current Temperature: 29.2°C
•	Weather Condition: Sunny
•	Location: Bangalore
•	Last Updated Date Display
•	City comparison (Ajmer, Bangalore, Bhopal)
________________________________________
3-Day Weather Forecast
Line chart displaying:
•	Saturday
•	Sunday
•	Monday
Shows temperature trend visually for quick understanding of fluctuation.
________________________________________
Sunrise & Sunset Panel
•	Sunrise: 06:42 AM
•	Sunset: 06:25 PM
Useful for daylight duration analysis.
________________________________________
Weather Indicators (KPI Cards)
The dashboard includes:
•	Humidity (%)
•	Wind Speed (Kph)
•	Visibility (KM)
•	Pressure (mm)
•	UV Index
•	Precipitation (mm)
These metrics provide a complete environmental overview.
________________________________________
Air Quality Overview
Includes:
•	AQI Status Indicator (Good – 23)
•	PM10
•	PM2.5
•	SO2
•	NO2
•	CO
•	O3
Color-coded indicators improve readability and user experience.
________________________________________
Chances of Rain
Bar visual showing rain probability for:
•	Saturday
•	Sunday
•	Monday
Helps users plan activities accordingly.
________________________________________
Tools & Technologies Used
•	Power BI Desktop
•	DAX (Data Analysis Expressions)
•	Data Modeling
•	KPI Cards
•	Line Chart
•	Bar Chart
•	Gauge Visual
•	Custom Layout & UI Design
________________________________________
DAX Calculations Used
Examples of measures created:
Average Temperature = AVERAGE(Weather[Temperature])

Rain Probability % = 
DIVIDE(
    SUM(Weather[RainChance]),
    COUNT(Weather[Day])
)

AQI Status = 
IF([AQI Value] <= 50, "Good",
   IF([AQI Value] <= 100, "Moderate", "Unhealthy"))
________________________________________
Business Use Case
This dashboard can be used by:
•	Travel agencies
•	Event planners
•	Environmental analysts
•	City monitoring authorities
•	Weather tracking applications
It enables quick, visual, and interactive weather analysis.
________________________________________
Insights Derived
•	Temperature is stable between 23–29°C.
•	AQI level is within "Good" range.
•	UV Index is high (12), indicating sun exposure risk.
•	Rain probability varies by day.
________________________________________
Repository Structure
Weather-Dashboard/
│
├── Weather Dashboard.pbix
├── Weather_dashboard.png
└── README.md
________________________________________
How to Use
1.	Download the .pbix file
2.	Open in Power BI Desktop
3.	Refresh data (if connected to live source)
4.	Interact using filters and visuals
________________________________________
Future Improvements
•	Real-time API integration
•	Multi-city comparison
•	Monthly trend analysis
•	Mobile responsive layout
•	Historical weather data trends


