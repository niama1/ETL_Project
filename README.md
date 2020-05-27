# ETL
ETL Project Report

Extract: 

The original data sources we used were all csv files and came from various places. The NBA player profile data and statistical data came from Kaggle.com which we will merge with lat and lng information.
The Player Profile LAt and Lng came InkPlant.com, and the NBA team LAt and Lng cam from WikiPedia. of which was copied and pasted in to excel and saved as a csv file which were than reformated in VSCode and save for use in Python.
-Transform: 
After importing Player datadsets we renamed and selected only columns we wanted to use(Player , birth_state, position) and seprated specific columns later merges ((height cm, weight lbs)and (College)). 
were merged the two player profile  dataset into one dataframe and then again with Uunited States Latitude Longitude dataset on States. 
 removed any duplicate players or non US born players.
Next we imported team Latitude and Longitude and merge with Player stats base on the players Team.
Once agian selected and renamed only the columns we wanted to use.
As well the time frame of 2010 - 2015.
than we merge the player stat with player profile on Player
that gave of a clean list of NBA PLayer with Complete stats of interest for 2010- 2015
now we'll merger the player college with there names so no to exluced player who did not attend college. our nba player dadta set is complete and clean

 the PLayer State of birthe for tCleaning of the data was required to drop null values and to reformat the data into the database configuration that we wanted. Pandas was used within a jupyter notebook. We  wanted to use the NBA player stats from 2010-2015 only to use just data from a certain time period. Also the data set was cleaned to only include players born in the United States. Not all NBA players went to college so the dataframes were adjusted to account for that. We also wanted the latitude and longitude data for the birth states of the players in order to map it on google heatmaps. 

-Load: Databases were cleaned and formatted in pandas then transferred to SQL tables using an engine connection using SQLAlchemy.  Along the way we were reminded by multi errors that lower casign is best for pandas unles you Define the your tables with qutations 
(ex. Nba = bad  ,  nba= good or "Nba"=good ) . with that problem solved uploading and our data frame to our SQL NBA DataBAse was complete.
