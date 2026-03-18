# Exercise 7 — Tasks
1. Find the list of all buildings that have employees
```sql
SELECT DISTINCT Building FROM Employees;
```
<img width="926" height="167" alt="Screenshot (492)" src="https://github.com/user-attachments/assets/d0a1dfe3-bc06-4f8e-af68-e2389d0a5810" />

2. Find the list of all buildings and their capacity
```sql
SELECT * FROM Buildings;
```
<img width="926" height="262" alt="Screenshot (493)" src="https://github.com/user-attachments/assets/5b1c50ec-b8b4-4eae-b8aa-bd663ccf9331" />

3. List all buildings and the distinct employee roles in each building (including empty buildings)
```sql
SELECT DISTINCT Building_name, Role
FROM Buildings
LEFT JOIN Employees
ON Building_name = Employees.Building;
```
<img width="927" height="330" alt="Screenshot (494)" src="https://github.com/user-attachments/assets/25240d7d-8940-41fb-8218-4fd5af6e9484" />
