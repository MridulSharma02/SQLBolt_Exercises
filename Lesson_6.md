# Exercise 6 — Tasks
1. Find the domestic and international sales for each movie 
```sql
SELECT Title, Domestic_sales, International_sales
FROM Movies
INNER JOIN Boxoffice
    ON Movies.id = Boxoffice.Movie_id;
```
<img width="919" height="498" alt="Screenshot (489)" src="https://github.com/user-attachments/assets/5aac0e6e-d3bb-4b94-8e4e-2c052fb4b384" />

2. Show the sales numbers for each movie that did better internationally rather than domestically
```sql
SELECT Title, Domestic_sales, International_sales
FROM Movies
INNER JOIN Boxoffice
ON Movies.id = Boxoffice.Movie_id
WHERE International_sales > Domestic_sales;
```
<img width="916" height="499" alt="Screenshot (490)" src="https://github.com/user-attachments/assets/954ef8aa-05bf-4686-b791-edcc168f6f06" />

3. List all the movies by their ratings in descending order
```sql
SELECT Title, Rating
FROM Movies
INNER JOIN Boxoffice
ON Movies.id = Boxoffice.Movie_id
ORDER BY Rating DESC;
```
<img width="912" height="503" alt="Screenshot (491)" src="https://github.com/user-attachments/assets/5964000a-b1f7-4506-8f43-acde00a148ef" />


