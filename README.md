# Description
In this repository, I explore the use of an ETL pipeline using a STAR schema data design method to create a songs database for a music app. The database will help the music app address business questions regarding its users, including the types of songs they listen to and the artists of those songs, using the available log and song data. The database ensures a consistent and reliable storage solution for this data. This centralized data source is valuable in achieving its analytical objectives, such as identifying the most popular songs.

# Database Design and ETL Pipeline
For the schema design, the STAR schema is used as it simplifies queries and provides fast data aggregations and reporting.

![image](https://github.com/MNCEDISIMNCWABE/Songs-Data-Modelling/assets/67195600/391a5799-0ed9-491b-8b8b-40f580944ac6)

#### Tech Stack
- Python for building designing an ETL pipeline
- Google BiqQuery for schema design and data storage

#### Data Available in JSON format:
- Song data: Includes information about songs and artists, which is extracted and loaded into the users and artists dimension tables.
- Log data: Provides details about each user session. From this log data, information is extracted and loaded into the users dimension tables, as well as the songplays fact table.

### Star Schema Design:
The star schema is a type of database schema that is optimized for data warehousing and business intelligence applications. It consists of a central fact table surrounded by dimension tables. In our case, the fact table is the songplays table, and the dimension tables are users, songs, and artists.

#### Some Advantages of a Star Schema:
- Simplified Queries: The star schema design simplifies the structure of the database, making it easier to write queries. Each dimension table is directly related to the fact table, reducing the complexity of joins and making it more intuitive to query the data.
- Improved Query Performance: Because the star schema minimizes the number of joins needed to retrieve data, query performance is often improved. This is especially beneficial for large datasets where complex joins can be computationally expensive.
- Data Aggregation and Reporting: The star schema is optimized for data aggregation and reporting. The structure allows for fast summarization and aggregation of data, which is ideal for analytical queries and generating business reports.
- Scalability: The star schema design is scalable, allowing for the easy addition of new dimension tables without affecting the existing schema. This flexibility is crucial for growing datasets and evolving business requirements.
- Consistency and Reliability: By separating data into fact and dimension tables, the star schema ensures data consistency and reliability. Each piece of data is stored in a single place, reducing redundancy and the risk of data anomalies.


