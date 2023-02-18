Project Purpose:
A music streaming startup, Sparkify, has grown their user base and song database and want to move their processes and data onto the cloud. Their data resides in S3, in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

As their data engineer, I'm tasked with building an ETL pipeline that extracts the data from S3, stages them in Redshift, and transforms data into a set of dimensional tables for the analytics team to continue finding insights into what songs our users are listening to.


Our tasks will be as follows:

1- We will create 2 staging tables and fill them with a copy of the data saved on s3 directories 'logs' & 'songs'.

2- We will create a star schema consisting of 5 different data tables (4 dimentions and 1 fact table). This will facilitate the work of our analytical team by making the process of querying and analyzing data easy.

After completing the above steps, we will be able to run queries to analyze the data available after inserting them in our tables.

Project files include the below:

* Configuration file "dwh"
* 3 python scripts:
    a) sql_queries: contains the sql statements for creating & deleting all tables.
    b) create_tables: contains the functions used for creating and deleting the tables.
    c) etl: contains 
* Jupyter notebook 'Data Warehouse-Project' used to connect to the cluster in addition to running the python scripts by the magic command % .