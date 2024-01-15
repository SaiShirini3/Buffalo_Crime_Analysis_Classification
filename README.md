# Buffalo_Crime_Analysis_Classification
This repository contains a Python script for analyzing Buffalo crime data. The analysis includes data parsing, normalization, SQL querying, data visualization, and machine learning classification using a Decision Tree.

# Motivation
The primary motivation for this project is to understand different types of incidents in Buffalo and provide insights for effective planning by law enforcement agencies.

# Files and Directories
 BuffaloCrimeAnalysis.py: Python script containing the analysis code.
Crime_Incidents.csv: Input CSV file containing crime incident data. (https://data.buffalony.gov/Public-Safety/Crime-Incidents/d6g9-xbgu/about_data)
normalized.db: SQLite database file for storing normalized data.

# Usage
Ensure you have Python installed on your machine.
Install required dependencies using: pip install pandas sqlite3 plotly scikit-learn matplotlib seaborn.
Run the Python script: python BuffaloCrimeAnalysis.py.

# Data Source
The crime incident data is sourced from the file Crime_Incidents.csv. Ensure that this file is present in the repository.
# Dataset Overview

The dataset comprises crime incidents in the City of Buffalo, with 34 features and 300,000 data points. The information is collected until December 13th, 2023, offering a preliminary look at crime reports in Buffalo.

# Database Structure

The dataset has been split into five tables to store different types of information related to incidents and census data: INCIDENT INFO TABLE, CENSUS INFO 2010 TABLE, CENSUS_INFO TABLE, GEOID INFO TABLE, CASE INFO TABLE.

# Data preprocessing

Data from the INCIDENT_INFO TABLE was utilized. Longitude and Latitude were converted to String data types. Label encoding was applied to categorical columns. Unnecessary columns (CITY, STATE, INCIDENT_DATETIME) were removed. Feature selection was performed using a heatmap. Additional columns (LATITUDE, LONGITUDE) were removed based on the heatmap.
# Results
The analysis provides insights into yearly crime trends, incident type distribution, day-of-week analysis, and more. Machine learning classification is performed using a Decision Tree.
