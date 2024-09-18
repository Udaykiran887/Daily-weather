---

# Daily Weather Dashboard Using Node-RED and WeatherAPI

## Project Overview

This project demonstrates how to create a **Daily Weather Dashboard** using [Node-RED](https://nodered.org/) and [WeatherAPI](https://www.weatherapi.com/). The dashboard fetches real-time weather data for a user-selected city and displays current temperature, weather condition, wind speed, and humidity. The data updates automatically every 24 hours, ensuring users have up-to-date weather information.

The dashboard is created using **Node-RED Dashboard nodes** for UI, and it connects to the WeatherAPI to fetch live weather data.

---

## Installation Instructions

### Prerequisites

1. **Node.js**: Download and install from [Node.js official website](https://nodejs.org/).
2. **Node-RED**: Install Node-RED following the [official guide](https://nodered.org/docs/getting-started/).
3. **WeatherAPI Key**: Sign up for a free API key at [WeatherAPI](https://www.weatherapi.com/signup.aspx).
4. **Node-RED Dashboard Nodes**: Required for UI. Install them by running the following command in your Node-RED user directory:
   ```bash
   npm install node-red-dashboard
   ```

### Step-by-Step Installation

1. **Clone the Repository** (if you have the code in GitHub):
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Install Node-RED (if not already installed)**:
   ```bash
   npm install -g node-red
   ```

3. **Start Node-RED**:
   ```bash
   node-red
   ```

4. **Install Node-RED Dashboard**:
   Inside the Node-RED directory, run:
   ```bash
   npm install node-red-dashboard
   ```

5. **Get your WeatherAPI Key**:
   - Go to [WeatherAPI](https://www.weatherapi.com/signup.aspx) and sign up for a free API key.
   - Note down the API key for use in the flow.

6. **Configure the WeatherAPI Request URL**:
   - In Node-RED, add the WeatherAPI request URL in the **HTTP Request Node**.
   - Use this URL format:
     ```
     https://api.weatherapi.com/v1/current.json?key=<YOUR_API_KEY>&q=<CITY>&aqi=yes
     ```
   - Replace `<YOUR_API_KEY>` with your WeatherAPI key and `<CITY>` with the city you want to get the weather for.

7. **Deploy the Flow**:
   - Open the Node-RED editor at `http://localhost:1880/`.
   - Import the flow provided in the project and deploy it.

---

## Usage

### How to Use the Project

Once the flow is deployed, the dashboard will automatically fetch and display weather data every 24 hours. Follow the steps below to use the weather dashboard:

1. **Open the Node-RED Dashboard**:
   - Navigate to `http://localhost:1880/ui/` in your browser to access the weather dashboard.

2. **View Weather Data**:
   - The dashboard will display real-time weather data, including:
     - **City**: The name of the city.
     - **Temperature**: Current temperature in Celsius or Fahrenheit.
     - **Weather Condition**: A brief description of the weather (e.g., sunny, rainy).
     - **Humidity**: Percentage humidity in the air.
     - **Wind Speed**: Wind speed in meters per second (m/s).

### Example Usage

- For example, if you want to fetch weather data for **New York**, the API URL would look like this:
  ```
  https://api.weatherapi.com/v1/current.json?key=<YOUR_API_KEY>&q=New York&aqi=yes
  ```
- The dashboard will display New York's temperature, weather conditions, humidity, and wind speed.

---

## Contributing

We welcome contributions to enhance the project!

### How to Contribute:

1. **Fork the repository**.
2. **Create a new branch** for your feature or bugfix.
   ```bash
   git checkout -b feature/new-feature
   ```
3. **Commit your changes**.
   ```bash
   git commit -m "Add new feature"
   ```
4. **Push to the branch**.
   ```bash
   git push origin feature/new-feature
   ```
5. **Open a pull request** to the `main` branch.

Please follow the [Code of Conduct](CODE_OF_CONDUCT.md) when contributing.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contact Information

If you have any questions or issues, feel free to reach out!

- **Project Owner**: uday kiran 
- **Email**: [GMAIL](udaykirankothagattu@gmail.com)
- **GitHub**: [udaykiran887](https://github.com/Udaykiran887)

---
