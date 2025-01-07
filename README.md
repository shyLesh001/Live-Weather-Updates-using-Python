# Live-Weather-Updates-using-Python# Weather Scraper

This project is a Python-based weather scraper that fetches current weather information for a specified city using Google Search. It uses the `requests` library for sending HTTP requests and `BeautifulSoup` for parsing HTML content.

---

## Features

- Fetches real-time weather data for any city.
- Displays:
  - **Location**
  - **Time**
  - **Weather Condition**
  - **Temperature (°C)**

---

## Prerequisites

Ensure you have the following installed:

1. **Python 3.6 or higher**: [Download Python](https://www.python.org/downloads/)
2. **Required Libraries**:
   - `BeautifulSoup` from `bs4`
   - `requests`

You can install the required libraries using:
```bash
pip install requests beautifulsoup4
```

---

## How to Use

1. Clone the repository or download the script:
   ```bash
   git clone <repository-link>
   ```

2. Navigate to the project directory:
   ```bash
   cd weather-scraper
   ```

3. Run the script:
   ```bash
   python weather_scraper.py
   ```

4. Enter the name of the city when prompted:
   ```
   Enter the Name of Any City >> Mumbai
   ```

5. View the weather information in the output:
   ```
   Searching......

   Location: Mumbai, Maharashtra
   Time: Thursday, 3:00 PM
   Condition: Partly Cloudy
   Temperature: 30°C
   ```

---

## Code Overview

The script follows these steps:

1. Takes city name input from the user.
2. Replaces spaces with `+` for URL compatibility.
3. Sends a GET request to Google Search with the query `<city> weather`.
4. Parses the HTML response to extract weather details using CSS selectors.
5. Displays the extracted data.

---

## Example Output

```
Enter the Name of Any City >> London
Searching......

Location: London, United Kingdom
Time: Thursday, 2:00 PM
Condition: Rainy
Temperature: 15°C
```

---

## Potential Issues

- **Google's page structure changes**: The CSS selectors used for scraping (`#wob_loc`, `#wob_dts`, etc.) might become outdated if Google updates their page structure.
- **Blocked requests**: Automated scraping can trigger CAPTCHA or block requests.
- **Solution**: Consider using weather APIs like OpenWeatherMap for a more stable and reliable experience.

---


## Author

**Shailesh Pillai**  
[GitHub Profile](https://github.com/shyLesh001)  

