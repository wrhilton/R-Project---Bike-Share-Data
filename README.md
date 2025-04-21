Project provided in the Udacity Data Analytics Nanodegree. Work is my own.

# Project: Exploring US Bikeshare Data

## Overview

This project performs an exploratory data analysis on bikeshare usage data from three major US cities: Chicago, New York City, and Washington. The goal is to uncover patterns in usage by calculating descriptive statistics and identifying trends related to time, popular stations, trip durations, and user demographics.

The analysis is interactive, prompting the user to choose a city and apply filters for month and day of the week to explore the data dynamically.

## Data Source

The data used in this analysis covers bike share usage for the first six months of 2017 for the following cities:

* Chicago (Divvy)
* New York City (Citi Bike)
* Washington (Capital Bikeshare)

Data is provided by Motivate International Inc. and made available through Udacity. The datasets include information such as trip start/end times, stations, duration, user types, and demographic details (where available).

## Methodology

The analysis follows these key steps within the script/notebook:

1.  **Data Loading:** Loading datasets for Chicago, New York City, and Washington using Pandas.
2.  **User Input:** Gathering user preferences for:
    * City of interest.
    * Time filters (specific month, specific day of the week, or no filter).
3.  **Data Filtering:** Applying the selected month and day filters to the chosen city's dataset.
4.  **Descriptive Statistics Calculation:** Computing various statistics based on the filtered data, including:
    * Most frequent month of travel.
    * Most frequent day of the week.
    * Most frequent start hour.
    * Most popular start station.
    * Most popular end station.
    * Most frequent combination of start and end stations.
    * Total travel time.
    * Average travel time.
    * Counts of different user types (e.g., Subscriber, Customer).
    * Counts of gender (for NYC and Chicago).
    * Earliest, most recent, and most common year of birth (for NYC and Chicago).
5.  **Results Display:** Printing the calculated statistics clearly to the console.
6.  **Raw Data Display:** Offering an option to display chunks of the raw filtered data upon user request.

## Key Findings (Examples derived from analysis)

The analysis reveals insights such as:

* Peak usage times (common months, days, hours).
* Most frequented start and end locations, highlighting popular routes.
* Average trip durations.
* Breakdown of user types (e.g., subscribers vs casual riders).
* Basic demographic patterns where data is available (gender, age distribution).

*(Refer to the code and outputs in the `Explore_bikeshare_data.html` file or the original `.ipynb` notebook for specific statistical results based on different filter selections.)*

## Technologies & Libraries Used

* Python 3
* Pandas (for data manipulation and analysis)
* NumPy (for numerical operations)
* time (for calculating durations)
* Jupyter Notebook (as the development environment)

## How to Run

1.  **Prerequisites:** Ensure you have Python 3 installed along with the Pandas and NumPy libraries.
    ```bash
    pip install pandas numpy
    ```
2.  **Get the Code:** Download the original Jupyter Notebook (`.ipynb` file - **recommended to add this to the repo!**) associated with the `Explore_bikeshare_data.html` file.
3.  **Get the Data:** Download the corresponding city bikeshare `.csv` files (e.g., `chicago.csv`, `new_york_city.csv`, `washington.csv`) and place them in the same directory as the notebook/script.
4.  **Execute:** Run the Python script or the Jupyter Notebook. The script will prompt you for city and filter choices to perform the analysis.

## File Structure

* `Explore_bikeshare_data.ipynb` (Recommended): The original Jupyter Notebook containing the Python code and analysis steps.
* `Explore_bikeshare_data.html`: An HTML export of the notebook, viewable in a web browser.
* `chicago.csv`, `new_york_city.csv`, `washington.csv` (Data files - not included in this repo, must be obtained separately).
* `README.md`: This file.
