# Sqlalchemy-challenge

## Climate Analysis and Flask API with SQLAlchemy

## Overview

This project is part of the Bootcamp Module 10 Challenge, where I performed a climate analysis and designed a Flask API based on the provided dataset. The analysis involves using Python, SQLAlchemy ORM queries, Pandas, and Matplotlib to explore climate data. Additionally, a Flask API is designed to serve the analyzed data through various routes.

## Table of Contents

* Project Structure
* Setup and Execution
* SQLAlchemy Connection
* Precipitation Analysis
* Station Analysis
* Flask API Routes
* Closing
* Code Source
* License
* References
* Author

## Project Structure

The project repository is organized as follows:

* SurfsUp/: Directory for the Challenge, containing the main scripts and data files.
    * climate_analysis.ipynb: Jupyter notebook for climate analysis.
    * app.py: Flask application for the API.
    * Resources/: Folder containing the dataset (hawaii.sqlite), hawaii_measurements.csv hawaii_stations.csv.

## Setup and Execution

1.Clone this repository to your local machine:

    git clone https://github.com/AnyasorG/sqlalchemy_challenge.git
    cd sqlalchemy_challenge/SurfsUp

2.Install the required dependencies (ensure you have Python and pip installed):

    pip install -r requirements.txt

3.Run the Jupyter notebook (climate_starter.ipynb) to perform the climate analysis.

4.Run the Flask API (app.py) to start the web server:

    python app.py
Access the API through http://127.0.0.1:5000/ in your web browser.

## SQLAlchemy Connection

* Used create_engine() to connect to the SQLite database.
* Employed automap_base() to reflect tables into classes (station and measurement).
* Created a session to link Python to the database.

## Precipitation Analysis

* Identified the most recent date in the dataset.
* Queried the previous 12 months of precipitation data.
* Loaded and visualized data using Pandas and Matplotlib.
* Printed summary statistics for the precipitation data.

## Station Analysis

* Calculated the total number of stations.
* Found the most active station.
* Computed lowest, highest, and average temperatures for the most active station.
* Obtained the previous 12 months of TOBS data for the most active station.
* Plotted a histogram of TOBS.

## Flask API Routes

* /: Homepage with available routes.
* /api/v1.0/precipitation: Precipitation data for the last 12 months.
* /api/v1.0/stations: List of all stations.
* /api/v1.0/tobs: TOBS data for the most active station in the last year.
* /api/v1.0/<start>: Min, avg, and max temperatures from a specified start date to the end.
* /api/v1.0/<start>/<end>: Min, avg, and max temperatures for a specified date range.
  
## Closing

Ensure to close your Jupyter notebook and Flask API session when done.

## Code Source

The code source can be found here: GitHub Repository

## License

This project is open-source and is made available under the terms of the MIT License. The MIT License is a permissive open-source license that allows you to use, modify, and distribute this software for your purposes. For the full details of the MIT License, please refer to MIT License.

## References

* Menne, M.J., I. Durre, R.S. Vose, B.E. Gleason, and T.G. Houston, 2012: An overview of the Global Historical Climatology Network-Daily Database. Journal of Atmospheric and Oceanic Technology, 29, 897-910, Reference Link.
* SQLAlchemy documentation (2023). SQLAlchemy Documentation. Retrieved on December 26, 2023.
* Python documentation (2023). Python Documentation. Retrieved on December 22, 2023.
* Pandas documentation (2023). https://pandas.pydata.org/docs/.Retrieved on December 22, 2023.
* Matplotlib documentation (2023). https://matplotlib.org/stable/index.html.Retrieved on December 22, 2023.

## Author

* Godswill Anyasor
* Data is located at GitHub Repository
