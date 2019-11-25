# Optimizing BIXI Bikeshare system for sustainable travel

# Abstract
The goal of the project is to analyse the current bikeshare system in Montreal and try and optimize the system to promote sustainable and healthy travel for the residents of Montreal. In order to do this we must understand how the system is being used and where the gaps are that may be filled. For example, is the system being used as a replacement for public transport lines or to access areas not well serviced by public transport? Are there areas where more stations could be beneficial to increase the number of users? Are there certain roads that are more bike friendly than others and therefore may encourage bikeshare usage in these areas? Theses questions will allow us to paint a picture of the current usage and where it can be improved. 

# Research questions
We will address two main research questions, as well as answer a few smaller general questions to answer these questions:

Do the trips taken align with existing public transport lines or are they used to fill the gaps of the public transport routes?

Are there stations where bikes are underused and ones where more are required?

# Dataset

BIXI bikeshare data - 
https://montreal.bixi.com/en/open-data
.csv format
Contains information on station location, ride duration, start and end points of rides (time and location), whether the user is a member
Data goes from 2014 to 2019. Each year has a folder of .csv files organized by month. 
Station location dataset includes coordinates of stations.
It unfortunatly doesn't include data on the station's status at time of rental (i.e. how many bikes are available at the station, this could affect the number of people using each station)



Montreal public transport database - 
routes:
http://donnees.ville.montreal.qc.ca/dataset/stm-traces-des-lignes-de-bus-et-de-metro

This dataset is a shapefile. It contains the gps cordinates of sequences of points representing different traces. It can be converted to geoJSON which may be easier to treat.

timetable: (only current data)
http://donnees.ville.montreal.qc.ca/dataset/stm-horaires-planifies-et-trajets-des-bus-et-du-metro

Bike paths - http://donnees.ville.montreal.qc.ca/dataset/pistes-cyclables

The first step would be to combine all of the .csv files from the different years into a single database. 

# A list of internal milestones up until project milestone 2


# Questions for TAs
Add here some questions you have for us, in general or project-specific.
