# Daily Weather Data Analysis

## Project Overview

This project aims to analyze and visualize daily weather data collected from various global locations. The analysis covers several key aspects including temperature trends, geographical distribution of weather metrics, air quality, wind patterns, precipitation, and more. The insights derived will help understand the global weather patterns and their implications on various environmental factors.

## Tools Used

- **Python**: The primary programming language used for data analysis.
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical computations.
- **Matplotlib**: For creating static plots and visualizations.
- **Seaborn**: For enhanced data visualization, especially statistical plots.
- **Plotly**: For interactive and geographical visualizations.

## Data Description

The dataset used for this analysis contains the following columns:

- **last_updated**: The timestamp when the weather data was last updated.
- **temperature_celsius**: Temperature in Celsius.
- **temperature_fahrenheit**: Temperature in Fahrenheit.
- **latitude**: Latitude of the location.
- **longitude**: Longitude of the location.
- **location_name**: Name of the location.
- **condition_text**: Description of the weather condition.
- **wind_mph**: Wind speed in miles per hour.
- **wind_kph**: Wind speed in kilometers per hour.
- **precip_mm**: Precipitation in millimeters.
- **precip_in**: Precipitation in inches.
- **humidity**: Humidity percentage.
- **visibility_km**: Visibility in kilometers.
- **visibility_miles**: Visibility in miles.
- **uv_index**: UV index.
- **wind_direction**: Direction of the wind.
- **sunrise**: Sunrise time.
- **sunset**: Sunset time.
- **moon_phase**: Phase of the moon.
- **air_quality_Carbon_Monoxide**: Air quality measurement for Carbon Monoxide.
- **air_quality_Ozone**: Air quality measurement for Ozone.
- **air_quality_Nitrogen_dioxide**: Air quality measurement for Nitrogen Dioxide.
- **air_quality_Sulphur_dioxide**: Air quality measurement for Sulphur Dioxide.
- **air_quality_PM2.5**: Air quality measurement for PM2.5 particles.
- **air_quality_PM10**: Air quality measurement for PM10 particles.
- **air_quality_us-epa-index**: US EPA air quality index.
- **air_quality_gb-defra-index**: UK DEFRA air quality index.
- **gust_mph**: Wind gust speed in miles per hour.
- **gust_kph**: Wind gust speed in kilometers per hour.

## Data Analysis and Visualization

### Data Cleaning and Initial Exploration

1. **Loading and Inspecting Data**:
   - Loaded the dataset using `pd.read_csv`.
   - Inspected the first few rows using `df.sample(5)`.
   - Displayed dataset information using `df.info()`.
   - Checked for missing values using `df.isnull().sum()`.
   - Displayed basic statistics using `df.describe()`.

2. **Duplicate Values Check**:
   - Checked for duplicate entries using `df.duplicated().sum()`.

### Temporal Analysis - Temperature Trends Over Time

1. **Temperature Trends**:
   - Converted `last_updated` to datetime format.
   - Calculated daily average temperatures in both Celsius and Fahrenheit.
   - Plotted the temperature trends over time using `matplotlib`.

### Geographical Analysis - Temperature Distribution Across Locations

1. **Temperature Distribution**:
   - Used `plotly.express` to create a geographical scatter plot showing temperature distribution across various locations.

### Weather Condition Analysis - Frequency of Different Weather Conditions

1. **Weather Condition Frequency**:
   - Standardized `condition_text` to lowercase for consistency.
   - Calculated the frequency of different weather conditions.
   - Visualized the frequency distribution using a bar plot.

### Air Quality Analysis - Correlation Between Air Quality Metrics

1. **Correlation Matrix**:
   - Computed the correlation matrix for various air quality metrics.
   - Visualized the correlation matrix using a heatmap with `seaborn`.

### Wind Analysis - Wind Speed Distribution

1. **Wind Speed Distribution**:
   - Created histograms to show the distribution of wind speed in both miles per hour and kilometers per hour.

### Precipitation Analysis - Daily Precipitation Trends

1. **Precipitation Trends**:
   - Calculated daily average precipitation in both millimeters and inches.
   - Plotted the daily precipitation trends using `matplotlib`.

### Humidity vs. Temperature Analysis

1. **Scatter Plot**:
   - Visualized the relationship between humidity and temperature using a scatter plot with `seaborn`.

### Visibility Analysis - Impact of Weather Conditions on Visibility

1. **Visibility Analysis**:
   - Calculated average visibility for different weather conditions.
   - Visualized the average visibility in both kilometers and miles using bar plots.

### UV Index Analysis - UV Index Distribution Across Locations

1. **Geographical Distribution**:
   - Created a geographical scatter plot to show UV index distribution across various locations using `plotly.express`.

### Wind Direction Analysis - Dominant Wind Directions

1. **Wind Direction Frequency**:
   - Calculated the frequency of different wind directions.
   - Visualized the dominant wind directions using a bar plot.

### Sunrise and Sunset Analysis - Daily Variation in Sunrise and Sunset Times

1. **Daylight Hours**:
   - Calculated daylight hours by subtracting sunrise time from sunset time.
   - Plotted the average daylight hours over time using `matplotlib`.

### Moon Phase Analysis - Distribution of Moon Phases

1. **Pie Chart**:
   - Visualized the distribution of moon phases using a pie chart.

### UV Index vs. Temperature Analysis

1. **Scatter Plot**:
   - Visualized the relationship between UV index and temperature using scatter plots.

### Air Quality Index Analysis - Distribution of Air Quality Indices

1. **Histogram**:
   - Created histograms to show the distribution of US EPA and UK DEFRA air quality indices.

### Visibility vs. Humidity Analysis

1. **Scatter Plot**:
   - Visualized the relationship between visibility and humidity using scatter plots.

### Gust Speed Analysis - Distribution of Wind Gust Speeds

1. **Histogram**:
   - Created histograms to show the distribution of wind gust speeds in both miles per hour and kilometers per hour.

### Daylight Distribution Across Locations

1. **Geographical Distribution**:
   - Created a geographical scatter plot to show daylight distribution across various locations using `plotly.express`.

## Conclusion

This comprehensive analysis provides valuable insights into global weather patterns and their various aspects such as temperature trends, geographical distribution, air quality, and more. The visualizations created help in better understanding and interpreting the data, making it easier to derive actionable insights for environmental monitoring and planning.

---
