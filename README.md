# Import-csv-to-table
<p>Hi, in this tutorial I am going to show you how I imported csv file to postgresql table using sql query.</p>
<p>First, create a new table named company_data1 with the following columns:</p><br>

<img src="sample images/csv.png" width="450">

<p>Use the query tool in postgresql to copy the commands as given below</p>
<h4>COPY tablename(atribute1,attribute2,attribute3...) FROM 'Absolute Path to File' DELIMITER ',' CSV HEADER;</h4>
<code><pre>COPY company_data1("Employee ID","Full Name","Job Title","Department","Business Unit","Gender","Ethnicity","Age","Hire Date","Annual Salary","Bonus %","Country","City","Exit Date") 
FROM 'C:\Users\Public\company_data.csv' 
DELIMITER ',' CSV HEADER;</pre></code>
<p>After executing the query we have successfully imported the csv file to table.</p><br>
<img src="sample images/table.png" width="450">
