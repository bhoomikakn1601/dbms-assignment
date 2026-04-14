# DBMS Assignment - Relational Algebra

## Tables:
Employee(EmpID, Name, Salary, DeptID)  
Department(DeptID, DeptName, Location)  

---

### 1. Employees with salary > 50000
σ Salary > 50000 (Employee)

I used selection here to filter employees whose salary is more than 50000.

---

### 2. Names of employees with salary > 50000
π Name (σ Salary > 50000 (Employee))

First I selected employees with salary > 50000, then projected only the Name column.

---

### 3. Employees in DeptID = 2
σ DeptID = 2 (Employee)

This selects employees who belong to department 2.

---

### 4. Names of employees in HR department
π Name (σ DeptName = 'HR' (Employee ⋈ Department))

Here I joined Employee and Department tables, then selected HR department and projected names.

---

### 5. Names and salary of employees in Bangalore
π Name, Salary (σ Location = 'Bangalore' (Employee ⋈ Department))

I joined both tables, filtered by Bangalore location, and displayed name and salary.
