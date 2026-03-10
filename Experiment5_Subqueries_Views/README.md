# Experiment 5: Subqueries and Views

## AIM
To study and implement subqueries and views.

## THEORY

### Subqueries
A subquery is a query inside another SQL query and is embedded in:
- WHERE clause
- HAVING clause
- FROM clause

**Types:**
- **Single-row subquery**:
  Sub queries can also return more than one value. Such results should be made use along with the operators in and any.
- **Multiple-row subquery**:
  Here more than one subquery is used. These multiple sub queries are combined by means of ‘and’ & ‘or’ keywords.
- **Correlated subquery**:
  A subquery is evaluated once for the entire parent statement whereas a correlated Sub query is evaluated once per row processed by the parent statement.

**Example:**
```sql
SELECT * FROM employees
WHERE salary > (SELECT AVG(salary) FROM employees);
```
### Views
A view is a virtual table based on the result of an SQL SELECT query.
**Create View:**
```sql
CREATE VIEW view_name AS
SELECT column1, column2 FROM table_name WHERE condition;
```
**Drop View:**
```sql
DROP VIEW view_name;
```

**Question 1**


<img width="1285" height="917" alt="image" src="https://github.com/user-attachments/assets/8e1556dc-94dc-4c8a-93bb-022cad1bf570" />


**Output:**

<img width="1661" height="609" alt="image" src="https://github.com/user-attachments/assets/775643c2-11a0-4cff-bb22-9fdb98af3c0b" />


**Question 2**

<img width="1047" height="783" alt="image" src="https://github.com/user-attachments/assets/5a237762-ea05-4371-a859-2fc71c6e3a63" />


**Output:**

<img width="1286" height="519" alt="image" src="https://github.com/user-attachments/assets/0c9a1443-d4f3-4294-b10b-05baf259506b" />


**Question 3**

<img width="885" height="795" alt="image" src="https://github.com/user-attachments/assets/75104b1d-02d9-401b-9a95-af420956b328" />

**Output:**

<img width="1137" height="359" alt="image" src="https://github.com/user-attachments/assets/2c30b54d-7e7e-4de8-851a-b15b1ff3416b" />


**Question 4**

<img width="831" height="639" alt="image" src="https://github.com/user-attachments/assets/d381ea61-a07f-434c-b985-5a33cd53f04a" />

**Output:**

<img width="783" height="427" alt="image" src="https://github.com/user-attachments/assets/84ca9a4d-7751-4785-b5c6-d36ecc842f5d" />


**Question 5**


<img width="1036" height="871" alt="image" src="https://github.com/user-attachments/assets/b9b076f4-fb0e-4f66-933b-7cfdbb12acb0" />

**Output:**

<img width="1381" height="551" alt="image" src="https://github.com/user-attachments/assets/53824791-4f7c-4988-a492-f7ebf67f363b" />


**Question 6**


<img width="1333" height="956" alt="image" src="https://github.com/user-attachments/assets/e30e7c1b-ecc2-4e23-b18d-ae9fd250b564" />

**Output:**

<img width="564" height="621" alt="image" src="https://github.com/user-attachments/assets/8316a731-5754-4bd5-b90a-76fe9e7155a7" />


**Question 7**

<img width="1270" height="923" alt="image" src="https://github.com/user-attachments/assets/06e72839-5ab9-4e94-a4bb-64cfa246ce02" />

**Output:**

<img width="1503" height="523" alt="image" src="https://github.com/user-attachments/assets/c61f0155-9607-4144-885f-b82005926b82" />


**Question 8**

<img width="1487" height="883" alt="image" src="https://github.com/user-attachments/assets/9b04a972-51e7-49d3-8518-64375fdcaca4" />

**Output:**

<img width="1401" height="580" alt="image" src="https://github.com/user-attachments/assets/e73d7b47-c2c8-4d9d-8e47-37a756c3b1e5" />


**Question 9**

<img width="1218" height="877" alt="image" src="https://github.com/user-attachments/assets/aa7c6d0a-109d-4923-860b-772fd076a5a7" />

**Output:**

<img width="1508" height="512" alt="image" src="https://github.com/user-attachments/assets/ab6f8ab8-a2ba-410a-8880-e6c9deae55c2" />


**Question 10**

<img width="1098" height="956" alt="image" src="https://github.com/user-attachments/assets/58e50970-655e-4455-9146-10286414f634" />


**Output:**

<img width="1422" height="709" alt="image" src="https://github.com/user-attachments/assets/f87acdc8-5f8d-4f1f-b3b9-06f8a9b1594b" />


## RESULT
Thus, the SQL queries to implement subqueries and views have been executed successfully.
