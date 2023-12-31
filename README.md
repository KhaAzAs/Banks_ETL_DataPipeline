# World's Largest Bank ETL with Python
## Scenario
I have been hired as a data engineer by research organization. My boss has asked me to create a code that can be used to compile the list of the top 10 largest banks in the world ranked by market capitalization in billion USD. Further, the data needs to be transformed and stored in GBP, EUR and INR as well, in accordance with the exchange rate information that has been made available to me as a CSV file. The processed information table is to be saved locally in a CSV format and as a database table.

My job is to create an automated system to generate this information so that the same can be executed in every financial quarter to prepare the report.

## Objective
With this, I now trained to perform ETL operations on real-world data and make the processed information available for further use in different formats.

I should now be able to:
- Use Webscraping techniques to extract information from any website as per requirement.
- Use Pandas data frames and dictionaries to transform data as per requirement.
- Load the processed information to CSV files and as Database tables.
- Query the database tables using SQLite3 and pandas libraries.
- Log the progress of the code properly.

## Process Steps

### Data Source
Data taken from Wikipedia archived data [List of largest banks](https://web.archive.org/web/20230908091635/https://en.wikipedia.org/wiki/List_of_largest_banks).
![Data source](https://raw.githubusercontent.com/KhaAzAs/ETL_Banks_Project/main/Screenshoot/Task_2a_extract.png)

### Data Extracted
Data extracted from webscraping
<p align="center">
![Data extracted](https://raw.githubusercontent.com/KhaAzAs/ETL_Banks_Project/main/Screenshoot/Task_2c_extract.png)
</p>

### Data Transformed
Data transformed to other currency (GBP, EUR, INR)
> [!NOTE]
> Screenshot only show data in INR (Indian Rupee).
![Data transformed](https://raw.githubusercontent.com/KhaAzAs/ETL_Banks_Project/main/Screenshoot/Task_3b_transform.png)

### Data Load
Data loaded to CSV file
![Data load](https://raw.githubusercontent.com/KhaAzAs/ETL_Banks_Project/main/Screenshoot/Task_4_CSV.png)

### Data Query
Query on loaded data in SQL to read and analyze data. with command
```
SELECT * FROM Largest_banks
```
```
SELECT AVG(MC_GBP_Billion) FROM Largest_banks
```
```
SELECT Name from Largest_banks LIMIT 5
```
![Data query](https://raw.githubusercontent.com/KhaAzAs/ETL_Banks_Project/main/Screenshoot/Task_6_SQL.png)

### Logged ETL Process
![Code logged](https://raw.githubusercontent.com/KhaAzAs/ETL_Banks_Project/main/Screenshoot/Task_7_log_content.png)
