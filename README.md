# Optimizing BIXI Bikeshare system for sustainable travel

# Abstract
A 150 word description of the project idea, goals, dataset used. What story you would like to tell and why? What's the motivation behind your project?

The goal of the project is to analyse the current bikeshare system in Montral and try and optimize the system to promote sustainable and healthy travel for the residents of Montreal. In order to do this we must understand how the system is being used and where the gaps are that may be filled. For example, is the system being used as a replacement for public transport lines or to access areas not well serviced by public transport. Are there areas where more stations could be beneficial to increase the number of users? Are there certain roads that are more bike friendly than others and therefore may encourage bikeshare usage in these areas? Theses questions will allow us to paint a picture of the current usage and where it can be improved. 

# Research questions
A list of research questions you would like to address during the project. 

How has the use of the bikes evolved over time (increased use or decreased)?

At what time of day are the bikes mostly used and what stations are these between?

Do the trips taken allign with existing public transport lines or are they used to fill the gaps of the public transport routes?

Are there stations where bikes are underused and ones where more are required?

Are some areas of Montreal more bike friendly than others (i.e. have bike lanes or are smaller roads)?

Are most users members?

Do people rent for short periods (single trip) or longer periods (throughout the day)?

Is it mostly used as a commuting service or for more leisurly trips (a long duration between 2 close by stations could indicate leisure whereas a short duration between further stations would indicate commuting)?





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

timetable: (only current data)
http://donnees.ville.montreal.qc.ca/dataset/stm-horaires-planifies-et-trajets-des-bus-et-du-metro

Bike paths - http://donnees.ville.montreal.qc.ca/dataset/pistes-cyclables

The first step would be to combine all of the .csv files from the different years into a single database. 

# A list of internal milestones up until project milestone 2
Add here a sketch of your planning for the next project milestone.

# Questions for TAa
Add here some questions you have for us, in general or project-specific.