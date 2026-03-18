# Exercise 9 — Tasks
1. List all movies and their combined sales in millions of dollars
```sql
SELECT DISTINCT Title,(Domestic_sales + International_sales) / 1000000 
AS Sales
FROM Movies
INNER JOIN Boxoffice
ON Movies.id = Boxoffice.Movie_id;
```
<img width="923" height="497" alt="Screenshot (497)" src="https://github.com/user-attachments/assets/749ab21a-b2f8-4ee1-8e59-0a4e4bdb7eb8" />

2. List all movies and their ratings in percent
```sql
SELECT DISTINCT Title,(Rating * 10) 
AS Rate_percent
FROM Movies
INNER JOIN Boxoffice
ON Movies.id = Boxoffice.Movie_id;
```
<img width="913" height="490" alt="Screenshot (498)" src="https://github.com/user-attachments/assets/febd7659-c226-4141-8bf3-f278eb1c8296" />

3. List all movies that were released on even number years
```sql
SELECT Title FROM Movies WHERE Year % 2 = 0;
```
<img width="905" height="340" alt="Screenshot (499)" src="https://github.com/user-attachments/assets/c83d3866-1687-4e02-977a-06d79c657f83" />
