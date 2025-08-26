# Covid_19_Update_bot
A basic python project

This project fetches live COVID-19 updates for any country using the [disease.sh](https://disease.sh/) API.

How It Works
  1. Builds an API URL with the country name.
  2. Sends a request to fetch live COVID-19 data.
  3. Checks if the request was successful (`status 200`).
  4. Converts the response (JSON) into a Python dictionary.
  5. Extracts key details: total cases, today’s cases, deaths, recovered.
  6. Formats the data into a neat summary string.
     
- Output:
  A formatted text update, or an error message if data cannot be fetched.

Example use
print(covid_update("Japan"))

Example Output
 COVID-19 Update for Japan
 Total Cases: 33874629
 Today Cases: 0
 Deaths: 74896
 Recovered: 0

Summary
- Simple bot that gives COVID-19 stats for any country.
- Uses `requests` to fetch API data.
- Handles errors gracefully.
- Returns clean, human-readable results.
