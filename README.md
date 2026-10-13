# WeatherCast - Python Weather Prediction App

A desktop weather application built with Python and Tkinter. WeatherCast displays current weather conditions, air quality, a 48-hour forecast, and a 7-day outlook for Indian cities and other locations.

## Student / Developer Details

- **Name:** Prince Raj
- **Email:** princerajsinha979@gmail.com

> Note: The email address above is written exactly as provided. If you intended a conventional email address, check whether an `@` symbol is missing.

## Features

- Current weather conditions, including temperature and feels-like temperature
- Humidity, wind speed and direction, surface pressure, and precipitation
- Air quality information (US AQI, PM2.5, and PM10)
- Hourly weather forecast for the next 48 hours
- 7-day forecast with high/low temperatures and precipitation chance
- Sunrise and sunset times, plus a daylight visual
- Celsius and Fahrenheit display
- Search for Indian cities, with quick-select buttons for popular cities
- Optional worldwide city search
- Weather-based themes for clear, cloudy, rainy, snowy, and stormy conditions
- Background data fetching to keep the interface responsive

## Technologies Used

- **Python 3**
- **Tkinter / ttk** for the graphical user interface
- Python standard-library modules: `urllib`, `json`, `threading`, `queue`, `datetime`, `math`, `ssl`, and `traceback`
- **Open-Meteo Forecast API**
- **Open-Meteo Geocoding API**
- **Open-Meteo Air Quality API**

No API key is required for the Open-Meteo endpoints used by this project.

## Requirements

- Python 3.9 or newer recommended
- Internet connection
- Tkinter installed with your Python distribution

Most Python installations include Tkinter. On some Linux distributions, it may need to be installed separately.

## Project Structure

```text
WeatherCast/
├── weather_app.py
└── README.md
```

## Installation and Setup

### 1. Clone the repository

Replace `YOUR-USERNAME` with your GitHub username:

```bash
git clone https://github.com/YOUR-USERNAME/WeatherCast.git
cd WeatherCast
```

Alternatively, download the project files and open the project folder in VS Code.

### 2. Check Python

```bash
python3 --version
```

### 3. Run the application

If your Python file is named `weather_app.py`, run:

```bash
python3 weather_app.py
```

On Windows, you can usually use:

```bash
python weather_app.py
```

The app starts by loading weather information for Raipur by default. Use the search field or city quick-select buttons to view another location.

## APIs Used

- **Weather forecast:** https://open-meteo.com/en/docs
- **Geocoding:** https://open-meteo.com/en/docs/geocoding-api
- **Air quality:** https://open-meteo.com/en/docs/air-quality-api

Weather and air-quality data require an active internet connection. Air-quality data is optional; the application can still display weather if the AQI request fails.

## How It Works

1. The user selects or searches for a city.
2. The app obtains the city's latitude and longitude, using built-in coordinates for supported Indian cities or the geocoding service.
3. It requests current, hourly, and daily forecast data from Open-Meteo.
4. It requests air-quality data separately.
5. The Tkinter interface displays the results in **Now**, **48-Hour**, and **7-Day** tabs.

## Troubleshooting

- **No data / network error:** Check your internet connection and try again.
- **City not found:** Check the spelling. If **India only** is enabled, searches are restricted to Indian locations.
- **Tkinter import error:** Install the Tkinter package appropriate for your operating system or use a Python distribution that includes it.
- **SSL certificate error:** Update your Python installation and certificate store. Avoid disabling SSL certificate verification as a general solution.

## Future Improvements

- Add weather charts and historical weather comparisons
- Add severe-weather alerts
- Add saved locations and a favorites list
- Add unit tests and automated checks
- Improve accessibility and responsive layouts

## Author

**Prince Raj**  
Email: `princerajsinha979@gmail.com`

## License

No license has been specified yet. Add a license file before distributing or reusing this project publicly.
