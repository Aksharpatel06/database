### Database

Certainly! Here's a README file for your SQL table operations on GitHub:

### Employee Management SQL Operations
```markdown
This repository contains SQL scripts for managing an `employees` table. The table includes columns for name, role, salary, age, and phone number. Below are the details of the table structure and various SQL operations performed.
```

### Table Structure

```sql
CREATE TABLE employees (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255),
    role VARCHAR(255),
    salary INT,
    age INT,
    phone VARCHAR(255)
);
```

## Data Insertion

Inserting data into the `employees` table:

```sql
INSERT INTO employees (name, role, salary, age, phone) VALUES ("Akshar", "ceo", 100000, 19, 9727404868);
INSERT INTO employees (name, role, salary, age, phone) VALUES ("Ayush", "hr", 80000, 20, 8654312546);
INSERT INTO employees (name, role, salary, age, phone) VALUES ("Meet", "manager", 75000, 20, 7986542102);
INSERT INTO employees (name, role, salary, age, phone) VALUES ("Ashupal", "emp", 80000, 18, 8541325322);
INSERT INTO employees (name, role, salary, age, phone) VALUES ("Fenish", "emp", 95000, 19, 6854138658);
INSERT INTO employees (name, role, salary, age, phone) VALUES ("Darshan", "emp", 60000, 18, 8979658888);
```

## Data Retrieval

Selecting all data from the `employees` table:

```sql
SELECT * FROM employees;
```

Selecting specific columns:

```sql
SELECT name FROM employees;
SELECT salary FROM employees;
```

Filtering data based on conditions:

```sql
SELECT * FROM employees WHERE role = "manager";
SELECT * FROM employees WHERE name LIKE 'A%';
SELECT * FROM employees WHERE (age > 18 AND salary > 85000);
```

## Data Update

Updating data in the `employees` table:

```sql
UPDATE employees SET salary = 50000 WHERE id = 22;
UPDATE employees SET phone = 6520241545 WHERE id = 24;
```

## Data Deletion

Deleting data from the `employees` table:

```sql
DELETE FROM employees WHERE id = 25;
DELETE FROM employees WHERE age > 19;
```
