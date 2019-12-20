# Optimizing BIXI Bikeshare system for sustainable travel


# Abstract
The goal of the project is to analyse the current bikeshare system in Montreal and try and optimize the system to promote sustainable and healthy travel for the residents of Montreal. In order to do this we must understand how the system is being used and where the gaps are that may be filled. For example, is the system being used as a replacement for public transport lines or to access areas not well serviced by public transport? Are there areas where more stations could be beneficial to increase the number of users? Are there certain roads that are more bike friendly than others and therefore may encourage bikeshare usage in these areas? What is the influence of the weather on the use of the bikeshare system ? Theses questions will allow us to paint a picture of the current usage and where it can be improved. 

# Research questions
1. Do the trips taken align with existing public transport lines or are they used to fill the gaps of the public transport routes?
2. Are some areas of Montreal more bike-friendly than others (i.e. have bike lanes or are smaller roads) and is this bike friendliness correlated with more trips done in that area?

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

Weather historic - https://climat.meteo.gc.ca/historical_data/search_historic_data_f.html
 

# Notebook descriptions 
*Notebook to be graded is dataStory.ipynb*


# Member Contribution :
Guillaume : Plotting maps mainly chloropeths, testing if stations are in a neighbourhood. Focused mainly on public infrastructure.

Quentin : Created the code to calculate the density of bicycle paths created the comparison maps between the chloropleth obtained and BIXI stations, metro stations, bus stations and the analysis of the average popularity of a BIXI trip given the surrounding bike path density

Ariane : Analysis of the weather dataset and comparison with the number of travel per day

