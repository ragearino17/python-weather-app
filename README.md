# 🌤️ PyQt5 Weather Dashboard

A sleek, responsive desktop application built with Python and PyQt5 that displays real-time weather information using the OpenWeatherMap API. The app features robust error handling, professional modern styling, and clean dynamic icon mapping.

## ✨ Features
- **Real-Time Data**: Fetches accurate live weather metrics (temperature, descriptions) directly from the OpenWeatherMap endpoint.
- **Dynamic Emoji Mapping**: Custom condition algorithms smoothly translate raw weather IDs (200-804) into vibrant visual indicators (e.g., ⛈️ for thunderstorms, ❄️ for snow).
- **Secure Configuration**: Uses `python-dotenv` environment variables to completely keep sensitive API credentials hidden from public source control.
- **Comprehensive Error Handling**: Built-in HTTP response catch blocks to gracefully display user-friendly warnings for invalid text inputs, bad requests, timeouts, or network loss.

## 🚀 Installation & Setup
Follow these steps to run the desktop app locally on your machine:

1. **Clone the repository:**
   ```bash
   git clone https://github.com
   cd python-weather-app
   ```

2. **Set up a Virtual Environment & install dependencies:**
   ```powershell
   python -m venv .venv
   .venv\Scripts\Activate.ps1
   pip install -r requirements.txt
   ```

3. **Configure your API Key:**
   Create a file named `.env` in the root directory and add your unique token string:
   ```env
   WEATHER_API_KEY=your_actual_openweathermap_api_key
   ```

4. **Launch the application:**
   ```bash
   python main.py
   ```

## 🔑 How to Get Your Own API Key

This application requires an active API key from OpenWeatherMap. Follow these quick steps to get yours for free:

1. **Create a Free Account:** Go to the [OpenWeatherMap Sign-Up Page](https://openweathermap.org) and register a free developer profile.
2. **Access Your Keys:** Once logged in, navigate to the **API keys** tab in your dashboard panel (or visit [home.openweathermap.org/api_keys](https://openweathermap.org)).
3. **Generate a Key:** You will see a default key automatically generated for you. If needed, you can type a custom name (like `Weather App`) and click **Generate** to create a fresh one.
4. **Copy & Wait:** Copy the long string of letters and numbers. 
   
> ⚠️ **Note:** OpenWeatherMap takes anywhere from **10 minutes to 2 hours** to activate new keys globally on their servers. If your app returns an "Invalid API key" error immediately after signing up, wait a short while and try again!

## 🛠️ Built With
- **Python 3** - Core language execution logic
- **PyQt5** - Desktop UI layout construction and object styling
- **Requests** - Thread-safe API network communication 
- **Python-Dotenv** - Secure environment file parsing
