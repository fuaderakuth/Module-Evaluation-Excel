# Module-Evaluation-Excel
## Project Title: Healthcare Data Analysis and Insights

* The original datasheet are kept for future reference and a copy of each dataset is made as "Cust Nm_Solution", "Hosp Det_Sol" & "Med Exam_Sol" to workaround the data. *

1. Data Cleaning.
    *  Dataset are extracted to Power Query editor for transforming the data.
    *  Missing values in the "Medical Examinations” Table ( Smoker Field ) and "Hospitalization Details" ( Customer ID,	year,	month,Hospital tier, 	       City tier, & State ID ) Table were identified by checking through filter.
    *  Missing values in the "month" field is replaced by "Sep" as per the instruction by replacing values function in power query, followed by              finding the average of the "year" field and replacing its missing values.
    *  Replaced missing values in the following fields with its modes respectively, "smoker, Hospital tier & City Tier".
    *  Missing values in "State Id" field is replaced by "Unknown" text. 
      
2.  Data Transformation.
    * Split the ‘names’ column in the “Customer Names” Table into columns: ‘Title’, ‘First Name’, and ‘Last Name’ through "text-to-columns" feature.
    * Formatted inconsistencies in "Heart Issues' and 'smoker' columns values by capitalizing text via power query's format tool.
    * Created new two columns "Weight Status" and "Diabetes Status" as per the instruction via power query's "Add Column" > "Custom Column" feature       and "else if" function.
    * A new column named "Date of Birth" were created by merging "year", "month" and "date" through "Merge columns" function in "Add column"              ribbon.
    * "Age" column were created with "DATEDIF" function the excel sheet directly.
    * Changed data type of "Charges" table into currency via power query.    
      
3. Data Exploration, Analysis & Visualization.
    * A new sheet named "Healthcare" were added and combined the three tables using VLOOKUP by keeping the "Customer ID" as the look up value and insights were made with the new table.
