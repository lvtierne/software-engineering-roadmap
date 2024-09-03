# Weather App

## Objective
Build a weather application that fetches and displays the current weather based on user input.

## Features
- Input a city name.
- Fetch current weather data from a weather API.
- Display temperature, weather conditions, and other relevant data.

## Steps
1. **Choose a Language**: Implement the app using a language of your choice (e.g., JavaScript, Python).
2. **Use an API**: Obtain weather data from a weather API (e.g., OpenWeatherMap API).
3. **Design the Interface**: Create an interface for inputting a city and displaying weather data.
4. **Fetch Data**: Write code to make API requests and handle responses.

## Example Code
### JavaScript: Weather App
```html
<!DOCTYPE html>
<html>
<head>
    <title>Weather App</title>
</head>
<body>
    <h1>Weather App</h1>
    <input type="text" id="cityInput" placeholder="Enter city...">
    <button onclick="getWeather()">Get Weather</button>
    <div id="weather"></div>

    <script>
        async function getWeather() {
            const city = document.getElementById('cityInput').value;
            const apiKey = 'YOUR_API_KEY'; // Replace with your API key
            const response = await fetch(`https://api.openweathermap.org/data/2.5/weather?q=${city}&appid=${apiKey}`);
            const data = await response.json();
            document.getElementById('weather').innerHTML = `
                <h2>${data.name}</h2>
                <p>Temperature: ${(data.main.temp - 273.15).toFixed(2)} °C</p>
                <p>Weather: ${data.weather[0].description}</p>
            `;
        }
    </script>
</body>
</html>
```

## Learning Resources

- [Weather App Tutorial - YouTube](https://www.youtube.com/watch?v=l5s9TtHkP6Q)
