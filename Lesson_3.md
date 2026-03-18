# Exercise 3 — Tasks
1. Find all the Toy Story movies
```sql
SELECT * FROM movies WHERE Title LIKE "Toy Story%";
```
<img width="918" height="217" alt="Screenshot (473)" src="https://github.com/user-attachments/assets/772bb2de-0819-473f-b845-5e79e7c305d2" />

2. Find all the movies directed by John Lasseter
```sql
SELECT * FROM movies WHERE Director="John Lasseter";
```
<img width="933" height="297" alt="Screenshot (474)" src="https://github.com/user-attachments/assets/e9cad33e-edd2-4382-b936-650ee0992aa6" />

3. Find all the movies (and director) not directed by John Lasseter
```sql
SELECT Title,Director FROM movies WHERE Director IS NOT "John Lasseter";
```
<img width="938" height="499" alt="Screenshot (475)" src="https://github.com/user-attachments/assets/3efd55c8-4b28-4094-9b6a-8363aabfd0e6" />

4. Find all the WALL-* movies
```sql
SELECT * FROM movies WHERE Title Like "WALL-%";
```
<img width="928" height="180" alt="Screenshot (476)" src="https://github.com/user-attachments/assets/9c576c7a-445f-4666-81e2-ae0a50a7b34a" />

 
