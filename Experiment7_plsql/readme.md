# Experiment 7: PL/SQL – Variables, Control Structures and Loops

## AIM
To write and execute simple PL/SQL programs using variables, loops, and conditional statements.


## THEORY

PL/SQL, which stands for Procedural Language extensions to the Structured Query Language (SQL). It is a combination of SQL along with the procedural features of programming languages.

**Syntax:**
```sql
DECLARE 
   <declarations section> 
BEGIN 
   <executable command(s)>
EXCEPTION 
   <exception handling> 
END;
```

### Basic Components of PL/SQL Block:
- DECLARE: Section to declare variables and constants.
- BEGIN: The execution section that contains PL/SQL statements.
- EXCEPTION: Handles errors or exceptions that occur in the program.
- END: Marks the end of the PL/SQL block.

# PL/SQL Programs – Steps and Expected Output

## 1. Write a PL/SQL program to find the Greatest of Two Numbers

### Steps:
- Declare two numeric variables and initialize them.
- Use an `IF` statement to compare the values.
- Display the greater number using `DBMS_OUTPUT.PUT_LINE`.

**PROGRAM**

```
DECLARE
    num1 NUMBER := 80;  
    num2 NUMBER := 50;  
BEGIN
    IF num1 > num2 THEN
        DBMS_OUTPUT.PUT_LINE('Greater number is: ' || num1);
    ELSE
        DBMS_OUTPUT.PUT_LINE('Greater number is: ' || num2);
    END IF;
END;
```


**Expected Output:**  
Greater number is: 80

**OUTPUT**

<img width="318" height="124" alt="image" src="https://github.com/user-attachments/assets/7a8086f1-f5ea-4317-a430-d0827654a315" />

---

## 2. Write a PL/SQL program to Calculate Sum of First N Natural Numbers

### Steps:
- Declare a variable `n` and assign a value (e.g., 10).
- Initialize a `sum` variable to 0.
- Use a `WHILE` loop to iterate from 1 to `n`, adding each number to the sum.
- Display the result using `DBMS_OUTPUT.PUT_LINE`.

**PROGRAM**

```
SET SERVEROUTPUT ON;

DECLARE
    n NUMBER := 10;       
    i NUMBER := 1;        
    total_sum NUMBER := 0; 
BEGIN
    WHILE i <= n LOOP
        total_sum := total_sum + i;
        i := i + 1;
    END LOOP;

    DBMS_OUTPUT.PUT_LINE('Sum of first ' || n || ' natural numbers is: ' || total_sum);
END;
```


**Expected Output:**  
Sum of first 10 natural numbers is: 55

**OUTPUT**

<img width="607" height="135" alt="image" src="https://github.com/user-attachments/assets/d25283e2-1928-4fbc-a1d3-cceb9dc79b74" />


---

## 3. Write a PL/SQL program to generate Fibonacci series

### Steps:
- Declare the variable `n` to indicate how many terms to generate.
- Initialize the first two Fibonacci numbers (0 and 1).
- Use a loop to generate the next terms using the formula `c = a + b`.
- Print each term in the series.

**PROGRAM**

```
SET SERVEROUTPUT ON;
DECLARE
    n NUMBER := 7;     
    a NUMBER := 0;    
    b NUMBER := 1;     
    c NUMBER;          
    i NUMBER := 3;     
BEGIN
    DBMS_OUTPUT.PUT_LINE('Fibonacci sequence:');
    DBMS_OUTPUT.PUT_LINE(a);
    DBMS_OUTPUT.PUT_LINE(b);
    WHILE i <= n LOOP
        c := a + b;
        DBMS_OUTPUT.PUT_LINE(c);
        a := b;
        b := c;
        i := i + 1;
    END LOOP;
END;
```

**Expected Output:**  
n = 7  
Fibonacci sequence: 0, 1, 1, 2, 3, 5, 8

**OUTPUT**

<img width="227" height="259" alt="image" src="https://github.com/user-attachments/assets/ca5196e8-8ae5-430e-9a25-a77a0d9e2e78" />


---

## 4. Write a PL/SQL Program to display the number in Reverse Order

### Steps:
- Declare a variable `n` and assign a value (e.g., 1535).
- Use a loop to extract each digit using modulo and reverse the number.
- Display the reversed number.

**PROGRAM**

```
SET SERVEROUTPUT ON;

DECLARE
    n NUMBER := 1535;      
    original NUMBER := 1535;
    reversed NUMBER := 0;   
    digit NUMBER;           
BEGIN
    WHILE n > 0 LOOP
        digit := MOD(n, 10);              
        reversed := reversed * 10 + digit;
        n := TRUNC(n / 10);               
    END LOOP;

    DBMS_OUTPUT.PUT_LINE('n = ' || original);
    DBMS_OUTPUT.PUT_LINE('Reversed number is ' || reversed);
END;
```

**Expected Output:**  
n = 1535  
Reversed number is 5351

**OUTPUT**

<img width="267" height="128" alt="image" src="https://github.com/user-attachments/assets/cece343a-8ddc-4aa1-bf80-22ee8968307a" />


---

## 5. Write a PL/SQL program to find the largest of three numbers

### Steps:
- Declare three numeric variables `a`, `b`, and `c`.
- Use nested `IF-ELSIF-ELSE` conditions to find the largest among the three.
- Display the largest number.

**PROGRAM**

```
SET SERVEROUTPUT ON;

DECLARE
    a NUMBER := 10;
    b NUMBER := 9;
    c NUMBER := 15;
    largest NUMBER;
BEGIN
    IF a >= b AND a >= c THEN
        largest := a;
    ELSIF b >= a AND b >= c THEN
        largest := b;
    ELSE
        largest := c;
    END IF;

    DBMS_OUTPUT.PUT_LINE('a = ' || a || ', b = ' || b || ', c = ' || c);
    DBMS_OUTPUT.PUT_LINE('Largest of three number is ' || largest);
END;
```

**Expected Output:**  
a = 10, b = 9, c = 15  
Largest of three number is 15

**OUTPUT**

<img width="329" height="161" alt="image" src="https://github.com/user-attachments/assets/38debb28-f32b-42e5-b85c-cba08f18c7b7" />


## RESULT
Thus, the PL/SQL programs using variables, conditionals, and loops were executed successfully.

