# Project2-Producer-Team

Team Members:
Prince Emenalo, Stormm Van Rooi, Corey Chickowski

Proposal:

Hollywood Theatrical Market Synopsis 1995 to 2021
https://www.kaggle.com/johnharshith/hollywood-theatrical-market-synopsis-1995-to-2021?select=HighestGrossers.csv

1. Download nine CSV file sources from the described Kaggle link above

2. Read the CSVs into the jupyter notebook 

3. Transform the imported data into Data Frames and manipulate the data into our desired format

4. Check for duplicates in data and remove duplicates if necessary

5. Modify formatting of data to facilitate analysis
   
   a. Dropped cells in tickets_df and wide_release_df
      
      i. Unnamed: 5
     
     ii. Unnamed: 9
     
    iii. Total Major 6
   
   b. Dropped characters from tables
        
      i. c. Dollar signs
       
     ii. Commas
      
    iii. Percent signs
    
   c. Changed relevant objects to integers and floats
   
   d. Change headers to database rows

6. Create database connection to SQL using Postgres and load our dataframes into the database

7. Write our technical report(below proposal) and upload our report as well as the database to a GitHub repository.

# Techinical Report:

Step 1: Download nice CSV sources analyzing Box Office data from Kaggle Link.

Step 2: Create ipynb file for analysis and import libraries(numpy, pandas, sqlaclhemy).

Step 3: Begin Reading in CSV files for cleaning and formatting appropriate to ultimately load into an SQL Database.

   a. "AnnualTicketSales" CSV file is read into pandas. Modifications and cleaning include dropping 'Unnamed 5' column, removing dollar signs and commas from data. Columns were also rennamed to lower case and spaces removed for SQL formatting.
   Screenshot of final clean data table:

![Annual Ticket Sales Table](https://github.com/cchickowski/Project2-Producer-Team/blob/main/Images/Annual-Ticket-Sales.png)

   b. "HighestGrossers" CSV file is read into pandas. Modifications and cleaning include removing dollar signs and commas from data. Columns were also rennamed to lower case and spaces removed for SQL formatting. 
   Screenshot of final clean data table: 

![Higest Grosser Table](https://github.com/cchickowski/Project2-Producer-Team/blob/main/Images/Highest-Grossing.png)

   c. "PopularCreativeTypes" CSV file is read into pandas. Modifications and cleaning include removing dollar signs, percentage signs, and commas from data. Market Share column converted to a float. Nineth row with unnecessary data is dropped. Columns were also rennamed to lower case and spaces removed for SQL formatting. 
   Screenshot of final clean data table:

![Popular Creative Table](https://github.com/cchickowski/Project2-Producer-Team/blob/main/Images/Popular-Creative-Types.png)

   d. "TopDistributors" CSV file is read into pandas. Modifications and cleaning include removing dollar signs, percentage signs, and commas from data. Data converted to integers and Market Share column converted to a float. Columns were also rennamed to lower case and spaces removed for SQL formatting. 
   Screenshot of final clean data table:

![Top Distributors Table](https://github.com/cchickowski/Project2-Producer-Team/blob/main/Images/Top-Distributors.png)

   e. "TopGenres" CSV file is read into pandas. Modifications and cleaning include removing dollar signs, percentage signs, and commas from data. Data converted to integers and Market Share column converted to a float. Columns were also rennamed to lower case and spaces removed for SQL formatting. 
   Screenshot of final clean data table:

![Top Genres Table](https://github.com/cchickowski/Project2-Producer-Team/blob/main/Images/Top-Genres.png)

   f. "TopGrossingRatings" CSV file is read into pandas. Modifications and cleaning include removing dollar signs, percentage signs, and commas from data. Data converted to integers and Market Share column converted to a float. Columns were also rennamed to lower case and spaces removed for SQL formatting. 
   Screenshot of final clean data table:

![Top Grossing Ratings Table](https://github.com/cchickowski/Project2-Producer-Team/blob/main/Images/Top-Gross-Ratings.png)

   g. "TopGrossingSources" CSV file is read into pandas. Modifications and cleaning include removing dollar signs, percentage signs, and commas from data. Data converted to integers and Market Share column converted to a float. Columns were also rennamed to lower case and spaces removed for SQL formatting. 
   Screenshot of final clean data table:

![Top Grossing Sources Table](https://github.com/cchickowski/Project2-Producer-Team/blob/main/Images/Top-Gross-Sources.png)

  h. "TopProductionMethods" CSV file is read into pandas. Modifications and cleaning include removing dollar signs, percentage signs, and commas from data. Data converted to integers and Market Share column converted to a float. Columns were also rennamed to lower case and spaces removed for SQL formatting. 
   Screenshot of final clean data table:

![Top Production Methods Table](https://github.com/cchickowski/Project2-Producer-Team/blob/main/Images/Top-Production-Methods.png)

   i. "WideReleaseCount" CSV file is read into pandas. Modifications and cleaning includes droppign 'Unnamed: 9' column. Columns were also rennamed to lower case and spaces removed for SQL formatting. Screenshot of final clean data dable: 

![Wide Release Count Table](https://github.com/cchickowski/Project2-Producer-Team/blob/main/Images/Wide-Release-Count.png)

Step 4: Created database connection to SQL using Postgres and loaded our dataframes into the database.
