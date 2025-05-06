# COVID-19_DATA_TRACKER
# COVID-19 Global Data Tracker

This project analyzes global COVID-19 trends, including cases, deaths, vaccination progress, and hospitalization metrics. It utilizes data from the "Our World in Data" COVID-19 dataset and provides an interactive analysis dashboard with various visualizations and summary reports.

## Table of Contents

- [Overview](#overview)
- [Data Collection & Loading](#data-collection--loading)
- [Data Cleaning & Processing](#data-cleaning--processing)
- [Interactive Dashboard](#interactive-dashboard)
- [Visualization Functions](#visualization-functions)
- [Report Generation](#report-generation)
- [Global Map Visualization](#global-map-visualization)
- [Technologies Used](#technologies-used)
- [Usage](#usage)
- [Contributing](#contributing)

## Overview

The COVID-19 Global Data Tracker is a Python-based notebook that provides an interactive and comprehensive way to analyze and visualize global COVID-19 data. The system offers the ability to:
- Track global trends in COVID-19 cases, deaths, and vaccinations.
- Compare countries based on key metrics.
- View global visualizations like heatmaps.
- Filter and analyze data based on selected time periods and countries.

## Data Collection & Loading

The dataset is loaded directly from a raw GitHub URL containing the "Our World in Data" COVID-19 dataset. It includes information on:
- Total cases and deaths
- Vaccination data
- ICU patients and hospitalizations

The dataset is loaded, cleaned, and preprocessed to handle missing values and calculate derived metrics like death rate, vaccination rate, and hospitalization rates.

## Data Cleaning & Processing

The system offers a custom `clean_covid_data()` function that filters the dataset based on selected countries and date ranges. It also fills in missing values for key metrics (e.g., total cases, deaths, vaccinations) and computes derived metrics such as:
- Death rate
- Vaccination rate
- Hospitalization rate

## Interactive Dashboard

An interactive dashboard allows users to:
- Select countries for analysis.
- Choose date ranges for data analysis.
- Select key metrics such as cases, deaths, vaccinations, and hospitalizations.

This is done through the use of `ipywidgets` to provide a user-friendly interface for filtering and selecting the data to be analyzed.

## Visualization Functions

The notebook includes multiple visualization functions:
- Line charts for tracking total cases, deaths, and vaccinations over time.
- 7-day moving averages for daily cases and deaths.
- Bar charts comparing countries' metrics like death rates and vaccination rates.
- Custom visualizations for hospitalization metrics (ICU and hospital patients).

## Report Generation

The system generates a summary report, which includes:
- Summary of total cases, deaths, vaccinations, and hospitalizations.
- Comparative analysis of countries based on selected metrics.
- Output tables showing country-level summaries for cases, deaths, and vaccinations.

## Global Map Visualization

A global map is generated to show the number of COVID-19 cases per million people for each country. This visualization is created using Plotly and displayed as a choropleth map.

## Technologies Used

- **Python**: Core programming language
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical operations
- **Matplotlib & Seaborn**: Data visualization
- **Plotly**: Interactive visualizations (e.g., choropleth maps)
- **ipywidgets**: Interactive widgets for user interface
- **Jupyter Notebook**: Development environment

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/CharlesKJunior/covid-19-global-tracker.git
Install the required dependencies:

pip install -r requirements.txt
Open the Jupyter notebook and run the cells to analyze COVID-19 data:

jupyter notebook covid_19_analysis.ipynb

Contributing
If you would like to contribute to this project, feel free to submit a pull request. Please ensure your code follows the existing style and includes relevant tests.
