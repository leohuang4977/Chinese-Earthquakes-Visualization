# Chinese-Earthquakes-Visualization
![earthquake](https://github.com/user-attachments/assets/c6d573b5-7e5e-4720-b1ff-5b084e63c575)

Overview

This project focuses on analyzing earthquake data in China to explore patterns, trends, and risks associated with seismic activities. The project is part of a personal research initiative aimed at understanding earthquake dynamics and their implications for disaster management and preparedness. The data is sourced from the Wikipedia page "List of earthquakes in China" and includes preprocessing, analysis, and visualization to derive meaningful insights.


## Purpose

The primary goal of this project is to:
* Identify patterns in earthquake occurrence.
* Quantify the magnitude and impact of earthquakes (e.g., deaths, magnitude trends).
* Explore temporal and spatial trends in earthquake data.
* Develop visualizations to communicate findings effectively.

## Key Features

Data Scraping and Cleaning: Extract and preprocess earthquake data from Wikipedia.
Geospatial Analysis: Parse and plot earthquake locations on maps.
Time-Series Analysis: Examine earthquake trends over time.
Advanced Visualizations:
3D scatter plots of latitude, longitude, and magnitude.
Interactive maps using Plotly and animations.
Statistical visualizations with Matplotlib and Seaborn.

## Prerequisites

Python 3.7+

Libraries:
requests
beautifulsoup4
pandas
numpy
matplotlib
seaborn
plotly

Install dependencies via pip:

pip install requests beautifulsoup4 pandas numpy matplotlib seaborn plotly

## Data Preprocessing

Scraping: Data is fetched from the Wikipedia page using the requests and BeautifulSoup libraries.

Cleaning: Footnotes (e.g., [1]) are removed. Empty strings are replaced with NaN values. Columns with numeric data (e.g., magnitude, deaths) are converted to appropriate types.

Coordinate Parsing: Extracts and standardizes latitude and longitude from complex coordinate strings.

Year Extraction: Derives the Year column from the Date field.

Magnitude Normalization: Converts various magnitude scales (Ms, ML, Mw) into a unified MagMw scale using defined conversion factors.

## Analysis and Visualization

1. Descriptive Statistics

Overview of earthquake count, magnitude ranges, and death tolls.

2. Spatial Analysis

Earthquake locations are plotted on:

2D Maps: Overlay earthquake points on a map of China.
3D Scatter Plots: Latitude, longitude, and magnitude visualized in 3D space.

3. Temporal Trends

Yearly count of earthquakes using Seaborn line plots.
Average magnitude trends over time.

4. Interactive Visualizations

Animated Maps:
Temporal progression of earthquakes.
Markers sized by magnitude and colored by severity.

Interactive Geo Maps:
Hover features for detailed location and magnitude information.
## File Descriptions

earthquake_analysis_china.py: Python script containing all steps from data scraping to analysis and visualization.

earthquake_data_china.csv: Cleaned dataset saved after preprocessing.

Generated Plots:
Static and interactive visualizations saved in the output directory.

## How to Run the Script

Clone the repository:
git clone <repository_url>
cd <repository_directory>

Execute the script:
python earthquake_analysis_china.py

Explore outputs:
CSV files in the output directory.

Interactive visualizations in the browser.

License

This project is licensed under the MIT License.


