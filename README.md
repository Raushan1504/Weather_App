# ☀️ Simple Weather App
This is a clean, single-page web application that fetches and displays current weather data for any city using the OpenWeatherMap API.
## ✨ Features
* **Real-time Data:** Fetches current temperature, humidity, and weather description.
* **Temperature Conversion:** Converts temperature from Kelvin (API default) to Celsius (°C).
* **Weather Emojis:** Displays a corresponding emoji icon (sun, rain, snow, etc.) based on the weather ID.
* **Error Handling:** Provides user feedback if a city is not found or if the API cannot be reached.
## 🚀 How to Run
### Prerequisites
You need a valid API key from OpenWeatherMap.
1.  Sign up for an account on the [OpenWeatherMap website](https://openweathermap.org/api).
2.  Generate or locate your API key.
### Local Setup
1.  **Clone the repository:**
    ```bash
    git clone [Your Repository URL Here]
    cd weather-app
    ```
2.  **Update the API Key:**
    Open the `index.js` file and replace the placeholder API key with your own:
    ```javascript
    let apikey = "YOUR_API_KEY_HERE"; // Currently set to "1ec041db49ddfd3d9377cdecfc7b110d"
    ```
3.  **Open in Browser:**
    Open the `HTML.html` file directly in your web browser (e.g., Chrome, Firefox).
## 📁 File Structure
| File | Description |
| :--- | :--- |
| `HTML.html` | The main HTML structure, including the form and the weather card container. |
| `style.css` | Handles all styling, including the background gradient and font sizes for the weather card. |
| `index.js` | Contains the core logic: API calls, data handling, temperature conversion, and DOM manipulation. |
## ⚙️ Core Logic Explained
### API Interaction
The `getWeatherData(city)` function handles fetching data:
```javascript
// Example API Call
// [https://api.openweathermap.org/data/2.5/weather?q=delhi&appid=YOUR_API_KEY](https://api.openweathermap.org/data/2.5/weather?q=delhi&appid=YOUR_API_KEY)
