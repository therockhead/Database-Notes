-Using the database named "asifdb"
-creating table with their data type

**DECIMAL(decimal_part_size, precision_point)**
```
USE asifdb; 
CREATE TABLE employees (
	employeeID INT,
    firstName VARCHAR(50),employees
    last_Name VARCHAR(50),
    hourlyPay DECIMAL(5, 2),
    hireDate DATE
);
```
SELECTING a Table
-----------------------
```SELECT * FROM employees;```

Renaming a table
-----------------------
```RENAME TABLE employees to workers;```

the table named "employees" getting renamed to "workers" :)

To Drop/Delete a Table
----------------------

```DROP TABLE workers;```

TO ADD COLUMN IN TABLE
----------------------

```
ALTER TABLE workers
ADD phone_number VARCHAR(15);
```

![image](https://github.com/user-attachments/assets/6566a946-6dad-4a9a-b172-288dfd87c862)

Here we can see new column phone_number is added.

TO RENAME CERTAIN COLUMN
-------------------------

```
ALTER TABLE workers
RENAME COLUMN phone_number to Email;
```

![image](https://github.com/user-attachments/assets/70354a8b-9b05-42b5-9afb-5a6ca8dcb86f)

The phone_number column was renamed to "Email" Column.

TO MODIFY DATA TYPE
--------------------

```
ALTER TABLE workers
MODIFY COLUMN Email varchar(100);
```

![image](https://github.com/user-attachments/assets/dbf45adf-db6f-4ec8-bf65-452e193624cc)

NOW the varchar size is 100, it was 15 before.

TO REARRANGE THE ORDER OF THE COLUMNS
------------------------------------

```
ALTER TABLE workers
MODIFY Email VARCHAR(100)
AFTER last_Name;
```

![image](https://github.com/user-attachments/assets/e4bd63a5-350a-4123-bb9d-37eaa7bcc405)
T
he Email is now after last_Name.

We can also move the "Email" Column at the first position by adding FIRST keyword

```
ALTER TABLE workers
MODIFY Email VARCHAR(100)
FIRST;
```

![image](https://github.com/user-attachments/assets/89766c22-4684-4f9c-9e7e-2057f0dd6784)




