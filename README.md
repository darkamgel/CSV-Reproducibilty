# CSC 786 - Ethical and Reproducible Data Collection

## Project Overview

In this project, I demonstrate a reproducible workflow
for collecting weather data using Google Colab, Python,
WeatherAPI, and GitHub.

I focus on ethical transparency, secure authentication,
data provenance, documentation, and reproducibility.

## Tools

- Google Colab
- Python 3
- Git and GitHub
- WeatherAPI
- pandas
- requests

## Data Source

Provider: WeatherAPI
Documentation: https://www.weatherapi.com/docs/
Endpoint: https://api.weatherapi.com/v1/forecast.json
Location: Sioux Falls, South Dakota
Forecast duration: 1 day

## Repository Contents

- CSC786_Ethical_Reproducible_Data_Collection.ipynb
- README.md
- ETHICS.md
- DATA_README.md
- requirements.txt
- .gitignore

Generated CSVs and provenance metadata are stored locally
in the data/ directory.

## Instructions for Peer Reviewers

I have designed this project for independent reproduction.

### Step 1: Obtain the Notebook

Open my public GitHub repository and download the notebook.

You can open it in Google Colab using File > Upload notebook.

### Step 2: Prepare the Environment

1. Start a fresh Google Colab runtime.
2. Select Python 3.
3. Run the environment setup cells.
4. Verify that the required libraries are available.

### Step 3: Configure WeatherAPI

1. Visit https://www.weatherapi.com/
2. Create your own account.
3. Obtain your own API key.
4. Open Google Colab Secrets.
5. Create a secret named WEATHERAPI_KEY.
6. Paste your API key.
7. Enable notebook access.

Never place credentials directly inside notebook code.

### Step 4: Run the Experiment

Run the data collection and processing cells in order.

The notebook will:
1. Retrieve weather data.
2. Validate the API response.
3. Extract hourly forecasts.
4. Create a structured DataFrame.
5. Export a CSV file.
6. Generate provenance metadata.
7. Calculate and verify SHA-256 checksums.

### Step 5: Verify Reproducibility

Check that:
- The API request succeeds.
- The expected dataset columns are present.
- Dataset validation passes.
- The CSV is generated.
- The metadata JSON is generated.
- SHA-256 verification passes.

Live weather values may differ between executions.

## GitHub Authentication

The GitHub connection and publishing steps are part of
my development workflow.

Peer reviewers may skip publishing steps.

If a reviewer wants to reproduce the Git operations,
they should use their own repository and GITHUB_TOKEN.

## Ethical Considerations

I do not publish authentication credentials.

I document my data sources and collection methodology.

I follow the provider's applicable usage conditions.

## Limitations

Weather forecasts change over time.

API access may depend on account limits and availability.

Reproduction focuses on workflow correctness and
data integrity rather than identical weather values.

## References

WeatherAPI: https://www.weatherapi.com/docs/
Google Colab: https://colab.research.google.com/
Python: https://docs.python.org/3/
Git: https://git-scm.com/doc
