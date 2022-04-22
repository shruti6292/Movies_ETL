# Movies_ETL
In this Challenge we created an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. For this we refactored the code from the module to create one function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data—and performs the ETL process by adding the data to a PostgreSQL database.
There are 4 steps to achieve this. 
- 1: Write an ETL Function to Read Three Data Files
- 2: Extract and Transform the Wikipedia Data
- 3: Extract and Transform the Kaggle data
- 4: Create the Movie Database

## Extracting and Transform phase of the Data :

From various resources, we have extracted the raw data and then processed it in Jupyter Notebbok  by inspecting, planning and executing  multiple steps to get clean data to perform ETL pipeline. Things we have done are, creating functions to read the data by using dataframes. Learning how to write lambda function, how to use Regex, and how to clean the data and also how to set the variables through the functions. 

### Original Raw data files:

![alt_text](https://github.com/RGK73/Movies_ETL/blob/main/Images/Raw_Data_1.png)

![alt_text](https://github.com/RGK73/Movies_ETL/blob/main/Images/Raw_Data_2.png)

![alt_text](https://github.com/RGK73/Movies_ETL/blob/main/Images/Raw_Data_3.png)

### Files after Extract and Transform phase of the ETL pipeline

![alt_text](https://github.com/RGK73/Movies_ETL/blob/main/Images/clean_data_1.png)

![alt_text](https://github.com/RGK73/Movies_ETL/blob/main/Images/clean_data_2.png)

![alt_text](https://github.com/RGK73/Movies_ETL/blob/main/Images/clean_data_3.png)

## Load phase of the clean data

Apart from how to create a function and use lambda and Regex, we learned how to connect to the database through jupyter notebook. How to drop the table from database from our code and how much time is required to complete ETL process.
After extracting, transforming and cleaning the data, we needed to load the data in PostgreSQL to give it to Britta for Hackathon.
In this phase,The data from the movies_df DataFrame replaces the current data in the movies table in the SQL database. 
The data from the MovieLens rating CSV file is added to the ratings table in the SQL database.The elapsed time to add the data to the database is displayed as shown below.

![alt_text](https://github.com/RGK73/Movies_ETL/blob/main/Resources/movies_query.png)

![alt_text](https://github.com/RGK73/Movies_ETL/blob/main/Resources/movies_query_messages.png)

![alt_text](https://github.com/RGK73/Movies_ETL/blob/main/Resources/ratings_query.png)

![alt_text](https://github.com/RGK73/Movies_ETL/blob/main/Resources/ratings_query_messages.png)

![alt_text](https://github.com/RGK73/Movies_ETL/blob/main/Images/Elapsed_Time.png)

## Summary: 

Taking raw data and processing and loading it to form an ETL pipeline is very interesting and time consuming process. To know how to transform data is a learned skill with lot of practice. In the end to see the data transformation is like with the help of all these tools is very magical.
