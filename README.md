# weather-analytics-dashboard
Interactive Weather Analytics Dashboard built using Power BI and OpenWeather API

# 🌦️ Weather Intelligence Dashboard

An interactive **Real-Time Weather Intelligence Dashboard** built using **Microsoft Power BI** and the **OpenWeather API** to monitor, compare, and analyze weather conditions across multiple cities.

## 📊 Dashboard Preview

[Weather Intelligence Dashboard](Images/dashboard-overview.png)

## 🎯 Project Objective

The goal of this project is to transform real-time weather API data into an interactive and visually appealing analytical dashboard.

The dashboard helps users:

* Monitor current weather conditions
* Compare weather conditions across cities
* Analyze temperature, humidity, pressure, wind speed and visibility
* Evaluate weather comfort levels
* Identify weather-related risks
* Monitor API data freshness

## ✨ Key Features

### 🌡️ Weather KPI Cards

Displays:

* Average Temperature
* Average Humidity
* Average Pressure
* Average Wind Speed
* Visibility
* Weather Comfort Score

### 🏙️ City Analysis

The dashboard allows users to select and compare:

* Bengaluru
* Chennai
* Hyderabad

### 😊 Weather Comfort Score

A DAX-based scoring system evaluates weather conditions using:

* Temperature
* Humidity
* Wind Speed

The score provides an easy-to-understand indication of overall weather comfort.

### ⚠️ Weather Risk Overview

The dashboard provides analytical risk indicators for:

* Heat Risk
* Wind Risk
* Humidity Risk

### 🗺️ Geographic Analysis

A Power BI map visual displays weather information based on city locations using latitude and longitude.

### 🌅 Sunrise & Sunset

Displays the sunrise and sunset times for the selected city.

### 📊 City Comparison

Interactive comparison of:

* Temperature
* Humidity
* Wind Speed

across the selected cities.

### 🟢 Live Data Indicator

The dashboard includes:

* LIVE status
* Last Updated timestamp

to indicate the freshness of the API data.

## 🏗️ Data Model

The project uses a dimensional data model with:

```text
              DimCity
                 │
                 │ 1 : *
                 ▼
        Weather_All_Cities
                 ▲
                 │
                 │ 1 : *
              DimDate
```

### Dimension Tables

**DimCity**

* City
* Country
* Latitude
* Longitude

**DimDate**

* Date
* Day
* Month Name
* Quarter
* Year

### Weather Data

The main weather table contains API-based weather information such as:

* Temperature
* Feels Like
* Humidity
* Pressure
* Wind Speed
* Cloudiness
* Visibility
* Sunrise
* Sunset
* Recorded DateTime

## 🧮 DAX

DAX measures were created for:

* Weather KPIs
* Average weather metrics
* Weather Comfort Score
* Weather Risk Analysis
* Last Updated timestamp
* Dynamic weather insights

## 🔄 Data Pipeline

```text
OpenWeather API
       ↓
Power Query
       ↓
Data Cleaning & Transformation
       ↓
DimCity + DimDate
       ↓
Data Model
       ↓
DAX Measures
       ↓
Power BI Dashboard
```

## 🛠️ Technologies Used

| Technology         | Purpose                        |
| ------------------ | ------------------------------ |
| Microsoft Power BI | Dashboard & Visualization      |
| Power Query        | Data Cleaning & Transformation |
| DAX                | Calculations & Measures        |
| OpenWeather API    | Weather Data                   |
| Data Modeling      | Dimensional Data Model         |
| GitHub             | Project Version Control        |

## 📍 Cities Covered

Currently, the dashboard analyzes:

1. Bengaluru
2. Chennai
3. Hyderabad

## 🚀 How to Use

1. Download the `.pbix` file from this repository.
2. Open it using Microsoft Power BI Desktop.
3. Configure the OpenWeather API connection if required.
4. Refresh the data.
5. Use the city selector to explore weather conditions.
6. Interact with the dashboard visuals to compare cities and analyze weather patterns.

## 📁 Project Structure

```text
weather-intelligence-dashboard/
│
├── PowerBI/
│   └── Weather_Intelligence_Dashboard.pbix
│
├── Images/
│   └── dashboard-overview.png
│
└── README.md
```

## 📈 Skills Demonstrated

This project demonstrates practical experience with:

* Power BI Dashboard Development
* DAX
* Power Query
* Data Cleaning
* Data Modeling
* Star Schema
* API Integration
* Interactive Data Visualization
* KPI Development
* Data Analysis
* Business Intelligence

## 👩‍💻 Project Type

**Data Analytics / Business Intelligence Project**

Built as a portfolio project to demonstrate practical Power BI, DAX, API integration, and data visualization skills.

## 📌 Future Improvements

* Add more cities
* Add multi-day weather forecasting
* Add historical weather analysis
* Add precipitation analysis
* Add weather alerts
* Add automated refresh
* Add more advanced weather risk indicators
* Add AI-powered weather recommendations

---

⭐ If you find this project useful, consider giving the repository a star!
