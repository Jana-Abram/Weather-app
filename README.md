🌦️ Weather App

A sleek weather forecast app built with React + Vite, powered by the WeatherAPI. Search by city name or use your current location to get real-time conditions and an hourly forecast for the next 24 hours.

🔗 Live Demo:

✨ Features


Search by city — type any city name to get its current weather
Geolocation support — one click to get weather for your current location (with browser permission)
Current conditions — temperature, weather description, and a matching weather icon
24-hour forecast — scrollable hourly forecast list starting from the current hour
Dynamic weather icons — icon automatically matches the weather condition code returned by the API
Error handling — friendly fallback screen when a city isn't found or the request fails
Responsive, card-style UI — clean gradient design that adapts to mobile and desktop


🛠️ Built With


React — component-based UI (functional components + hooks: useState, useRef)
Vite — fast dev server & build tool
WeatherAPI — real-time weather & forecast data
CSS3 — custom properties, Flexbox, gradients, responsive design
Geolocation API — browser-based location detection


📂 Project Structure

weather-app/
├── src/
│   ├── components/
│   │   ├── SearchSection.jsx        # City search form + geolocation button
│   │   ├── CurrentWeather.jsx       # Current temperature & conditions display
│   │   ├── HourlyWeatherItem.jsx    # Single hourly forecast entry
│   │   └── NoResultsDiv.jsx         # Error / no-results screen
│   ├── constants.js                  # Weather condition code → icon mapping
│   ├── App.jsx                       # Main app logic & state
│   ├── main.jsx                       # React entry point
│   └── index.css                      # Global styles
├── public/
│   └── icons/                         # Weather icon SVGs
├── .env                                # API key (not committed — see below)
└── README.md

🔑 API Key Setup

This project uses a WeatherAPI key stored in an environment variable.


Get a free API key at weatherapi.com
Create a .env file in the project root:


   VITE_API_KEY=your_api_key_here


Make sure .env is listed in .gitignore — never commit your API key to a public repository.


🚀 Getting Started

This project requires Node.js and npm, since it's built with Vite.


Clone the repository:


bash   git clone https://github.com/your-username/weather-app.git
   cd weather-app


Install dependencies:


bash   npm install


Add your .env file (see API Key Setup above)
Start the development server:


bash   npm run dev


Open the local URL shown in the terminal (usually http://localhost:5173)


🖱️ How to Use


Type a city name into the search bar and press Enter, or
Click the location button to use your current location (browser will ask for permission)
View the current temperature and conditions
Scroll through the hourly forecast for the next 24 hours
