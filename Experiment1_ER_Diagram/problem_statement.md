# ER Diagram Workshop – Submission Template

## Objective
To understand and apply ER modeling concepts by creating ER diagrams for real-world applications.

## Purpose
Gain hands-on experience in designing ER diagrams that represent database structure including entities, relationships, attributes, and constraints.

---

# Scenario A: City Fitness Club Management

**Business Context:**  
FlexiFit Gym wants a database to manage its members, trainers, and fitness programs.

**Requirements:**  
- Members register with name, membership type, and start date.  
- Each member can join multiple programs (Yoga, Zumba, Weight Training).  
- Trainers assigned to programs; a program may have multiple trainers.  
- Members may book personal training sessions with trainers.  
- Attendance recorded for each session.  
- Payments tracked for memberships and sessions.

### ER Diagram:

<img width="1138" height="902" alt="Screenshot 2026-03-10 134756" src="https://github.com/user-attachments/assets/df8c75f8-f37c-4636-898f-1d0430459cd3" />





### Entities and Attributes

<img width="1052" height="363" alt="Screenshot 2026-03-10 134810" src="https://github.com/user-attachments/assets/407cfa5d-00fe-4362-90da-bd194b99ba66" />




### Relationships and Constraints

<img width="1068" height="319" alt="image" src="https://github.com/user-attachments/assets/2058d85a-fa4b-4650-8751-968c143b6d0a" />




### Assumptions
IDs are primary keys and unique.
Junction tables resolve all M:N relationships.
Session status covers attendance.

# Scenario B: City Library Event & Book Lending System

**Business Context:**  
The Central Library wants to manage book lending and cultural events.

**Requirements:**  
- Members borrow books, with loan and return dates tracked.  
- Each book has title, author, and category.  
- Library organizes events; members can register.  
- Each event has one or more speakers/authors.  
- Rooms are booked for events and study.  
- Overdue fines apply for late returns.

### ER Diagram:

<img width="1146" height="897" alt="image" src="https://github.com/user-attachments/assets/97452b24-ea0b-49ac-970a-8a648a8d8da7" />


### Entities and Attributes

<img width="1000" height="440" alt="image" src="https://github.com/user-attachments/assets/ef347055-906d-48e4-8942-4c689071c416" />


### Relationships and Constraints

<img width="1041" height="441" alt="image" src="https://github.com/user-attachments/assets/410ddeb9-8dd8-4abf-a6b5-ee71aca77ce2" />


### Assumptions

Each book copy is unique via BookID.

lines are only for late returns.
Rooms can serve multiple purposes (events, study).
M:N relationships are resolved with junction tables.
All IDs are unique primary keys.

# Scenario C: Restaurant Table Reservation & Ordering

**Business Context:**  
A popular restaurant wants to manage reservations, orders, and billing.

**Requirements:**  
- Customers can reserve tables or walk in.  
- Each reservation includes date, time, and number of guests.  
- Customers place food orders linked to reservations.  
- Each order contains multiple dishes; dishes belong to categories (starter, main, dessert).  
- Bills generated per reservation, including food and service charges.  
- Waiters assigned to serve reservations.

### ER Diagram:


<img width="1104" height="803" alt="image" src="https://github.com/user-attachments/assets/b7bbcf23-7eba-40e7-8d3c-1e965fddd44d" />


### Entities and Attributes

<img width="1169" height="413" alt="image" src="https://github.com/user-attachments/assets/b0acf175-261b-433e-b9a9-fe4ed057e6e1" />


### Relationships and Constraints


<img width="1139" height="401" alt="image" src="https://github.com/user-attachments/assets/c8f3c49a-1d88-4cb4-b432-50c102db26ad" />


### Assumptions

Table Assignment: A reservation is assigned to one specific table. Walk-in customers might create a reservation record on the spot.

Order-Reservation Link: Every order must be associated with an existing reservation.
Dish Category: Each dish belongs to a single category.
Bill Generation: A single bill is generated per reservation, encompassing all orders for that reservation.
Waiter Assignment: Waiters can be assigned to multiple reservations, and a single reservation might have multiple waiters over its duration (e.g., shift changes).
All IDs are unique primary keys.


## Instructions for Students

1. Complete **all three scenarios** (A, B, C).  
2. Identify entities, relationships, and attributes for each.  
3. Draw ER diagrams using **draw.io / diagrams.net** or hand-drawn & scanned.  
4. Fill in all tables and assumptions for each scenario.  
5. Export the completed Markdown (with diagrams) as **a single PDF**
