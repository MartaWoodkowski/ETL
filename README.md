# ETL Process

## Artists, Billboard & Grammy
### Extract: 

There are 3 different datasets limited to the years 1999-2019 from the public platform [Kaggle](https://www.kaggle.com/danield2255/data-on-songs-from-billboard-19992019/version/1) conducted by Daniel DeFoe. The raw data can be found in Resources folder.

The datasets used for this project provided information on:
* Artists
* BillboardHot100 songs from the year 1999 to 2019.
* Grammy songs from 1999 to 2019.

I put each CSV into a pandas DataFrame.

### Transform:

* Copied only the columns needed into a new DataFrame; 
* Renamed the column headers; 
* Transformed all strings to lower case and removed unnecessary strings (i.e. not meaningful symbols); 
* Dropped duplicates and set the index to the previously created primary key.
### Load:

* Created a connection to PostgreSQL database; 
* Checked for a successful connection to the database and confirmed that the tables have been created; 
* Appended DataFrames to tables; 
* Confirmed successful Load by querying database.

### Documentation:

[Documentation Containing Business Rules](Documentation.xlsx)

### Instructions:
Running the program:

1. Open ETL.ipynb
2. run everything and when prompted, enter pgAdmin password




    
    




