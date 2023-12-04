# DSCI 510 Final Project

## Name of the Project

Is there a Relationship between Crime Rates in US Cities and State and Political Affiliation?

## Team Members (Name and Student IDs)

Echo Tang (6198213027)
Misha Khan (7474924431)

## Instructions to create a conda enviornment

1. Open up the 'Terminal' app and navigate to a folder of your choice, preferably one that is specifically for DSCI510. 

2. Type in `conda create --name [project name of choice]`

3. Activate the environment with `conda activate [project name of choice]`. 

4. Clone the project repository https://github.com/USC-DSCI-510/final-project-mkhan58.git

## Instructions on how to install the required libraries

Once the repository has been cloned, navigate to the final-project-mkhan58 folder. Run `pip install -r requirements.txt` to install the packages required for the project. If successful, you will see a successful installation statement in the terminal. 

Note: our project uses the `geoplot` package, which many users have noted may lead to installation issues on their computer. If `geoplot` is not able to install, please run `brew install geos` first, then run `pip install geoplot --no-cache-dir`. 

## Instructions on how to download the data

To download the data, navigate to the get_data.py file in the src folder and run this script. If successful, the data will be stored as HTML files in data/raw with the following file names: crime.html, election.html, as well as .txt files in data/raw with the following file names: crime_table.txt and election_table.txt. The HTML files contain website content from the URLs which data has been web scraped from, and the txt files contain the raw HTML tag content from the data of interest extracted from the respective URLs. 

## Instructions on how to clean the data

To clean the data, navigate to the clean_data.py file in the src folder and run this script. This file will clean the raw data into more readable CSV files, as well as perform data imputation of any missing values. If successful, the data will be stored as CSV files in the data/processed folder with the following file names: crime_data.csv, crime_and_election_data.csv, crime_election_geo_data.csv, and election_data.csv. 

## Instructions on how to run analysis code

To run the analysis code, navigate to the run_analysis.py file in the src folder and run this file. This file will generate descriptive statistics on crime rates in the top 100 most populous US cities by political affiliation taken from the election data and mapped to their respective states. T-tests were performed to determine if crime rates were statistically significantly different by political affiliation for the following crimes: murder/manslaughter, rape, robbery, assault, burglary, larceny/theft, vehicle theft, and arson. 

## Instructions on how to create visualizations

To create visualizations, please go to the visualize_results.py file in the src folder. This file contains all the code for our data visualizations. To see our visualizations, please go to the results folder and open visualizations_final_project.ipynb. 