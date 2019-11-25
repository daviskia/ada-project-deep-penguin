# Optimizing BIXI Bikeshare system for sustainable travel

# Abstract
A 150 word description of the project idea, goals, dataset used. What story you would like to tell and why? What's the motivation behind your project?

The goal of the project is to analyse the current bikeshare system in Montral and try and optimize the system to promote sustainable and healthy travel for the residents of Montreal. In order to do this we must understand how the system is being used and where the gaps are that may be filled. For example, is the system being used as a replacement for public transport lines or to access areas not well serviced by public transport. Are there areas where more stations could be beneficial to increase the number of users? Are there certain roads that are more bike friendly than others and therefore may encourage bikeshare usage in these areas? Theses questions will allow us to paint a picture of the current usage and where it can be improved. 

# Research questions
A list of research questions you would like to address during the project.

Do the trips taken align with existing public transport lines or are they used to fill the gaps of the public transport routes?

Are some areas of Montreal more bike-friendly than others (i.e. have bike lanes or are smaller roads) and is this bike friendliness correlated with more trips done in that area?

# Dataset
List the dataset(s) you want to use, and some ideas on how do you expect to get, manage, process and enrich it/them. Show us you've read the docs and some examples, and you've a clear idea on what to expect. Discuss data size and format if relevant.

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
Add here a sketch of your planning for the next project milestone.

For the 11/11 :

Extract the data of whether => Ariane

How to do arrow on the map of Montreal => Kiara

Get real time data (cap « city ») => Guillaume

Use fiona / pyproj / geopanda / folium to treat spatial data in order to do good representation with the map of Montreal => Quentin

For the 18/11 :

End the analysis, answer to questions

For the 25/11 : (milestone 2)
What could be added to/removed from this system to improve it, and what are the consequences we expect from our changes. Would it also improve significantly social good ?


# Questions for TAa
Add here some questions you have for us, in general or project-specific.
