# DataWarehouse
REST API- SSIS- SQL

1. Consume any REST API and load the response to database. You 
don’t need to load all the response fields, 3 or 4 is okay for me.

2. Implement SCD type 6 for the below “EMPLOYEE_Q2” table:
ID Name City Email Update_Date
1001 Ahmed Cairo ahmed@mail.com 20-04-2023
1002 Alaa Giza alaa@mail.com 20-04-2023
1003 Samy Cairo samy@mail.com 20-04-2023
Notes:
1. The SCD fields are City and Email.
2. Read source data using Incremental Load.

3.  Load data to a table using versioning like below:
3.1 Source table “EMPLOYEE_Q3”
ID Name City Email Schedule_Date
1001 Ahmed Cairo ahmed@mail.com 20-04-2023
1002 Alaa Giza alaa@mail.com 20-04-2023
1003 Samy Cairo samy@mail.com 20-04-2023
3.2 Target table after first run on the same day
3.3 Target table after second run on the same day
3.4 Target table after first run on the next day (just change Schedule_Date
in the source data to simulate to next day)

