
# Weather Forecast CLI Application 🌤️

This is a simple Go-based CLI application that fetches and displays current and hourly weather forecast data for a specified location using the [WeatherAPI](https://www.weatherapi.com/).

## Features
- Fetches current weather details and displays temperature and condition.
- Provides an hourly forecast for the next 24 hours.
- Highlights forecast hours with a high chance of rain using colored output.
- Supports dynamic location input through command-line arguments.

## Installation
To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/weather-cli-app.git
   cd weather-cli-app
   ```

2. Install dependencies (e.g., `fatih/color`):
   ```bash
   go get github.com/fatih/color
   ```

3. Build the application:
   ```bash
   go build -o weather
   ```

4. Set up your environment variable for the Weather API key:
   - Replace `YOUR_API_KEY` with your WeatherAPI key:
   ```bash
   export WEATHER_API_KEY=YOUR_API_KEY
   ```

## Usage
Run the CLI application with the following command:

```bash
./weather [location]
```

### Example
```bash
./weather "Lucknow"
```
If no location is provided, the default location "Lucknow" will be used.

## Output Format
- Displays the current weather condition and temperature of the specified location.
- Displays hourly forecast with temperature, chance of rain, and conditions.
- Uses colored text to highlight hours with a high chance of rain.

## Code Structure
- `main.go`: The main file containing the logic to fetch and parse weather data from the WeatherAPI.

## Dependencies
- [fatih/color](https://github.com/fatih/color): A Go library used for colored output in the terminal.

## API Key
To use this application, you need to sign up for a free API key at [WeatherAPI](https://www.weatherapi.com/) and set it as an environment variable:

```bash
export WEATHER_API_KEY=your_api_key
```

## Future Improvements
- Add support for extended forecast (up to 7 days).
- Allow user to configure output formats (e.g., JSON, plain text).
- Add unit tests for error handling and JSON parsing.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing
Contributions are welcome! Please fork this repository and submit a pull request with your changes.

---

**Author**: Abhay Gupta
```

Replace placeholders like `your-username` and `YOUR_API_KEY` with your actual GitHub username and WeatherAPI key. Let me know if you need help with any specific sections or want to include more information!
