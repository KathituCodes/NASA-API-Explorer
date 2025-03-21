# NASA-API-Explorer

## 🌌 Overview
Ever wanted to pull real-time space data straight from NASA’s public APIs? This project is all about practicing API consumption retrieving astronomical data, processing it into structured formats, and exporting it for analysis. By the end of this, you’ll have hands-on experience with API requests, data handling in pandas, and saving insights to a CSV for easy sharing.

## 🎯 Objective
The goal is to practice accessing and using NASA’s public APIs to retrieve and manipulate space related data. This includes:
- Obtaining an API key from NASA’s portal.
- Making API requests to fetch data.
- Processing responses into a structured pandas DataFrame.
- Exporting results to a CSV for further analysis or sharing.

## 🛠️ How It Works
1. **Generate Your API Key** – Head to the [NASA API Portal](https://api.nasa.gov/) and request your personal API key.
2. **Make API Requests** – Use Python’s `requests` library to call endpoints.
3. **Fetch Astronomy Picture of the Day (APOD)** – Retrieve and display NASA’s featured space image.
4. **Extract Asteroid Data** – Pull asteroid details from the **Near Earth Object Web Service (NeoWs)**.
5. **Clean and Process Data** – Transform the raw asteroid data into a structured pandas DataFrame with these key columns:
   - `Asteroid ID`
   - `Asteroid Name`
   - `Minimal Estimated Diameter (km)`
   - `Absolute Magnitude`
   - `Relative Velocity (km/s)`
6. **Export Data to CSV** – Save the cleaned dataset for sharing or further analysis.

## 📌 Usage
### Installation
Ensure you have the required libraries installed:
```bash
pip install requests pandas
```

### Running the Script
```python
from nasa_api_explorer import fetch_asteroid_data

data = fetch_asteroid_data()
data.to_csv("asteroid_data.csv", index=False)
print("Asteroid data saved successfully!")
```

### Expected Output
A structured CSV file (`asteroid_data.csv`) with cleaned asteroid details, ready for analysis or visualization.

## 🎯 Why Use This?
- **Hands-on API practice** – Learn how to consume and manipulate real-world data.
- **Work with live NASA data** – Explore asteroid information and stunning space imagery.
- **Data science-ready** – The cleaned dataset is ideal for further analysis, visualization, or machine learning projects.

## 🚀 Future Enhancements
- Automate API calls for daily updates.
- Expand data collection to include other NASA APIs (e.g., Mars Rover photos).
- Create visualizations of asteroid orbits and sizes.

---
Get your API key, start exploring, and let the data take you to the stars! ✨

