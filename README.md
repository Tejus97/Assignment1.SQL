**COMMAND 1
Finding the minimum latitude of the location 
1 – latitude of location 
2 – SELECT min(latitude) as latitude 
3 – FROM ‘bigquery-public-data.austin_bikeshare_stations’ LIMIT 1000
RESULT – 
1-	30.24258

**COMMAND 2
Find the maximum latitude of the location 
1 - Max latitude of the location 
2 – SELECT max(latitude) as latitude 
3 – FROM ‘bigquery-public-data.austin_bikeshare_stations’ LIMIT 1000
Results 
1-	30.29439

**COMMAND 3
SUBSTITUTING THE AVERAGE LATITUDE FROM THE GIVEN DATA 
Average latitude of the location
SELECT avg(latitude) as lat
FROM ‘bigquery-public-data.austin_bikeshare_stations’ LIMIT 1000
RESULTS 
1-	30.268465416666665

**COMMAND 4
FINDING OUT THE AVERAGE UNQIUE KEYS OF CRIME 
SELECT count(clearance_status)
FROM ‘bigquery-public-data.austin_bikeshare_stations’ LIMIT 1000
Results 
1 – 111561

**COMMAND 5
ESTIMATION OF THE NULL HYPOTHESIS VALUES 
SELECT latitude 
FROM ‘bigquery-public-data.austin_bikeshare_stations’ LIMIT 1000
Where latitude is null 
RESULT – Syntax error: Expected end of input but got keyword WHERE at [3:1]

**COMMAND 6
Number of rows in “latitude” and is not null 
1 – SELECTION OF ROWS FROM ‘LATITUDE’ AND IS NOT NULL 
2 – SELECT count(latitude)
FROM ‘bigquery-public-data.austin_bikeshare_stations’ LIMIT 100
Results 
1 – 96

**COMMAND 7 
**SUM TOTAL OF THE LOAD WEIGHT
1 - SELECTION OF ROWS FROM ‘LOAD WEIGHT’ AND IS NOT NULL 
2 – SELECT count(latitude)
 RESULTS 
1 – 96

**COMMAND 8
LOAD SUM WEIGHT
1-	sum of the total load weight 
2-	SELECT sum(load_weight)
3-	FROM ‘bigquery-public-data.austin_bikeshare_stations’ LIMIT 100
Results – 
1 – 7.616688276E9

**COMMAND 9
10 NAMES OF AREAS IN AUSTIN
1-	10 names of areas
2-	SELECT distinct name
3-	FROM ‘bigquery-public-data.austin_bikeshare_stations’ LIMIT 10
Results – 
1-	Rio Grande & 28th
2-	11th & San Jacinto 
3-	Hollow Creek & Barton Hills
4-	22st & University
5-	Nueces & 26th
6-	East 6th & Pedernales St.
7-	Brazos & 6th
8-	Capital Metro HQ – East 5th at Broadway 
9-	Barton Springs @ Kinney Ave 
10-	Henderson & 9th

**COMMAND 10
FINDING THE MAXIMUM PRICE APPROXIMATE OF THE LOCAL CURRENCY 
-- price approx of local currency 
SELECT max(price_approx_local_currency)
FROM ‘bigquery-public-data.austin_bikeshare_stations’ LIMIT 100
Results – 
1 – 283358.66

