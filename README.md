# Optimizing BIXI Bikeshare system for sustainable travel


# Abstract
The goal of the project is to analyse the current bikeshare system in Montreal and try and optimize the system to promote sustainable and healthy travel for the residents of Montreal. In order to do this we must understand how the system is being used and where the gaps are that may be filled. For example, is the system being used as a replacement for public transport lines or to access areas not well serviced by public transport? Are there areas where more stations could be beneficial to increase the number of users? Are there certain roads that are more bike friendly than others and therefore may encourage bikeshare usage in these areas? Theses questions will allow us to paint a picture of the current usage and where it can be improved. 

# Research questions
Research questions can be found in joined.ipynb or alternatively in Pipeline.ipynb

# Setup

Download pickled data here :
https://drive.google.com/open?id=1IZey_n6xR1WtFI03uY69HgJfeBz4_2Lv

# Datasets

BIXI bikeshare data - 
https://montreal.bixi.com/en/open-data
.csv format
Contains information on station location, ride duration, start and end points of rides (time and location), whether the user is a member
Data goes from 2014 to 2019. Each year has a folder of .csv files organized by month. Data is contained in the GitHub folder in "/BikiMontrealRentals"

Montreal public transport database - 
routes:
http://donnees.ville.montreal.qc.ca/dataset/stm-traces-des-lignes-de-bus-et-de-metro

This dataset is a shapefile. It contains the gps cordinates of sequences of points representing different traces. It can be converted to geoJSON which may be easier to treat.

timetable: (only current data)
http://donnees.ville.montreal.qc.ca/dataset/stm-horaires-planifies-et-trajets-des-bus-et-du-metro

Bike paths - http://donnees.ville.montreal.qc.ca/dataset/pistes-cyclables

Speed limits - http://donnees.ville.montreal.qc.ca/dataset/panneaux-de-signalisation (based on road signs)
 

# Notebook descriptions 
*Notebook to be graded is Joined.ipynb*

BikePaths - Visualisations of the bikepaths in Montreal

bixi_visual - exploratory analysis on a month of the 2019 data to experiment with different visualization methods (both statistics and folium maps)

BixiAnalysis - combines BIXI .csv data into a combined dataframe with additional elements (splits up dates, adds distance approximation of rides) initial analysis of bike share data and initial analysis of station use with visualization in folium
Additional requirements: install haversine library
Data: saved in Google drive as "combined_data", run notebook from "Load saved combined dataframe.." 

BusLines - Visualisations of the busline in Montreal

Pipeline - Contains only the planning for the project. 

Joined - Contains the important parts of the different notebooks.

Weather - Currently loads and cleans weather data of Montreal. In the future will have correlation with bike traffic.


# Questions for TAs
Is there an  easy way to get the density of paths from a geojson file without creating a custom algorithm ? 
