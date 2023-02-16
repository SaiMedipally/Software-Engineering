***Date and Time***


In python, Date and Time are stored as special datatype, they can be translated into string reprensentation and common set of codes determine date and time as string formatting.

In pandas date and time are stored as object(string) by default. We need to specify the columns to specify date and time with ```parse_dates``` argument.

```parse_dates``` accepts numbers or names to parse, and also list containing list which is sublist to columns can combine and parsed as one such as date, month and year.

To combine them parse them and store the results in a new column, by suppling a dictionary where each key is new column names and values are list of columns to parse together.
<a href="https://github.com/SaiMedipally/Software-Engineering/blob/main/Codes/Parsing"> Parsing_Date </a>

***Non-Standard Dates***

```parse_dates``` doesn't work with non-standard datetime formats, so to work ```parse_dates``` we need to use ```pd.to_datetime()``` after loading the data. 
And there is a argument to represent the datetime ```format```.

```%Y``` indicates the 4-digit year

```%m``` indicates the month(zero-padded)

```%d``` indicates the day(zero-padded)

```%H``` indicates the hour(24-hour clock)

```%M``` indicates the minute(zero-padded)

```%S``` indicates the second(zero-padded)

dates that pandas could interpret automatically. But if a date is in a non-standard format, like 19991231 for December 31, 1999, it can't be parsed at the import stage. Instead, use pd.to_datetime() to convert strings to dates after import.

```survey_data["Part2EndTime"] = pd.to_datetime(survey_data["Part2EndTime"],format="%m%d%Y %H:%M:%S")```

***Getting data from Databases using Pandas***

To get data from a database, we need to create database engine using SQLAlchemy. 

Using sqlalchemy's ```create_engine()``` makes an engine to handle the database connections.
To load data from a database using pandas we use ```pd.read_sql(query, engine)``` 

```query``` can be indicated by the table name or the sql query and ```engine``` indicates the object which uses as connection between the database.

<a href="https://github.com/SaiMedipally/Software-Engineering/blob/main/Codes/DB%20using%20Pandas" > SQLAlchemy Engine </a>
