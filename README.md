# SparkifyDb   

#### Purpose
The ETL project is designed and implemented to help a hypothetical company Sparkify to perform analysis on users' song play activity using our new music app event data.

#### Database design and ETL pipeline

The data is ingested from source folders _event_data_ in form of csv files using pandas library in Python. Data is further filtered, cleaned and recorde using Cassandra CQL and Python statements and commands. The tables are created to answer below questions.

#### Example of some analysis query:

 1. Give me the artist, song title and song's length in the music app history that was heard during  sessionId = 338, and itemInSession  = 4
 2. Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182
 3. Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'

#### How to use the product?
1. Run etl.ipynb in jupyter notebook to clean the source data and create database/tables.

### REMEMBER: Make sure to `close` connection to sparkifydb
Remember to close the connection to sparkify database after use since multiple connections to the same database are not allowed. 
