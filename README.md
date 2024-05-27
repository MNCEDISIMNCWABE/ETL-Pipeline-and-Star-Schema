# Description
In this repository I explore the use of the ETL pipeline techniques to created a songs database for a music app. The database will to help the music app address business questions regarding its users, including the types of songs they listen to and the artists of those songs, using the available log and songs data. The database ensures a consistent and reliable storage solution for this data. This centralized data source is valuable in achieving its analytical objectives, such as identifying the most popular songs.

# Database Design and ETL Pipeline
For the schema design, the STAR schema is used as it simplifies queries and provides fast data aggregations and reporting.

### For this I use song data and log data, both in JSON format:
- Song data includes information about songs and artists, which is extracted and loaded into the users and artists dimension tables.

- Log data provides details about each user session. From this log data, information is extracted and loaded into the users dimension tables, as well as the songplays fact table.
