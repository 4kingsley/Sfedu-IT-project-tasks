# Practice 6. User Stories and Backlog Mapping  
## SFedU Student Event Portal

---

# 1. Introduction

The purpose of Practice 6 is to create **User Stories**, organize them into a **Product Backlog**, and map them to the Scrum sprints defined in Practice 4.  
User Stories describe the system from the perspective of its users and help structure development tasks.

This practice ensures that the project follows the Scrum methodology selected in Practice 3 and aligns with the schedule created in Practice 4.

---

# 2. User Story Format

All User Stories follow the standard template:

**As a _[user role]_, I want to _[goal]_, so that _[benefit]_.**

Each story includes **acceptance criteria** to define when it is considered complete.

---

# 3. User Stories

## **User Story 1 — Browse Events**
**As a** student  
**I want to** browse a list of upcoming SFedU events  
**So that** I can easily find events to attend  

**Acceptance Criteria:**
- events are displayed in a list  
- each event shows title, date, and location  
- list loads without errors  

---

## **User Story 2 — View Event Details**
**As a** student  
**I want to** open an event page  
**So that** I can read full event information  

**Acceptance Criteria:**
- event page shows description, date, time, location  
- page loads correctly  
- user can return to the event list  

---

## **User Story 3 — Register for an Event**
**As a** student  
**I want to** register for an event  
**So that** I can receive a digital ticket  

**Acceptance Criteria:**
- registration button is visible  
- system confirms registration  
- ticket is generated  

---

## **User Story 4 — Receive Digital Ticket**
**As a** student  
**I want to** receive a digital ticket after registration  
**So that** I can show it at the event  

**Acceptance Criteria:**
- ticket contains unique code  
- ticket is displayed or downloadable  
- ticket is linked to the correct event  

---

## **User Story 5 — Create Event**
**As a** staff organizer  
**I want to** create a new event  
**So that** students can register for it  

**Acceptance Criteria:**
- organizer can enter title, date, location, description  
- event is saved  
- event appears in the catalog  

---

## **User Story 6 — Edit Event**
**As a** staff organizer  
**I want to** edit event details  
**So that** I can update information if needed  

**Acceptance Criteria:**
- organizer can modify event fields  
- changes are saved  
- updated event is visible to students  

---

## **User Story 7 — View Attendee List**
**As a** staff organizer  
**I want to** see who registered for my event  
**So that** I can manage attendance  

**Acceptance Criteria:**
- attendee list shows student names  
- list updates automatically  
- only authorized organizers can view it  

---

## **User Story 8 — Manage Users**
**As an** administrator  
**I want to** manage user roles  
**So that** I can control access to organizer features  

**Acceptance Criteria:**
- admin can assign roles  
- admin can revoke roles  
- changes apply immediately  

---

# 4. Product Backlog (Ordered List)

| Priority | User Story | Description |
|----------|-------------|-------------|
| 1 | Browse Events | student views event list |
| 2 | View Event Details | student opens event page |
| 3 | Register for Event | student registers |
| 4 | Receive Ticket | ticket generation |
| 5 | Create Event | organizer creates event |
| 6 | Edit Event | organizer edits event |
| 7 | View Attendee List | organizer sees registrations |
| 8 | Manage Users | admin controls roles |

---

# 5. Sprint Mapping

Based on the schedule from Practice 4:

## **Sprint 1**
- User Story 1: Browse Events  
- User Story 2: View Event Details  

## **Sprint 2**
- User Story 3: Register for Event  
- User Story 4: Receive Ticket  

## **Sprint 3**
- User Story 5: Create Event  
- User Story 6: Edit Event  
- User Story 7: View Attendee List  

## **Sprint 4**
- User Story 8: Manage Users  
- UI polishing  
- Testing  
- Documentation  

---

# 6. Backlog Item Breakdown (Tasks)

### **User Story 1 — Browse Events**
- design event list UI  
- implement event list API  
- connect frontend to backend  
- test event list  

### **User Story 2 — View Event Details**
- design event detail page  
- implement event detail API  
- connect UI to backend  
- test event detail page  

### **User Story 3 — Register for Event**
- create registration form  
- implement registration logic  
- save registration to database  
- test registration flow  

### **User Story 4 — Receive Ticket**
- generate ticket code  
- display ticket to user  
- test ticket generation  

### **User Story 5 — Create Event**
- design event creation form  
- implement event creation API  
- validate event data  
- test event creation  

### **User Story 6 — Edit Event**
- design edit form  
- implement update logic  
- test event editing  

### **User Story 7 — View Attendee List**
- create attendee list UI  
- implement attendee list API  
- test attendee list  

### **User Story 8 — Manage Users**
- create admin panel  
- implement role assignment  
- test role management  

---

# 7. Conclusion

Practice 6 provides a complete set of **User Stories**, a structured **Product Backlog**, and a **Sprint Mapping** aligned with the Scrum methodology.  
This practice prepares the project for the final stage: creating the **Scrum Board and task distribution** in Practice 7.
