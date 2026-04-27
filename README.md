## Navya Bhargava
## 25070123079

#  Experiment 20: COVID-19 Data Analysis

## Aim 

The aim of this experiment is to analyze COVID-19 dataset using Python and Pandas. The objective is to preprocess the dataset, calculate active cases, and analyze the number of confirmed, recovered, and death cases for different countries based on the latest available date.

## Theory 

Data analysis is the process of inspecting, cleaning, transforming, and modeling data to discover useful information and support decision-making.

In this experiment, Python libraries such as Pandas and NumPy are used for handling and analyzing the COVID-19 dataset.


Key concepts used in the experiment include:

1) Data Cleaning: Removing unnecessary columns and correcting data types.
 
2) Data Transformation: Converting date columns into datetime format.
 
3) Feature Engineering: Creating a new column for Active Cases using the formula: Active = Confirmed − Recovered − Deaths
 
4) Data Filtering: Extracting data for the most recent observation date.
 
5) Grouping and Aggregation: Summarizing data by country to determine total confirmed, deaths, recovered, and active cases.

These techniques help in understanding how the pandemic affected different regions.

## Algorithms ⚙️


### 1. Algorithm for Importing Libraries

Start the program.

Import the Pandas library for data manipulation.

Import the NumPy library for numerical operations.

Ensure the libraries are successfully loaded.

---

### 2. Algorithm for Loading the Dataset

Specify the file path of the COVID-19 dataset.

Use the read_csv() function from Pandas to load the dataset.

Store the dataset in a dataframe variable.

Display the first few rows using head() to verify successful loading.

---

### 3. Algorithm for Exploring the Dataset

Display the first five rows of the dataset.

Check the structure of the dataset using info().

View column names and data types.

Identify unnecessary or irrelevant columns.

---

### 4. Algorithm for Data Cleaning

Identify columns that are not required for analysis.

Remove unnecessary columns such as SNo and Last Update.

Check the dataframe again to ensure the columns are removed.

Confirm that the dataset now contains only relevant columns.

---

### 5. Algorithm for Data Type Conversion

Identify columns with incorrect data types.

Convert ObservationDate to datetime format.

Convert Confirmed, Deaths, and Recovered columns to integer type.

Verify the changes using info().

---

### 6. Algorithm for Creating Active Cases Column

Create a new column named Active.

Use the formula:
Active = Confirmed − Recovered − Deaths

Store the calculated values in the new column.

Display the dataframe to verify the new column.

---

### 7. Algorithm for Finding the Latest Observation Date

Access the ObservationDate column.

Use the max() function to determine the latest date.

Store the latest date in a variable.

Display the latest observation date.

---

### 8. Algorithm for Filtering Data for the Latest Date

Compare each record's observation date with the latest date.

Filter rows where the date matches the latest observation date.

Store the filtered data in a new dataframe.

Display the filtered dataset.

---

### 9. Algorithm for Counting Affected Countries

Access the Country/Region column in the filtered dataset.

Identify unique country names using unique().

Count the number of countries using len().

Display the total number of affected countries.

---

### 10. Algorithm for Country-Wise Data Analysis

Group the dataset by Country/Region.

Calculate the total values for:

Confirmed cases
Deaths
Recovered cases
Active cases

Use aggregation functions such as sum().

Store the grouped results in a new dataframe.

Display the summarized country-wise statistics.

---


read_csv(): Used to load dataset from a CSV file into a DataFrame.

head(): Displays the first few rows of the dataset for quick preview.

drop(): Removes unwanted columns or rows from the dataset.

axis: Defines whether operation is applied on rows (0) or columns (1).

info(): Provides summary of dataset including data types, non-null values, and memory usage.

astype(): Used to convert data type of a column (e.g., string to datetime or integer).

datetime64: A data type used for storing date and time values in proper format.

Feature Engineering: Creating new columns from existing data to derive insights.

Active Cases: Calculated as Confirmed − Recovered − Deaths to find current cases.

max(): Returns maximum value from a column (used to find latest date).

Filtering: Selecting rows based on conditions using boolean indexing.

groupby(): Groups data based on a column and performs aggregation.

Aggregation: Applying functions like sum(), mean() on grouped data.

sum(): Calculates total values for grouped data.

reset_index(): Converts grouped index into a normal column.

nunique(): Returns number of unique values in a column.

unique(): Returns unique elements present in a column.

iloc: Used for integer-based indexing to access specific rows.

Sorting: Arranging data in ascending or descending order using sort_values().

sort_values(): Sorts dataset based on column values.

Boolean Indexing: Used to filter data using conditions (e.g., country == India).

fillna(): Replaces missing values with specified value.

Choropleth Map: A map visualization where regions are colored based on data values.

px.choropleth(): Used to create world map visualization using Plotly.

locationmode: Defines how location data is interpreted (e.g., country names).

color_continuous_scale: Defines color gradient used in map visualization.

range_color: Sets range for color scaling.

Time Series Analysis: Analysis of data over time using date column.

Date-wise Grouping: Grouping data by date to analyze trends over time.

Top N Analysis: Selecting top records (e.g., top 20 countries) based on values.

Data Cleaning: Handling missing or inconsistent data for accurate analysis.

Conclusion: This experiment helped in analyzing real-world COVID-19 data using Pandas. It improved understanding of data cleaning, grouping, filtering, and visualization techniques. It also demonstrated how to extract meaningful insights such as active cases, country-wise analysis, and time-based trends.

---
## Conclusion 

The experiment demonstrated how to analyze a real-world COVID-19 dataset using Python and Pandas. Data preprocessing, transformation, and aggregation techniques were used to extract meaningful insights such as active cases and country-wise statistics. This experiment highlights the importance of data analysis techniques in understanding large datasets and deriving useful information.
