# SSMS-SQL-PowerQueryM-Functions :atom:
Using Power Query M to extract values from Excel workbooks for dynamic insertion into SQL code.

## Requirements :basecamp:
* `SSMS`
* `ODBC Driver For SQL Server`
* `Microsoft Excel`

## Instructions :page_with_curl:
* Ensure you have all the requirements and everything is configured properly (especially SSMS and the ODBC Driver).
* Open an Excel Workbook.
* Name you're first sheet as Parameters (this is where we will be extracting the text value from).
* Paste your SSMS server name wherever you'd like (ideally on the top left corner).
* Have another cell ready below the server name for continents, and name the cells 'Server' and 'Continent', respectively.
* Now go to the `Data Tab` :arrow_right: `Get Data` :arrow_right: `From Other Sources` :arrow_right: `Blank Query` :arrow_right: `Advanced Editor`.
* Once you're in the Advanced Editor you will need to first input the fnGetParam Power Query M script I've attached, this code basically extracts the value from the named cells (make sure the it is named fnGetParam or else the function call will not work).
* Create another blank query either by right-clicking in the [Queries] section and selecting New Query.
* Paste the SQL code I've attached and change all the necessary customizable named components such as the ODBC Driver you're using and the database you're extracting from.
* Voila, you can now close and load, and if it asks you for authentication, I usually select `Windows` :arrow_right: `Use Current Credentials`. 

## Video Sample :film_strip:

[Watch the video](https://github.com/Turnipdo/SSMS-SQL-PowerQueryM-Functions/blob/main/fnGetParam.mp4)



