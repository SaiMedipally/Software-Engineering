***Date and Time***


In python, Date and Time are stored as special datatype, they can be translated into string reprensentation and common set of codes determine date and time as string formatting.

In pandas date and time are stored as object(string) by default. We need to specify the columns to specify date and time with ```parse_dates``` argument.

```parse_dates``` accepts numbers or names to parse, and also list containing list which is sublist to columns can combine and parsed as one such as date, month and year.

To combine them parse them and store the results in a new column, by suppling a dictionary where each key is new column names and values are list of columns to parse together.
<a href="https://github.com/SaiMedipally/Software-Engineering/blob/main/Codes/Parsing"> Parsing_Date </a>
