# Experiment 4: Aggregate Functions, Group By and Having Clause

## AIM
To study and implement aggregate functions, GROUP BY, and HAVING clause with suitable examples.

## THEORY

### Aggregate Functions
These perform calculations on a set of values and return a single value.

- **MIN()** – Smallest value  
- **MAX()** – Largest value  
- **COUNT()** – Number of rows  
- **SUM()** – Total of values  
- **AVG()** – Average of values

**Syntax:**
```sql
SELECT AGG_FUNC(column_name) FROM table_name WHERE condition;
```
### GROUP BY
Groups records with the same values in specified columns.
**Syntax:**
```sql
SELECT column_name, AGG_FUNC(column_name)
FROM table_name
GROUP BY column_name;
```
### HAVING
Filters the grouped records based on aggregate conditions.
**Syntax:**
```sql
SELECT column_name, AGG_FUNC(column_name)
FROM table_name
GROUP BY column_name
HAVING condition;
```

**Question 1**

<img width="1020" height="838" alt="image" src="https://github.com/user-attachments/assets/f281ed52-c66a-408c-98af-7e655cac3d68" />

**Output:**

<img width="753" height="604" alt="image" src="https://github.com/user-attachments/assets/11f23608-98ff-4188-a6f3-0f8e2eced8a2" />


**Question 2**


<img width="785" height="827" alt="image" src="https://github.com/user-attachments/assets/7c9cb37d-c8f4-48f8-b343-82bb211f6237" />


**Output:**

<img width="769" height="752" alt="image" src="https://github.com/user-attachments/assets/99f019f0-1a4f-4272-891f-1e994b727171" />


**Question 3**

<img width="675" height="839" alt="image" src="https://github.com/user-attachments/assets/0b4e073d-5525-4894-8027-87e570d37e06" />


**Output:**

<img width="718" height="720" alt="image" src="https://github.com/user-attachments/assets/f000d8af-a416-4009-8616-5be5179464f4" />


**Question 4**

<img width="839" height="732" alt="image" src="https://github.com/user-attachments/assets/d2ce2752-d740-4034-8013-1fc7e56f8d0c" />


**Output:**

<img width="522" height="382" alt="image" src="https://github.com/user-attachments/assets/6896542d-962d-4084-a73e-f476f9d9aa7f" />



**Question 5**

<img width="1068" height="627" alt="image" src="https://github.com/user-attachments/assets/877d97f9-0bb6-4253-8ef8-69b4a3254b9d" />


**Output:**

<img width="568" height="396" alt="image" src="https://github.com/user-attachments/assets/0e8c57fe-0431-431d-ab85-3ca5b41dc7d3" />


**Question 6**


<img width="867" height="670" alt="image" src="https://github.com/user-attachments/assets/55357bec-6be9-4690-bf4f-76514693d678" />


**Output:**

<img width="735" height="389" alt="image" src="https://github.com/user-attachments/assets/b34aa485-15e3-4c23-b163-1888ce57a5cf" />


**Question 7**

<img width="763" height="675" alt="image" src="https://github.com/user-attachments/assets/a6ebce23-b59f-4bdf-b691-bbbb250737fd" />


**Output:**



<img width="457" height="382" alt="image" src="https://github.com/user-attachments/assets/758e0c13-21cc-4329-b369-443f97d263e4" />


**Question 8**


<img width="1192" height="800" alt="image" src="https://github.com/user-attachments/assets/4976870f-a2b7-434d-b38b-510a447ed22c" />


**Output:**


<img width="788" height="435" alt="image" src="https://github.com/user-attachments/assets/0e05278b-b666-4353-9e41-7034613f15ee" />


**Question 9**


<img width="1199" height="759" alt="image" src="https://github.com/user-attachments/assets/1ec5cfd0-6674-4914-9bb9-5a6f2970e322" />


**Output:**


<img width="628" height="407" alt="image" src="https://github.com/user-attachments/assets/442d90dd-be90-4f4f-8168-d376dd531860" />


**Question 10**


<img width="1196" height="757" alt="image" src="https://github.com/user-attachments/assets/b0a6f6ff-8d62-47e7-a0e2-37b1794da6e7" />


**Output:**


<img width="692" height="461" alt="image" src="https://github.com/user-attachments/assets/fc65bfda-850c-4e50-8d50-858c551f6df4" />



## RESULT
Thus, the SQL queries to implement aggregate functions, GROUP BY, and HAVING clause have been executed successfully.
