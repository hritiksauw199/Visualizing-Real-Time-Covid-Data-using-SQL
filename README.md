# Visualizing UK's real-Time Covid-Data using SQL

In this project we explores the UK Gov's COVID-19 data which is 
publically available for download via a REST API from gov.uk. 
We make use of a Sqlite3 database to query this data using SQL and 
import aggregations into Pandas data frames. We then use the Seaborn
library to visualise the results.

Dataset Link: https://coronavirus.data.gov.uk/details/download

Additionally, the dataset can be downloaded from this repository `c19.db.gz`.
Download it and extract the rar file.

`Note`: Download the `ltla_utla_region_mappings.csv` file from this
repository.

# Steps carried out

1. Loading Libraries and Connecting to Database
2. Create Tables to store data
   - For more details, see https://coronavirus.data.gov.uk/details/developers-guide/main-api
   - See the `structure` and `list of valid values for areaType metrics`
3. Extract Data using API
   - Convert column names from Camel Case to Snake Case
   - Handling Metrics and Area Types in REST API
4. Extracting Data as CSV file
5. Load the Data (csv file) into the dataframe
