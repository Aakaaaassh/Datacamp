![pig-stands-front-stock-chart_7023-14041](https://github.com/Aakaaaassh/SQL/assets/66636545/83ed4c65-2b0e-451e-a947-07bbff378cf1)
#  Designing a Bank Marketing Database
In 2020 Data Engineering grew by 40% year on year. The ability to extract, transform, and load data is highly sought after by businesses worldwide, and continues to grow in demand.

In this notebook, you will apply your data engineering skills to clean data and design a PostgreSQL database to store information about marketing campaigns run by a bank.

You will need to modify values, add new features, and consider how data should be stored within a PostgreSQL database efficiently and clearly.

## Project Instructions

* Read in <code>bank_marketing.csv</code> as a pandas DataFrame.

* Split the data into three DataFrames using information provided about the desired tables as your guide: one with information about the <code>client</code>, another containing <code>campaign</code> data, and a third to store information about <code>economics</code> at the time of the campaign.

* <P>Rename the column <code>"client_id"</code> to <code>"id"</code> in <code>client</code> (leave as-is in the other subsets); <code>"duration"</code> to <code>"contact_duration"</code>, <code>"previous"</code> to <code>"previous_campaign_contacts"</code>, <code>"y"</code> to <code>"campaign_outcome"</code>, <code>"poutcome"</code> to <code>"previous_outcome"</code>, and <code>"campaign"</code> to <code>"number_contacts"</code> in <code>campaign</code>; and <code>"euribor3m"</code> to <code>"euribor_three_months"</code> and <code>"nr_employed"</code> to <code>"number_employed"</code> in <code>economics</code></P>

* Clean the <code>"education"</code> column, changing <code>"."</code> to <code>"_"</code> and <code>"unknown"</code> to NumPy's null values.

* Remove periods from the <code>"job"</code> column.

* Convert <code>"success"</code> and <code>"failure"</code> in the <code>"previous_outcome"</code> and <code>"campaign_outcome"</code> columns to binary (<code>1</code> or <code>0</code>), along with the changing <code>"nonexistent"</code> to NumPy's null values in <code>"previous_outcome"</code>.

* Add a column called <code>campaign_id</code> in <code>campaign</code>, where all rows have a value of <code>1</code>.

* Create a <code>datetime</code> column called <code>last_contact_date</code>, in the format of <code>"year-month-day"</code>, where the year is <code>2022</code>, and the <code>month</code> and <code>day</code> values are taken from the "month" and "day" columns.

* Remove any redundant data that might have been used to create new columns, ensuring the columns in each subset of the data match the table displayed in the notebook.

* Save the three DataFrames to csv files without an index as <code>client.csv</code>, <code>campaign.csv</code>, and <code>economics.csv</code> respectively.

* Create a Python variable called <code>client_table</code>, containing SQL code as a multi-line string to create a table called <code>client</code> using values from <code>client.csv</code>.

* Create a Python variable called <code>campaign_table</code>, containing SQL code as a multi-line string to create a table called <code>campaign</code> using values from <code>campaign.csv</code>.

* Create a Python variable called <code>economics_table</code>, containing SQL code as a multi-line string to create a table called <code>economics</code> using values from <code>economics.csv</code>.

* In <code>client</code>, <code>campaign</code>, and <code>economic</code>, ensure the final line copies the data from their respective csv files using the following template code snippet: <code>\copy table_name from 'file_name.csv' DELIMITER ',' CSV HEADER</code>
