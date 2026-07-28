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

<img width="1215" height="819" alt="image" src="https://github.com/user-attachments/assets/e6a1d3a7-8f3f-4c93-a4b1-609ac31b9eb7" />


### Entities and Attributes

<img width="627" height="318" alt="image" src="https://github.com/user-attachments/assets/5a706a4d-2ca1-4c83-bd1b-746bc5efb35c" />

### Relationships and Constraints
<img width="505" height="272" alt="image" src="https://github.com/user-attachments/assets/2aa0d40e-296a-4105-9982-f3a5b81c68e7" />


### Assumptions
- A member can join multiple programs.
- Trainers can be assigned to multiple programs.
- Personal training sessions always involve one trainer and one member.

---

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

<img width="1600" height="966" alt="WhatsApp Image 2026-07-27 at 9 22 43 AM" src="https://github.com/user-attachments/assets/e81ede25-389d-4950-8394-244e6231d93e" />


### Entities and Attributes
<img width="863" height="798" alt="image" src="https://github.com/user-attachments/assets/7b606bbb-74b5-4f04-a98a-f9014fe58785" />
            

### Relationships and Constraints
<img width="863" height="750" alt="image" src="https://github.com/user-attachments/assets/13044d02-fcdd-47c2-8538-2465912ef889" />



### Assumptions
- A member can borrow multiple books, but each loan entry is for one book at a time.
- FineAmount is calculated separately and stored in the Loan entity.
- A room can host many events but an event can take place in only one room.

---

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
<img width="1292" height="902" alt="resturant draw drawio" src="https://github.com/user-attachments/assets/8769e259-a6ab-41fe-a040-01a0bb250aa1" />


### Entities and Attributes

<img width="857" height="772" alt="image" src="https://github.com/user-attachments/assets/019da0cd-ee7c-42b4-a601-95f960251083" />

### Relationships and Constraints
<img width="863" height="882" alt="image" src="https://github.com/user-attachments/assets/10715ce1-5dac-49cc-aade-4fbb2dcbe5fd" />


### Assumptions
- A customer may or may not make a reservation before ordering.
- Each order contains one dish per entry (multiple dishes = multiple order entries).
- Billing is done per reservation, not per individual order.
- A waiter can serve multiple orders but an order is handled by exactly one waiter.

---
