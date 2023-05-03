Download Link: https://assignmentchef.com/product/solved-cs341-project-05-divvy-database-app
<br>
The project is to develop a console application using C# and ADO.NET that retrieves data from a Divvy database residing in Azure:

Use the same login credential as the crimes database:

<u>server</u>: uiccs341.database.windows.net <u>authentication type</u>: SQL Login <u>user</u>: student

<u>pwd</u>: cs341!uic

Much like HW #11, you’ll be putting the SQL queries to retrieve various data from the database into separate .sql files.  In this case you’ll be retrieving data about Divvy trips much like you did against the csv file of trips in Project 4.

<h1>Assignment</h1>

For each of the following problems, write a query which retrieves the data containing the answer in Project05##.sql, where ## is the number of the question, such as 01.

<ol>

 <li>Retrieve the number of trips recorded in the database as NumTrips.</li>

 <li>Retrieve the number of unique bikeIDs as NumBikes.</li>

 <li>For each BikeID, retrieve the bikeID, number of trips taken with that bike as NumTrips and the total amount of time that bike was checked out as TimeCheckedOut. Restrict the results to the top 10 by total time checked out in order.</li>

 <li>For each StationID, retrieve the ID, number of trips taken from that station as NumTripsFrom and to that station as NumTripsTo (as separate values). Order the results in descending order by the total number of trips both from and to the station.</li>

 <li>For each customer list the number of trips they have taken. Include the customer ID and the number of trips as NumTrips, ordering the results from most to fewest trips.   If multiple users have taken the same number of trips, order the results by UserID in ascending order. Restrict the results to the 10 users who have taken the most trips.</li>

 <li>For each age group (year) among customers, list the average ride duration for trips customers of that age group took. The table should include the age group as Age, and Average trip duration for users in that age group as AverageTripDurationPerAgeGroup.  Sort the results from longest trips to shortest, trimming the table to the top 10 entries.</li>

 <li>For each hour of the day, list how many bikes were checked out during that time as NumTrips. Order the results starting from 0 (midnight) up through 23 (11 pm).</li>

 <li>For each hour of the day, list the percentage of bikes checked out during that hour relative to the other hours of the day AS Percentage. Order the results starting from 0 (midnight) up through 23 (11 pm).</li>

 <li>The station contains a location as latitude and longitude. Compute for each trip the distance covered by that trip, using the following equation to approximate: sqrt( (69 miles * difference in latitude)^2 + (52 miles * difference in longitude)^2 ).  For this computation, use the SQRT function and SQUARE function in SQL.  For the 10 longest trips, return the trip ID, starting station ID, ending station ID, and distance travelled as Distance.</li>

 <li>Compute for each trip the average speed of the bicyclist, by taking the distance travelled computed in the previous question (which is in miles) and divide by the length in hours (the length is stored in seconds). For the 10 fastest trips, return the trip ID, bike ID, and the speed as mph.</li>

</ol>

<h1>Requirements</h1>

You will be required to use an SQL join when retrieving data from more than one table.  Join tables by putting commas between them in the FROM clause, then including the condition that the primary key matches the foreign key in the WHERE clause.

Given the importance of database applications, there are numerous tools that generate SQL for you (e.g.

from the database schema).  Such tools cannot be used — you are required to write your SQL queries yourself, from scratch.

<h1>Programming environment:  Codio</h1>

You are free to work in whatever programming environment you prefer.  By default, you can login to Codio and begin work immediately using the project “project06”.  This environment is similar to the one from HW11, containing SQL files for you to write your code and buttons to test your answers.


