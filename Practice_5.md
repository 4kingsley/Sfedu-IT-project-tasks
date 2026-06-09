# Practice 5. System Structure and Modeling  
## SFedU Student Event Portal

---

# 1. Introduction

The purpose of Practice 5 is to describe the **system structure**, define the **main components**, and present **UML-style diagrams** in Markdown format for the SFedU Student Event Portal.  
These diagrams help visualize the architecture, data flow, and interactions between system elements.

All diagrams are simplified for academic use and formatted to display correctly in GitHub.

---

# 2. System Architecture Overview

The system follows a **three-layer architecture**:

### **1. Presentation Layer (Frontend)**
- event catalog  
- event detail pages  
- registration form  
- organizer dashboard UI  

### **2. Application Layer (Backend)**
- event management logic  
- registration processing  
- ticket generation  
- user/role management  

### **3. Data Layer (Database)**
- events table  
- users table  
- registrations table  

---

# 3. Component Diagram (Markdown UML)

```
+---------------------------+
|     Presentation Layer    |
|---------------------------|
| - Event Catalog UI        |
| - Event Details UI        |
| - Registration Form       |
| - Organizer Dashboard     |
+-------------+-------------+
              |
              v
+---------------------------+
|    Application Layer      |
|---------------------------|
| - Event Controller        |
| - Registration Controller |
| - Ticket Generator        |
| - Auth / Role Manager     |
+-------------+-------------+
              |
              v
+---------------------------+
|        Data Layer         |
|---------------------------|
| - Events Table            |
| - Users Table             |
| - Registrations Table     |
+---------------------------+
```

---

# 4. Use Case Diagram (Text-Based UML)

```
          +-------------------+
          |     Student       |
          +---------+---------+
                    |
                    | Browse Events
                    |
                    v
        +---------------------------+
        |     Event Catalog         |
        +---------------------------+

                    |
                    | Register for Event
                    |
                    v
        +---------------------------+
        |   Registration System     |
        +---------------------------+
                    |
                    | Receive Ticket
                    v
        +---------------------------+
        |    Ticket Generator       |
        +---------------------------+


          +-------------------+
          |   Organizer       |
          +---------+---------+
                    |
                    | Create / Edit Event
                    |
                    v
        +---------------------------+
        |   Organizer Dashboard     |
        +---------------------------+
```

---

# 5. Class Diagram (Simplified)

```
+---------------------+
|       Event         |
+---------------------+
| id                  |
| title               |
| date                |
| location            |
| description         |
+---------------------+
| +createEvent()      |
| +editEvent()        |
+---------------------+

+---------------------+
|       User          |
+---------------------+
| id                  |
| name                |
| email               |
| role                |
+---------------------+
| +register()         |
+---------------------+

+---------------------+
|    Registration     |
+---------------------+
| id                  |
| userId              |
| eventId             |
| ticketCode          |
+---------------------+
| +generateTicket()   |
+---------------------+
```

---

# 6. Sequence Diagram (Event Registration Flow)

```
Student -> Event Page: Open Event
Event Page -> Backend: Request Event Details
Backend -> Database: Fetch Event Data
Database -> Backend: Return Event Data
Backend -> Event Page: Display Details

Student -> Event Page: Click "Register"
Event Page -> Backend: Submit Registration
Backend -> Database: Save Registration
Backend -> Ticket Generator: Create Ticket
Ticket Generator -> Backend: Return Ticket Code
Backend -> Event Page: Show Confirmation
```

---

# 7. Data Model (ER Diagram in Markdown)

```
+-------------+        +------------------+        +------------------+
|   Users     |        |   Registrations  |        |     Events       |
+-------------+        +------------------+        +------------------+
| id (PK)     | 1    n | userId (FK)      | n    1 | id (PK)          |
| name        |--------| eventId (FK)     |--------| title            |
| email       |        | ticketCode       |        | date             |
| role        |        |                  |        | location         |
+-------------+        +------------------+        | description      |
                                                    +------------------+
```

---

# 8. System Modules

### **1. Event Module**
- create event  
- edit event  
- delete event  
- view event details  

### **2. Registration Module**
- register for event  
- validate registration  
- generate ticket  

### **3. Organizer Module**
- login (simple)  
- event management  
- attendee list  

### **4. Admin Module**
- manage roles  
- manage users  
- system settings (basic)

---

# 9. Updated WBS (Technical Focus)

### **1. Architecture & Modeling**
- define system layers  
- create UML diagrams  
- define data model  

### **2. Backend Development**
- event controller  
- registration controller  
- ticket generator  
- database integration  

### **3. Frontend Development**
- event catalog UI  
- event details UI  
- registration form  
- organizer dashboard  

### **4. Testing**
- unit tests  
- integration tests  
- UI testing  

---

# 10. Conclusion

Practice 5 provides the structural and modeling foundation for the **SFedU Student Event Portal**.  
It includes architecture descriptions, UML-style diagrams, data models, and module definitions.  
These artifacts prepare the project for detailed implementation planning in the next practices.
