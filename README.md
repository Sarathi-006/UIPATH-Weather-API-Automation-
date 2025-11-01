## UiPath – Weather API Automation Workflow
This repository contains a UiPath workflow that demonstrates how to:

- Fetch real-time weather data using a public API
- Extract temperature, humidity, and conditions from the API response
- Display results in the UiPath output panel or Message Box
## Project Overview
- Built using UiPath Studio (Modern Design Experience)
- Demonstrates usage of HTTP Request, Deserialize JSON, and Assign activities
- Perfect for learning API integration and JSON parsing in UiPath
## Project Files
- Main.xaml → The main automation workflow
- project.json → UiPath project configuration file
## Workflow Logic
# HTTP Request
Sends a GET request to the Weather API endpoint, for example: https://api.openweathermap.org/data/2.5/weather?q=Chennai&appid=YOUR_API_KEY&units=metric
Retrieves real-time weather data in JSON format.
🔹 Deserialize JSON
Converts the JSON response into a readable UiPath object.
Enables easy extraction of nested fields like main.temp, main.humidity, and weather[0].description.
🔹 Assign / Message Box
# Extracts and displays key details such as:
City: Chennai
Temperature: 30°C
Humidity: 70%
Condition: Clear sky
