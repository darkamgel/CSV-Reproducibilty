# Dataset Documentation

## Data Source

I use WeatherAPI to retrieve hourly weather forecasts
for Sioux Falls, South Dakota.

API Documentation:
https://www.weatherapi.com/docs/

## Collection Method

I use a Python HTTP GET request to retrieve JSON data.

I process the response using pandas and export
hourly forecast records into a CSV file.

## Expected Dataset Columns

| Column | Description |
|---|---|
| location | City |
| region | State or region |
| country | Country |
| forecast_time | Local forecast timestamp |
| temperature_c | Temperature in Celsius |
| humidity_percent | Relative humidity percentage |
| wind_kph | Wind speed in kilometers per hour |
| precipitation_mm | Precipitation in millimeters |
| condition | Text description of weather conditions |

## Data Validation

I will check:
- Required columns
- Missing values
- Valid timestamps
- Duplicate timestamps
- Numeric fields
- Valid humidity range
- Non-negative wind and precipitation

## Provenance

After collection, I will record:
- API endpoint
- Non-sensitive request parameters
- UTC collection timestamp
- Dataset filename
- Dataset dimensions
- Software versions
- SHA-256 checksum

## Reproducibility

A peer reviewer can run the notebook using their
own WeatherAPI credentials.

Live weather forecasts may differ between executions.

## Data Availability

Generated data is stored in the local Colab
data/ directory.

Public redistribution depends on the applicable
WeatherAPI usage terms.

## References

WeatherAPI:
https://www.weatherapi.com/docs/

pandas:
https://pandas.pydata.org/docs/
