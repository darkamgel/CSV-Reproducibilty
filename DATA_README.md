# Dataset Documentation

## 1. Overview

I collected hourly weather forecast data for
Sioux Falls, South Dakota, using WeatherAPI.

Data Source: WeatherAPI
Endpoint: https://api.weatherapi.com/v1/forecast.json
HTTP Method: GET

## 2. Collection Information

Collection Timestamp (UTC): 2026-10-24T210736Z
Forecast Date: 2026-10-24

Location: Sioux Falls
Region: South Dakota
Country: United States of America

## 3. Dataset Summary

Generated CSV: weather_hourly_2026-10-24T210736Z.csv

Total Records: 24
Total Columns: 9

Missing Values: 0

## 4. Dataset Schema

| Column | Description |
|---|---|
| location | City |
| region | State or region |
| country | Country |
| forecast_time | Local forecast timestamp |
| temperature_c | Temperature in Celsius |
| humidity_percent | Relative humidity percentage |
| wind_kph | Wind speed in kilometers per hour |
| precipitation_mm | Forecast precipitation in millimeters |
| condition | Weather condition |

## 5. Data Integrity

I generated a SHA-256 checksum for my local CSV.

SHA-256: 6bb88b668f192cf2e6e8f4d661a8d2a1b3c8b17acdd63faecaa9390d301c1f49

The checksum verifies the identity of the local
file used in this execution.

Peer reviewers must calculate and verify their
own checksum after generating their own CSV.

## 6. Provenance

I recorded the following in the local metadata JSON:

- WeatherAPI endpoint
- Non-sensitive request parameters
- UTC collection timestamp
- Dataset filename
- Dataset dimensions
- Python and package versions
- SHA-256 checksum

## 7. Reproduction Instructions

1. Open the notebook in Google Colab.
2. Configure WEATHERAPI_KEY in Colab Secrets.
3. Execute the environment setup.
4. Retrieve weather data.
5. Convert the JSON response into a DataFrame.
6. Validate and export the CSV.
7. Generate provenance metadata.
8. Verify the SHA-256 checksum.

GitHub publishing is not required to verify the
data collection workflow.

## 8. Limitations

Forecast values may change across executions.

The SHA-256 checksum does not establish the
accuracy of the weather forecasts.

Generated forecast data is kept locally,
subject to WeatherAPI's applicable terms.

## 9. References

WeatherAPI:
https://www.weatherapi.com/docs/

WeatherAPI Terms:
https://www.weatherapi.com/terms

Python hashlib:
https://docs.python.org/3/library/hashlib.html
