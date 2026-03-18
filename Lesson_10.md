# Exercise 10 — Tasks
1. Find the longest time that an employee has been at the studio
```sql
SELECT MAX(Years_employed) as Max_years_employed
FROM Employees;
```
<img width="928" height="161" alt="Screenshot (500)" src="https://github.com/user-attachments/assets/f611aac6-057a-4cc1-ab2d-624bc07545f8" />

2. For each role, find the average number of years employed by employees in that role
```sql
SELECT Role, AVG(Years_employed) as Average_years_employed
FROM Employees
GROUP BY Role;
```
<img width="926" height="219" alt="Screenshot (501)" src="https://github.com/user-attachments/assets/b04d54a1-8775-43ec-8941-72020f9f35d9" />

3. Find the total number of employee years worked in each building
```sql
SELECT Building, SUM(Years_employed) as Total_years_employed
FROM Employees
GROUP BY Building;
```
<img width="915" height="179" alt="Screenshot (502)" src="https://github.com/user-attachments/assets/061bbba7-d958-4dde-90c4-9bd944cba94c" />
