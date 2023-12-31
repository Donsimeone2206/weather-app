# Weather App

## Overview

This is a simple Weather App that uses the OpenWeatherMap API to fetch weather data based on a city input. The app displays the current temperature, humidity, wind speed, and a weather icon corresponding to the current weather condition.

## Setup

1. **API Key**: The app uses an API key to access the OpenWeatherMap data. The key is already provided in the code as `apiKey`. If you want to use your own API key, please sign up on [OpenWeatherMap](https://openweathermap.org/) and replace the `apiKey` value with your own.

2. **API Endpoint**: The endpoint used to fetch weather data is `https://api.openweathermap.org/data/2.5/weather?units=metric&q=`. The data is fetched in metric units.

3. **Weather Icons**: Make sure you have the following images in your `images` directory:
    - `clouds.png`
    - `clear.png`
    - `rain.png`
    - `drizzle.png`
    - `mist.png`

## How to Use

1. **Search Box**: Enter the name of the city you want to check the weather for in the search input box.

2. **Search Button**: Click the search button to fetch and display the weather data for the entered city.

3. **Weather Display**: If the city is found and data is retrieved successfully, the weather data will be displayed on the page. This includes:
    - City name
    - Temperature (in Celsius)
    - Humidity (in percentage)
    - Wind speed (in km/h)
    - A weather icon representing the current weather condition (Clouds, Clear, Rain, Drizzle, or Mist).

4. **Error Handling**: If there's an error or if the city is not found, an error message will be displayed.

## Code Structure

- **API Calls**: The `checkWeather` function makes an asynchronous call to the OpenWeatherMap API, fetches the data, and updates the DOM with the weather information or displays an error message.

- **Weather Icon Update**: Based on the main weather condition, the app updates the weather icon on the page.

- **Event Listener**: An event listener is added to the search button. When the button is clicked, the `checkWeather` function is triggered with the value from the search input box.

## Note

Avoid exposing your API key in the source code for security reasons. This example uses a hardcoded key for simplicity. Consider moving it to a secure configuration or environment variable in production applications.

## Contributing

If you'd like to contribute to this project or suggest improvements, please create an issue or submit a pull request.

## License

This project is open source.
