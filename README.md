# Buffalo Crime Analysis Classification

This repository contains a Python script for analyzing Buffalo crime data. The analysis includes data parsing, normalization, SQL querying, data visualization, and machine learning classification using a Decision Tree.

## Motivation

The primary motivation for this project is to understand the different types of crime incidents in Buffalo and provide insights that can aid law enforcement agencies in effective planning and decision-making.

## Files and Directories

- **BuffaloCrimeAnalysis.py:** Python script containing the analysis code.
- **Crime_Incidents.csv:** Input CSV file containing crime incident data. [Crime Incidents Data Source](https://data.buffalony.gov/Public-Safety/Crime-Incidents/d6g9-xbgu/about_data)
- **normalized.db:** SQLite database file for storing normalized data.

## Usage

1. **Ensure Python is installed:** Make sure Python is installed on your machine.
2. **Install dependencies:**
   ```bash
   pip install pandas sqlite3 plotly scikit-learn matplotlib seaborn
3. **Run the Python Script**
   ```bash
   python BuffaloCrimeAnalysis.py

 ## Data Source

The crime incident data is sourced from the file `Crime_Incidents.csv`. Ensure that this file is present in the repository before running the script.

## Dataset Overview

The dataset comprises crime incidents in the City of Buffalo, containing 34 features and 300,000 data points. The data is collected up until December 13th, 2023, providing a comprehensive view of crime reports in Buffalo.

## Database Structure

The dataset is split into five tables within the SQLite database to store various types of information related to incidents and census data:

- **INCIDENT INFO TABLE**
- **CENSUS INFO 2010 TABLE**
- **CENSUS_INFO TABLE**
- **GEOID INFO TABLE**
- **CASE INFO TABLE**

## Data Preprocessing

- **Incident Info Table:** Data from the INCIDENT_INFO TABLE was utilized.
- **Data Types:** Longitude and Latitude were converted to string data types.
- **Label Encoding:** Applied to categorical columns.
- **Column Removal:** Unnecessary columns (CITY, STATE, INCIDENT_DATETIME) were removed.
- **Feature Selection:** Performed using a heatmap, resulting in the removal of additional columns (LATITUDE, LONGITUDE).

## Results

The analysis provides insights into yearly crime trends, the distribution of incident types, day-of-week analysis, and more. Machine learning classification is performed using a Decision Tree to further analyze the data.

## Access the Application

Open a web browser and go to `http://localhost:5000` to interact with the app.

## Using the Web Application

- **Prediction:** Navigate to the main page, fill out the form with listing details (e.g., neighborhood, room type, minimum nights), and submit to get the predicted price.
- **Visualization:** Use the tools provided to generate visualizations and explore data patterns and correlations.
