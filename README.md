# Vacation-Tracking-System(VTS)

# Vision

Vacation Tracking System (VTS) is to make it easy for employees to manage their vacation, sick leave, and personal time off. The system will save time for both employees and the HR department. It will help employees take control of their time off, while reducing the workload of managers and HR staff.

---

# Function Requirements

- **Flexible rules-based system for validating**
    
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

# Domain

Vacation Tracking System (VTS) focuses on managing employee leave requests, including vacation, sick leave, and personal time off. It allows employees to request and track leave, while managers approve or reject requests. The system enforces company policies, integrates with HR systems, and ensures secure data handling. Automated notifications keep users informed, and the system is designed to be scalable, reliable, and user-friendly.

---

# Actor

- **Employee:** The main user of this system. An employee uses this system to
manage his or her vacation time.
- **Manager:** An employee who has all the abilities and goals of a regular employee,
 but with the added responsibility of approving vacation requests for immediate subordinates.
 A manager may award subordinates comp time, subject to certain limits set in the system.
- **Clerk:** A member of the HR department who has sufficient rights to view employees’ personal data and is responsible for ensuring that employees’ information in all HR systems is up to date and correct.
    - An HR clerk can add or remove nearly any record in the system.
- **System Admin:** A role responsible for the smooth running of the system’s technical 
resources (e.g., Web server, database) and for collecting and archiving all log files.

---

# Flowchart

### Create Request

![Flowchart](https://github.com/user-attachments/assets/03c41622-f979-4a2f-afd4-418507c4700f)


### Withdraw Request

![Flowchart](https://github.com/user-attachments/assets/3d0df5bb-7412-4d5e-a423-f585ead9062b)

### Cancel Approved Request

![Flowchart (1)](https://github.com/user-attachments/assets/08d7d55a-7be6-46bd-88d9-25c4c9133819)


---

# Sequence Diagram

### Create Request
![Sequence_diagram](https://github.com/user-attachments/assets/d9233f58-72a3-40eb-9394-2654cd6cb7d8)
