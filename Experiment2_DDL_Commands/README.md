# Experiment 2: DDL Commands

## AIM
To study and implement DDL commands and different types of constraints.

## THEORY

### 1. CREATE
Used to create a new relation (table).

**Syntax:**
```sql
CREATE TABLE (
  field_1 data_type(size),
  field_2 data_type(size),
  ...
);
```
### 2. ALTER
Used to add, modify, drop, or rename fields in an existing relation.
(a) ADD
```sql
ALTER TABLE std ADD (Address CHAR(10));
```
(b) MODIFY
```sql
ALTER TABLE relation_name MODIFY (field_1 new_data_type(size));
```
(c) DROP
```sql
ALTER TABLE relation_name DROP COLUMN field_name;
```
(d) RENAME
```sql
ALTER TABLE relation_name RENAME COLUMN old_field_name TO new_field_name;
```
### 3. DROP TABLE
Used to permanently delete the structure and data of a table.
```sql
DROP TABLE relation_name;
```
### 4. RENAME
Used to rename an existing database object.
```sql
RENAME TABLE old_relation_name TO new_relation_name;
```
### CONSTRAINTS
Constraints are used to specify rules for the data in a table. If there is any violation between the constraint and the data action, the action is aborted by the constraint. It can be specified when the table is created (using CREATE TABLE) or after it is created (using ALTER TABLE).
### 1. NOT NULL
When a column is defined as NOT NULL, it becomes mandatory to enter a value in that column.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) NOT NULL
);
```
### 2. UNIQUE
Ensures that values in a column are unique.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) UNIQUE
);
```
### 3. CHECK
Specifies a condition that each row must satisfy.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) CHECK (logical_expression)
);
```
### 4. PRIMARY KEY
Used to uniquely identify each record in a table.
Properties:
Must contain unique values.
Cannot be null.
Should contain minimal fields.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) PRIMARY KEY
);
```
### 5. FOREIGN KEY
Used to reference the primary key of another table.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size),
  FOREIGN KEY (column_name) REFERENCES other_table(column)
);
```
### 6. DEFAULT
Used to insert a default value into a column if no value is specified.

Syntax:
```sql
CREATE TABLE Table_Name (
  col_name1 data_type,
  col_name2 data_type,
  col_name3 data_type DEFAULT 'default_value'
);
```

**Question 1**
<img width="1222" height="330" alt="image" src="https://github.com/user-attachments/assets/6f4ccad2-2cdc-46ea-821f-13480908ae5b" />

**Output:**

<img width="1087" height="194" alt="image" src="https://github.com/user-attachments/assets/60bfeb3a-3899-44e2-966c-3ec5b8dc834a" />

---------------------------

**Question 2**

<img width="610" height="330" alt="image" src="https://github.com/user-attachments/assets/63706132-13cd-440b-9565-a85f4699ebbe" />


**Output:**

<img width="641" height="202" alt="image" src="https://github.com/user-attachments/assets/9997930f-4f36-46ba-80f8-32aaf3a8ca51" />

-----------------------------------------------
**Question 3**

<img width="623" height="461" alt="image" src="https://github.com/user-attachments/assets/0bec6a21-a59e-4b53-b70a-20e77fcdbcac" />


**Output:**

<img width="885" height="237" alt="image" src="https://github.com/user-attachments/assets/374b2d3b-76c5-4cc9-8377-bfe505232786" />

-------------------------------------------------
**Question 4**

<img width="883" height="399" alt="image" src="https://github.com/user-attachments/assets/8e1a4cf5-26cb-45db-8dc5-272b377fe23b" />


**Output:**

<img width="768" height="168" alt="image" src="https://github.com/user-attachments/assets/d90120b6-a787-4588-a12f-697ff5cf45bc" />

------------------------------------------------


**Question 5**

<img width="529" height="370" alt="image" src="https://github.com/user-attachments/assets/91a64bae-02b0-4287-9023-48eeb747e5ad" />


**Output:**

<img width="781" height="173" alt="image" src="https://github.com/user-attachments/assets/8bc84a61-d60c-4f61-9576-83fb3d510721" />

------------------------------------------------
**Question 6**


<img width="770" height="348" alt="image" src="https://github.com/user-attachments/assets/381fed75-ff55-4f58-89ae-13b895e91142" />


**Output:**

<img width="1027" height="178" alt="image" src="https://github.com/user-attachments/assets/affc9303-ff95-4071-aef3-f7a84abdba22" />

----------------------------------------------
**Question 7**

<img width="636" height="357" alt="image" src="https://github.com/user-attachments/assets/eb26f0ec-5f34-4ade-88b9-373c4202a168" />


**Output:**

<img width="894" height="196" alt="image" src="https://github.com/user-attachments/assets/17007307-522d-4d6e-b8ca-ade0c57cdaf6" />

-----------------------------------------------------------

**Question 8**

<img width="542" height="465" alt="image" src="https://github.com/user-attachments/assets/94c8439d-669a-4119-a865-4a7b75256603" />


**Output:**

<img width="813" height="202" alt="image" src="https://github.com/user-attachments/assets/bd7fd9ce-eff1-4a10-96dc-e0d06950a21a" />

----------------------------------------------------
**Question 9**

<img width="477" height="322" alt="image" src="https://github.com/user-attachments/assets/419a2fc6-d148-43a5-8292-cfefda24c810" />


**Output:**

<img width="798" height="180" alt="image" src="https://github.com/user-attachments/assets/95966f4b-2226-4a47-901a-2049eb7e1044" />

------------------------------------------------

**Question 10**

<img width="517" height="434" alt="image" src="https://github.com/user-attachments/assets/d8fb8794-21a5-4994-b862-45ec50e1a338" />


**Output:**

<img width="1020" height="232" alt="image" src="https://github.com/user-attachments/assets/01ebb3e1-3a95-4130-8873-e3c79603f55b" />




## RESULT
Thus, the SQL queries to implement different types of constraints and DDL commands have been executed successfully.
