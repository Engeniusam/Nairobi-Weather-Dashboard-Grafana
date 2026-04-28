# 🌤️ Nairobi Weather Dashboard — Grafana

A live weather dashboard built with **Grafana** and the **Infinity datasource**,
pulling real-time data from the OpenWeatherMap API.

![Nairobi Weather Dashboard](<img width="1528" height="1146" alt="Nairobi Weather Dashboard-1777371107957" src="https://github.com/user-attachments/assets/6b636136-1730-4b42-af7f-ef46ae94278c" />
)

## 📊 What It Shows

| Panel | Data |
|---|---|
| 🌡️ Temperature | Current temp in °C |
| 💧 Humidity | Relative humidity % |
| 💨 Wind Speed | Wind speed in m/s |
| 📍 Summary Table | City, country, feels like, visibility |

## 🔧 How It Works

1. **Datasource**: [Infinity](https://grafana.com/grafana/plugins/yesoreyeram-infinity-datasource/)
   — a Grafana plugin that fetches data from any HTTP URL
2. **API**: [OpenWeatherMap](https://openweathermap.org/api) free current weather endpoint
3. **Data extraction**: jq selectors pull specific fields from the JSON response
   e.g. `main.temp` → temperature, `wind.speed` → wind speed

## 🚀 Import This Dashboard

1. Open Grafana → **Dashboards → Import**
2. Upload `nairobi-weather-dashboard.json`
3. Select your Infinity datasource
4. Click **Import**

> ⚠️ You will need your own [OpenWeatherMap API key](https://home.openweathermap.org/api_keys)
> and update it in each panel query.

## 🔑 API Endpoint Used
