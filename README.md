# COVID-19 Data Analysis Notebook

## Introduction
This project focuses on analyzing COVID-19 data to explore confirmed cases, deaths, and their relationships with various socio-economic factors, including insights drawn from the Worldwide Happiness Report. The analysis aims to visualize the impact of the pandemic across different countries and understand correlations with happiness metrics.


## Project Structure

The project consists of the following components:

- **Data Folder**: Contains the raw data files needed for analysis:
  - `covid19_Confirmed_dataset.csv`: Dataset containing confirmed COVID-19 cases by country.
  - `covid19_deaths_dataset.csv`: Dataset containing COVID-19 death counts by country.
  - `worldwide_happiness_report.csv`: Dataset containing the happiness scores and related metrics for various countries.

- **Main Notebook**: A Jupyter notebook that includes all the steps of the analysis, from data loading to visualization.

## Libraries Used
This project utilizes the following libraries:
- `pandas`: For data manipulation and analysis.
- `numpy`: For numerical operations.
- `seaborn`: For enhanced data visualization.
- `matplotlib`: For creating static, animated, and interactive visualizations in Python.

## Data Loading and Preparation

### Covid-19 Confirmed Cases
1. **Loading**: The confirmed cases dataset is loaded from `covid19_Confirmed_dataset.csv`.
2. **Cleaning**:
   - Removed unnecessary columns (`Lat`, `Long`).
   - Aggregated the dataset by country.
   - Plotted trends for countries like China and Italy.

### Covid-19 Deaths
1. **Loading**: The deaths dataset is loaded from `covid19_deaths_dataset.csv`.
2. **Cleaning**:
   - Removed unnecessary columns.
   - Aggregated the dataset by country.

### Merging Datasets
- The confirmed cases and deaths datasets are merged based on country and date.

### Happiness Data
1. **Loading**: The Worldwide Happiness Report is imported from `worldwide_happiness_report.csv`.
2. **Cleaning**: Useless columns are dropped, and the data is indexed by country.
3. **Combining**: The COVID-19 data is joined with the happiness metrics to analyze correlations.

## Visualizations
- Plots showcasing confirmed COVID-19 cases and deaths over time for specific countries.
- Regression plots analyzing the relationships between happiness metrics (such as GDP, social support, and healthy life expectancy) and the maximum infection rate in various countries.

## Requirements
To run this project, ensure you have the following libraries installed:
- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn

You can install the required libraries using pip:
```bash
pip install pandas numpy matplotlib seaborn
