# Weather.io Dashboard Application

A modern, interactive weather dashboard that provides real-time weather information, user temperature reporting, and advanced weather data visualization. This application combines real-time weather data with user-reported temperatures to create a comprehensive weather monitoring system.

## Features

### Real-time Weather Data
- Live weather updates from OpenWeather API
- Current temperature, humidity, wind speed, and pressure
- UV index and visibility information
- Weather condition descriptions with icons

### Interactive Temperature Reporting
- Users can report their local temperature
- Daily temperature reports are automatically cleared
- Temperature data is stored in Firebase for persistence
- Real-time visualization of user-reported temperatures

### Advanced Data Visualization
- Interactive charts using Chart.js
- Hourly and daily temperature forecasts
- Precipitation analysis with rain and snow data
- Historical temperature trends and patterns
- User-reported temperature averages

### User Experience
- Responsive design works on all devices
- Dark/light mode support
- Customizable temperature units (Celsius/Fahrenheit)
- Time format preferences (12h/24h)
- Location-based weather tracking

## Live Demo

[https://psu.mediaspace.kaltura.com/media/Shen-Han+Chius+Zoom+Meeting/1_wo09g87y]

## Prerequisites

Before you download the files, please follow the requirements:

### System Requirements
- A modern web browser (Chrome, Firefox, Safari, or Edge)
- Node.js (v14.0.0 or higher)
- npm (v6.0.0 or higher)
- Stable internet connection

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/weather-dashboard.git
cd weather-dashboard
```

### 2. Install Dependencies
```bash
npm install
```
This will install all required packages:
- Chart.js for data visualization
- Firebase for data storage
- Leaflet for map integration
- Other utility packages

## Usage

### 1. Starting the Application
```bash
npm start
```
This will:
- Start the development server
- Compile all assets
- Open your default browser to `http://localhost:3000`

### 2. Initial Setup
- Allow location access when prompted
- The application will automatically fetch weather data for your location
- Your preferences will be saved in local storage

### 3. Using the Dashboard

#### Viewing Weather Data
- Current weather conditions are displayed at the top
- Hourly forecast shows the next 24 hours
- Daily forecast provides a 5-day outlook
- Precipitation chart shows expected rain and snow

#### Reporting Temperature
1. Enter your local temperature in the input field
2. Click "Submit" or press Enter
3. Your report will appear in the visualization
4. Reports are cleared daily at midnight

#### Customizing Display
- Toggle between Celsius and Fahrenheit
- Switch between 12-hour and 24-hour time formats
- Adjust chart display preferences
- Change location manually or use current location

## Testing

### 1. Temperature Reporting Test
1. Enter a temperature value (e.g., 25°C)
2. Submit the temperature
3. Verify that:
   - The temperature appears in the chart
   - The data is stored in Firebase
   - The visualization updates correctly

### 2. Visualization Testing
Check the hourly forecast chart for:
- API Temperature (red line)
  - Should show current and forecasted temperatures
  - Updates every 3 hours
- Feels Like Temperature (green line)
  - Should follow a similar pattern to actual temperature
  - Accounts for humidity and wind
- User Average (blue dashed line)
  - Should show the average of all user reports
  - Updates in real-time as new reports come in

### 3. Location Features
Test location functionality:
1. Click "Get Current Location"
   - Should update to your current location
   - Weather data should refresh
2. Click on the map
   - Should update to the clicked location
   - All data should update accordingly

## Project Structure
```
weather.io/
├── index.html          # Main HTML file with UI structure
├── styles.css         # CSS styles and responsive design
├── script.js         # Main JavaScript file with all functionality
├── README.md        # Documentation
└── package.json    # Project dependencies and scripts
```

### Key Files Explained

#### index.html
- Contains the main UI structure
- Includes all necessary script and style imports
- Defines the layout for weather information display

#### styles.css
- Defines the visual appearance
- Implements responsive design
- Contains animations and transitions
- Manages dark/light mode styles

#### script.js
- Handles all application logic
- Manages API calls and data processing
- Implements chart visualizations
- Handles user interactions and data storage


This project is licensed under the PSU License

The PSU License allows you to:
- Use the code commercially
- Modify the code
- Distribute the code
- Use the code privately
- Sublicense the code

## Acknowledgments

- [OpenWeather API](https://openweathermap.org/api) for providing weather data
- [Firebase](https://firebase.google.com/) for backend services and data storage
- [Chart.js](https://www.chartjs.org/) for data visualization
- [Leaflet](https://leafletjs.com/) for map integration
- Thank you Professor Kaamran Raahemifar, Shen-Han Chiu, and Jacob O'Leary for their contribution and sugguestions to improve this project. 

## Contact

Shen-Han Chiu - [spc6178@psu.edu]
Applied Data Science | College of Information Sciences and Technology
The Pennsylvania State University
E301 Westgate Building, University Park, PA 16802
814-280-7039 (office) | spc6178@psu.edu

Project Link: [https://github.com/yourusername/weather-dashboard](https://github.com/yourusername/weather-dashboard)

Contact Shen-Han Chiu at spc6178@psu.edu for further support. 
