# weather_app_live-_forecast
Weather app live forecast

Weather Forecast Application
This is a Python-based weather forecasting application built using Streamlit for the front end and Plotly for data visualization. The app provides weather forecasts for the next few days based on user inputs and displays either temperature trends or sky conditions (e.g., clear, cloudy, rainy).

Features
Input a location to get weather forecasts.
Select the number of forecast days (1–5 days).
Choose between Temperature or Sky Conditions visualization:
Temperature: Displays a line chart of daily temperatures.
Sky Conditions: Displays corresponding images for the weather (e.g., clouds, rain).
How It Works
The app uses a backend function (get_data) to fetch weather data based on the selected location and number of forecast days.
If the user selects:
Temperature: A line chart of daily temperature trends is displayed using Plotly.
Sky: Weather condition images (clear, cloudy, rainy, etc.) are displayed based on the forecast.
User-friendly error handling informs the user if the location does not exist or the data cannot be fetched.
Requirements
Python Libraries:
Streamlit: For building the web application.
Plotly: For creating interactive temperature plots.
Pillow: For displaying weather condition images.
External Files:
backend.py: Handles fetching weather data (ensure this is implemented and functional).
images/: A folder containing weather condition images:
clear.png
cloud.png
rain.png
snow.png
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/weather-forecast-app.git
cd weather-forecast-app
Install the required Python libraries:

bash
Copy code
pip install streamlit plotly pillow
Run the application:

bash
Copy code
streamlit run app.py
Folder Structure
bash
Copy code
weather-forecast-app/
│
├── app.py            # Main Streamlit application
├── backend.py        # Backend script to fetch weather data
├── images/           # Folder for weather condition images
│   ├── clear.png
│   ├── cloud.png
│   ├── rain.png
│   ├── snow.png
└── README.md         # Project documentation
Usage
Launch the app using streamlit run app.py.
Enter a place name in the input box (e.g., "New York").
Select the number of forecast days (1 to 5) using the slider.
Choose what data to display:
Temperature: Shows a line chart with daily temperatures.
Sky: Displays images representing the sky condition for each day.
Error Handling
If the application cannot find data for the given location, an error message is displayed:

Copy code
That place does not exist.
Future Improvements
