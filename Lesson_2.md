# Exercise 2 — Tasks
1. Find the movie with a row id of 6
```sql
SELECT * FROM movies WHERE Id=6;
```
<img width="926" height="160" alt="Screenshot (469)" src="https://github.com/user-attachments/assets/5a7a901d-79c3-48c5-a4cf-7b2e7011a122" />

2. Find the movies released in the years between 2000 and 2010
```sql
SELECT * FROM movies WHERE Year BETWEEN 2000 AND 2010;
```
<img width="926" height="417" alt="Screenshot (470)" src="https://github.com/user-attachments/assets/8550c4bf-9725-42ba-9f1a-8cbdc5d3e5af" />

3. Find the movies not released in the years between 2000 and 2010
```sql
SELECT * FROM movies WHERE Year NOT BETWEEN 2000 AND 2010;
```
<img width="936" height="335" alt="Screenshot (471)" src="https://github.com/user-attachments/assets/71db710b-5b6b-4786-ac30-0b9ad561ecb0" />

4.Find the first 5 Pixar movies and their release year
```sql
SELECT Title,Year FROM movies 
ORDER BY YEAR ASC 
LIMIT 5;
```
<img width="940" height="300" alt="Screenshot (472)" src="https://github.com/user-attachments/assets/6aad12db-ca6e-4894-a910-d9b3aaa39ab5" />

