# Exercise 8 — Tasks
1. Find the name and role of all employees who have not been assigned to a building
```sql
SELECT Name, Role FROM Employees WHERE Building IS NULL;
```
<img width="922" height="199" alt="Screenshot (495)" src="https://github.com/user-attachments/assets/08e54624-fa06-49b4-acd2-9169ec072146" />

2. Find the names of the buildings that hold no employees
```sql
SELECT DISTINCT Building_name
FROM Buildings
LEFT JOIN Employees
ON Building_name = Employees.Building
WHERE Employees.Building IS NULL;
```
<img width="914" height="184" alt="Screenshot (496)" src="https://github.com/user-attachments/assets/ca789a62-6dee-4a37-8de4-55dda1918d1a" />
