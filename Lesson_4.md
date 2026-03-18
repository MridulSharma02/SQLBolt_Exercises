# Exercise 4 — Tasks
1. List all directors of Pixar movies (alphabetically), without duplicates
```sql
SELECT DISTINCT Director FROM Movies ORDER BY Director ASC;
```
<img width="931" height="382" alt="Screenshot (479)" src="https://github.com/user-attachments/assets/0cf12b68-6b08-4610-bed9-a20550ee003e" />

2. List the last four Pixar movies released (ordered from most recent to least)
```sql
SELECT Title,Year FROM Movies 
ORDER BY Year DESC 
LIMIT 4;
```
<img width="936" height="266" alt="Screenshot (478)" src="https://github.com/user-attachments/assets/111f160c-b988-4ae6-828a-9975a08ed42f" />

3. List the first five Pixar movies sorted alphabetically
```sql
SELECT Title FROM Movies 
ORDER BY Title
LIMIT 5;
```
<img width="920" height="303" alt="Screenshot (481)" src="https://github.com/user-attachments/assets/70f2bf67-c8b7-46fd-b2f7-cdbe8e181d65" />

4. List the next five Pixar movies sorted alphabetically
```sql
SELECT title FROM movies ORDER BY title LIMIT 5 OFFSET 5;
```
<img width="941" height="301" alt="Screenshot (482)" src="https://github.com/user-attachments/assets/4caa571b-c544-4ef0-8ccc-ed29fffd87a0" />
