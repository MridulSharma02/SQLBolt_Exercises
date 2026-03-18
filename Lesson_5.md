# Exercise 5 — Tasks
1. List all the Canadian cities and their populations
```sql
SELECT City,Population FROM north_american_cities WHERE Country="Canada";
```
<img width="944" height="186" alt="Screenshot (483)" src="https://github.com/user-attachments/assets/f5d2f048-9f6e-46d2-9f93-82d930df87cf" />

2. Order all the cities in the United States by their latitude from north to south
```sql
SELECT City
FROM North_american_cities
WHERE Country = "United States"
ORDER BY Latitude DESC;
```
<img width="932" height="341" alt="Screenshot (484)" src="https://github.com/user-attachments/assets/be4ceea5-4fa0-496b-a76b-cfc157b6c0cb" />

3. List all the cities west of Chicago, ordered from west to east 
```sql
SELECT City
FROM North_american_cities
WHERE Longitude < -87.629798
ORDER BY Longitude;
```
<img width="919" height="344" alt="Screenshot (485)" src="https://github.com/user-attachments/assets/41e7844f-0db4-45ce-8fc2-0b6b5f8ca542" />

4. List the two largest cities in Mexico (by population) 
```sql
SELECT City
FROM North_american_cities
WHERE Country = "Mexico"
ORDER BY Population DESC
LIMIT 2;
```
<img width="937" height="179" alt="Screenshot (486)" src="https://github.com/user-attachments/assets/749c9c0a-186c-47c1-892a-2e564002b91a" />

5. List the third and fourth largest cities (by population) in the United States and their population
```sql
SELECT City
FROM North_american_cities
WHERE Country = "United States"
ORDER BY Population DESC
LIMIT 2 OFFSET 2;
```
<img width="921" height="184" alt="Screenshot (488)" src="https://github.com/user-attachments/assets/36a59da9-7824-48c9-99c3-d8a1d20246db" />
