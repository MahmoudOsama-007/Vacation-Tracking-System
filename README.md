# Vacation Tracking System(VTS)
# Index
- [**Vision**](#vision)
- [**Domain**](#domain)
- [**Actors**](#actors)
- [**Requirements**](#requirements)
  - [Function Requirements](#function-requirements)
  - [Non-Function Requirement](#non-function-requirement)
  - [Constraints](#constraints)
- [**Flowcharts**](#flowcharts)
- [**Sequence Diagrams**](#sequence-diagrams)
- [**State Machine Diagrams**](#state-machine-diagrams)
  - [Vacation Request State](#vacation-request-state)
- [**Data Model**](#data-mode)


# Vision

Vacation Tracking System (VTS) is to make it easy for employees to manage their vacation, sick leave, and personal time off. The system will save time for both employees and the HR department. It will help employees take control of their time off, while reducing the workload of managers and HR staff.
---

# Domain

Vacation Tracking System (VTS) focuses on managing employee vacation requests, including vacation, sick leave, and personal time off. It allows employees to request and track vacation, while managers approve or reject requests.

---
# Actors

- **Employee:** The main user of this system. An employee uses this system to
manage his or her vacation time.
- **Manager:** An employee who has all the abilities and goals of a regular employee,
 but with the added responsibility of approving vacation requests for immediate subordinates.
 A manager may award subordinates comp time, subject to certain limits set in the system.
- **Clerk:** A member of the HR department who has sufficient rights to view employees’ personal data and is responsible for ensuring that employees’ information in all HR systems is up to date and correct.
- **System Admin:** A role responsible for the smooth running of the system’s technical 
resources (e.g., Web server, database) and for collecting and archiving all log files.

---

# Function Requirements

- **Flexible rules-based system for validating:**
    
    Ensures requests are validated according to predefined rules and criteria before approval.
    
- **Manager approval (optional) :**
    
    Managers can approve or reject leave requests, with this option being flexible depending on the organization’s needs.
    
- **Access Requests :**
    
    Employees can view requests from the previous calendar year, and allows requests to be made up to a year and a half in the future
    
- **E-mail notification:**
    
    Notifies managers for approval requests and employees about the status of their leave requests.
    
- **Intranet portal integration :**
    
    The system is implemented as an extension to the existing intranet portal, using the portal’s single sign-on for authentication.
    
- **Activity logs :**
    
    All transactions are logged for auditing and tracking purposes.
    
- **Override capabilities for HR and system administration :**
    
    HR and system administrators can override restrictions and rules, with all actions logged
    
- **award of personal leave time:**
    
    Managers can directly assign personal leave within system-set limits.
    
- **HR department legacy systems :**
    
    Integrates with HR legacy systems to retrieve necessary employee information and handle updates.
    

---

# Non-Function Requirement

- **Performance**
    - The system should handle up to 500 concurrent users without significant performance degradation.
    - Requests for leave validation and manager approval should be processed within 2 seconds.
- **Scalability**
    - The system should be scalable to support an increasing number of employees as the company grows.
    - It should be able to handle a 50% increase in users without requiring significant infrastructure changes.
- **Security**
    - All employee data should be encrypted both in transit and at rest.
- **Availability**
    - The system should have 99.9% uptime, excluding scheduled maintenance periods.
    - Any downtime should be communicated to users in advance, and issues should be resolved within 4 hours.

---
# Constraints

- Uses existing hardware and middleware
- Deal with existing intranet portal system, and uses the portal’s single-sign-on mechanisms for all authentication

---

# Flowcharts

### Create Request

![image](https://github.com/user-attachments/assets/3088a0a4-c9e2-4dbb-851a-dee3a172b0c5)

### Withdraw Request

![image](https://github.com/user-attachments/assets/44567a51-da7b-41d8-95cc-0ca795f7132e)

### Cancel Approved Request

![image](https://github.com/user-attachments/assets/c2081073-15a0-4bc6-90a4-e0c3b98e0ee2)


### Edit Pending Request

![image](https://github.com/user-attachments/assets/74d141ef-ac17-475e-9737-6c2332c480a0)

---

# Sequence Diagram
## create Request
  ![Sequence diagram](https://github.com/user-attachments/assets/8a7b8ae6-22a0-48b8-bc72-a5ce940dbe50)


---

# Data Mode
![image](https://github.com/user-attachments/assets/a9381ef1-6559-49ef-a553-eb59c6ecd01c)

---
# State Machine Diagrams
## Vacation Request State
![image](https://github.com/user-attachments/assets/122c522a-8789-466b-8805-def25c080b59)


