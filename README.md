# Weather Station

This is a weather station project by Open Green Energy, using ESPHome and an ESP32 board. It is designed to collect various meteorological data such as temperature, humidity, atmospheric pressure, rainfall, and wind speed, and wirelessly report this information to a Home Assistant server for monitoring and further analysis. The Open Green Energy Solar Powered WiFi Weather Station V4.0 originally came with Arduino code, but I have adapted it to work with Home Assistant via ESPHome.

**Original Project Links:**
- [Instructables Project Page](https://www.instructables.com/Solar-Powered-WiFi-Weather-Station-V40/)
- [Hackaday Project Page](https://hackaday.io/project/187061-solar-powered-wifi-weather-station-v40)

## Features

- **SparkFun Arduino IoT Weather Station**
  - **Rainfall Detection**: Rain gauge implemented with a tipping bucket sensor connected to a pulse counter.
  - **Wind Speed Monitoring**: Anemometer sensor output processed via a pulse counter.
  - **Wind Direction**: Detected by a wind vane.
- **Temperature Sensing**: BME280 and Dallas sensors.
- **Humidity Sensing**: BME280 sensor.
- **Atmospheric Pressure Measurement**: BME280 sensor.
- **Battery Monitoring**: Voltage monitoring to estimate remaining battery life.
- **Wireless Connectivity**: Wi-Fi to connect to local network and Home Assistant. (Haven't adopted LORA yet).
- **Over-The-Air (OTA) Updates**: Updates via ESPHome.
- **Deep Sleep Capabilities**: To conserve power, the ESP32 enters deep sleep mode.

## Hardware Components

- [PCBWay for a Solar Powered WiFi Weather Station V4.0](https://www.pcbway.com/project/shareproject/https_www_instructables_com_Solar_Powered_WiFi_Weather_Station_V40_515ff597.html)
- ESP32 development board
- BME280 sensor module (temperature, humidity, and pressure)
- Dallas temperature sensor
- Rain gauge sensor
- Anemometer
- Wind vane
- Battery for power supply
- Solar Panel

## Deep Sleep Configuration

The ESP32 is configured to enter deep sleep mode to save battery. You can adjust the sleep duration and conditions directly in the ESPHome configuration file.

## Contributions

Contributions to this project are welcome. Please fork the repository and submit a pull request with your suggested changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

<img src="https://github.com/teamsuperpanda/Weather-Station/assets/60556240/12e95408-0101-4e61-bb9c-39b2de19d0dd" width="300" alt="Weather Station Image 1">
<img src="https://github.com/teamsuperpanda/Weather-Station/assets/60556240/a581f776-bab5-4f58-9afc-af63b46e84f8" width="300" alt="Weather Station Image 2">
<img src="https://github.com/teamsuperpanda/Weather-Station/assets/60556240/18f87ddd-6480-490a-84f6-73d5c52dc065" width="300" alt="Weather Station Image 3">

