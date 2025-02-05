# Software Requirements Specification for MotorPH Payroll System Expansion

### Prepared and Presented by:

Jomari Abejo  
Jasmin Pascual  
Lawrence Samuel Grefiel  

BSIT Major in Software Development and Network and Cybersecurity  
3rd Term, 2023-2024

---

## TABLE OF CONTENTS

- [Introduction](#introduction)
  - [Purpose](#purpose)
  - [Project Scope and Exclusions](#project-scope-and-exclusions)

- [Overall Description](#overall-description)
  - [Product Perspective](#product-perspective)
  - [User Needs](#user-needs)
  - [Assumptions and Dependencies](#assumptions-and-dependencies)

- [System Features and Requirements](#system-features-and-requirements)
  - [System Features](#system-features)
  - [Non-functional Requirements](#non-functional-requirements)

- [Conclusion](#conclusion)

- [Appendix](#appendix)
  - [Glossary](#glossary)
  - [Diagrams](#diagrams)

 
---

## Introduction

### Purpose

The purpose of creating the Software Requirements Specification (SRS) is to provide a comprehensive and detailed description of the payroll system. This document aims to ensure that the system meets the intended requirements, and serves as a reference for the development, maintenance, and enhancement of the system. The SRS covers both functional and non-functional requirements and includes sections on project scope, product perspective, user needs, assumptions, dependencies, system features, and non-functional requirements. Key stakeholders, such as project managers, developers, testers, and end-users, will use this document to understand and implement the system accurately.

### Project Scope and Exclusions

#### Scope

The updated payroll system aims to enhance employee management and payroll processing capabilities. The system will provide a user-friendly interface and includes features such as employee management, payroll calculation, leave management, reporting, and a self-service portal for employees. The primary objectives are to improve efficiency, accuracy, and compliance with regulatory requirements. This system supports the corporate goal of enhancing operational efficiency and employee satisfaction.

#### Exclusions

The payroll system does not extend to employee performance evaluations, goal setting, or other aspects of performance management. Additionally, integration with external third-party software, non-payroll HR functions such as recruitment, and multi-currency payroll processing are excluded from this system.

---

## Overall Description

### Product Perspective

The expanded payroll system offers a range of key features and functionalities to streamline payroll processing and employee management. It includes a secure employee login, automated payroll generation, comprehensive HR management, leave management, and a self-service portal for employees. These features enhance the overall efficiency and accuracy of operations. For example, the system's advanced reporting tools enable HR personnel to generate detailed payslips and payroll summaries effortlessly.

### User Needs

The payroll system addresses several key user needs:

#### Employees:
- **Self-Service Options:** Access electronic payslips, submit leave requests, and view personal information conveniently.
- **Clear Information Access:** Easily understand and access pay details, allowance breakdown, salary details, and leave balances.
- **User-Friendly Interface:** Navigate the system effortlessly for self-service tasks.

#### HR Administrators:
- **Employee Management:** Edit, view, and delete employee information as necessary to maintain accurate records and ensure compliance with company policies.
- **Leave Approval Management:** Streamline and automate the process of approving employee leave requests to ensure timely responses and compliance with company policies.
- **Dashboard for Leave Management:** Access a centralized dashboard to monitor leave balances, track employee absences, and forecast staffing needs effectively.
- **Timesheet Management:** Efficiently manage and track employee work hours and attendance through an integrated timesheet management module.

#### Payroll Administrators:
- **Accuracy and Compliance:** Ensure precise payroll calculations and compliance with labor laws.
- **Efficiency in Processing:** Streamline payroll processes to reduce manual errors and improve efficiency.
- **Payroll Dashboard:** Access a dashboard for monthly pay period management and monitoring.

#### IT Administrators:
- **Access Control:** Manage access levels and permissions for employees to ensure data security and regulatory compliance.
- **Password Management:** Facilitate secure password management and updates for employee accounts, ensuring robust cybersecurity practices across the payroll system infrastructure.

### Assumptions and Dependencies

#### Assumptions

- **User Adoption:** Users will efficiently adopt and adapt to the new system with adequate training and support.
- **Data Accuracy:** Users will enter accurate and up-to-date data into the system.
- **Security Measures:** Implemented security measures will safeguard sensitive payroll data.

#### Dependencies

- **Database Management System (DBMS):** The system's stability relies on the chosen DBMS (e.g., MySQL) for efficient data management.
- **Hardware Requirements:** Adequate hardware resources are essential for the system's performance and scalability.
- **Regulatory Updates:** The system must adapt to timely updates in legal or regulatory requirements, impacting functionalities and compliance measures.

---

## System Features and Requirements

### System Features

1. **Employee Login Functionality:** 
- Description: Provides a secure login mechanism for employees to access their profiles and personal information. Includes error handling for invalid login attempts and password recovery options.
- Mode of Operation: Includes normal operation and password recovery modes.
- User Class: Targets employee users for accessing personal information and IT administrators for managing security aspects.
- Object Class: Manages user credentials securely.
- Functional Hierarchy: Includes modules for authentication and session management.
   
   ![sucesslogin](https://github.com/user-attachments/assets/552542f0-d34b-4bb6-9aca-1e27668a52a6){:width="500px"}
   <small>Figure 1: Successful Login</small>

   ![forgotpassword](https://github.com/user-attachments/assets/aabced58-4299-43a4-b6fe-6d34fbee41a8){:width="500px"}
   <small>Figure 2: Submitting Forgot Password</small>

2. **Payroll Generation Capability:** 
- Description: Automates calculation and generation of employee payslips based on predefined rules and inputs. Allows administrators to review, edit, and distribute payslips.
- Mode of Operation: Includes processes for generating, editing, and distributing payslips securely.
- User Class: Targets payroll administrators for managing payslip generation and distribution.
- Object Class: Manages payroll data and rules for accurate calculation.
- Functional Hierarchy: Includes modules for payroll calculation, editing, and distribution.

   ![generatepay](https://github.com/user-attachments/assets/ec16e37c-3cce-4416-b626-1e211a674dda){:width="500px"}
   <small>Figure 3: Generating and Saving Payslips</small>

   ![editpayslip](https://github.com/user-attachments/assets/2e1065af-871a-44d0-a896-e26ff5cb0f23){:width="500px"}
   <small>Figure 4: Viewing and Editing Employee Payslips</small>

3. **HR Management Functions:**
- Description: Enables HR personnel to manage employee records, including adding, editing, viewing detailed information, and handling deletions.
- Mode of Operation: Includes secure operations for managing employee data.
- User Class: Targets HR administrators for managing employee information securely.
- Object Class: Manages employee data integrity and validation.
- Functional Hierarchy: Includes modules for employee data management and validation.

   ![addem](https://github.com/user-attachments/assets/c4ebbe15-ce8e-4136-bb14-45b1be2881df){:width="500px"}
   <small>Figure 5: Adding a new employee</small>

   ![editem](https://github.com/user-attachments/assets/23911efc-06cc-4655-bb41-ed152d000d81){:width="500px"}
   <small>Figure 6: Editing Employee Information</small>

   ![delete](https://github.com/user-attachments/assets/57286280-f9ea-4055-bc00-c1f6ee9fbad8){:width="500px"}
   <small>Figure 7: Viewing and Deleting Employee Information</small>
   
4. **Leave Management:**
- Description: Facilitates the process of leave request management, including approval, disapproval, viewing, and deletion of leave requests.
- Mode of Operation: Includes secure processes for managing leave requests and approvals.
- User Class: Targets HR personnel for managing leave requests efficiently.
- Object Class: Manages leave request data and approval workflows.
- Functional Hierarchy: Includes modules for leave request submission, approval, and tracking.

   ![last](https://github.com/user-attachments/assets/5239b9cf-d6cf-4505-901f-a355e32f4538){:width="500px"}
    <small>Figure 8: Filing Employee Leave</small>

   ![approve](https://github.com/user-attachments/assets/595a7434-025f-4dd7-8cdb-6e56f3e13c3a){:width="500px"}
   <small>Figure 9: Approving Leave Request</small>

   ![disap](https://github.com/user-attachments/assets/7b6cf2ca-f985-4a55-bd5c-8901228b0f03){:width="500px"}
   <small>Figure 10: Disapproving Leave Request</small>

   ![deleterequest](https://github.com/user-attachments/assets/d5912217-4186-4e1d-a434-457f412a8f40){:width="500px"}
   <small>Figure 11: Viewing and Deleting Leave Request</small>
   
5. **Employee Self-Service Portal:**
- Description: Provides employees with access to update their personal details, record attendance for each workday, submit requests for leave, and view detailed payslip information. Additionally, the portal offers a secure option for employees to change their login passwords.
- Mode of Operation: Includes processes for secure access and management of personal data.
- User Class: Targets employees for accessing and managing personal information securely.
- Object Class: Manages employee self-service data and transactions.
- Functional Hierarchy: Includes modules for personal information management, attendance recording, leave request submission, and payslip viewing.

   ![vieww](https://github.com/user-attachments/assets/aa9c6c01-9bba-4c25-8aa6-b0f30b2b43c7){:width="500px"}
   <small>Figure 12: Viewing Personal Information</small>

   ![changepass](https://github.com/user-attachments/assets/aee99097-fd6c-4aec-9321-9e6038c5c5ca){:width="500px"}
   <small>Figure 13: Changing Password</small>

   ![timeinn](https://github.com/user-attachments/assets/cb833416-520e-4844-bfc6-fc2a7854c23e){:width="500px"}
   <small>Figure 14: Recording Time in</small>

   ![timeoutt](https://github.com/user-attachments/assets/375394cb-0ef0-444d-9058-0f7c38bc4357){:width="500px"}
   <small>Figure 15: Recording Time out</small>

   ![submit](https://github.com/user-attachments/assets/c7333a69-5a20-45a6-90c6-d9ed43f0b6c1){:width="500px"}
   <small>Figure 16: Submitting Leave Request</small>

   ![viewp](https://github.com/user-attachments/assets/84659770-0d10-4723-81b3-777b3b403856){:width="500px"}
   <small>Figure 17: Viewing Payslip</small>

  
6. **Reporting Capabilities:**
- Description: Provides integrated analytics and reporting dashboards for payroll trends, attendance patterns, leave utilization, and other HR metrics.
- Mode of Operation: Includes processes for generating and presenting analytical insights securely.
- User Class: Targets HR administrators and management for data-driven decision-making.
- Object Class: Manages data aggregation and visualization for reporting purposes.
- Functional Hierarchy: Includes modules for report generation, data visualization, and dashboard presentation.
 
   ![generatepay](https://github.com/user-attachments/assets/ec16e37c-3cce-4416-b626-1e211a674dda){:width="500px"}
   <small>Figure 18: Generating Payslip Report</small>

   ![paydashboard](https://github.com/user-attachments/assets/4a2e7bf5-dcfd-42ad-a902-a4d58e1e99bb){:width="500px"}
   <small>Figure 19: Payroll Dashboard</small>

   ![dash](https://github.com/user-attachments/assets/ab3226aa-fe00-4b01-aed2-765128641791){:width="500px"}
   <small>Figure 20: HR Dashboard</small>

7. **System Administrator Functionalities:**
- Description: Provides tools for system administrators to manage user accounts, roles, permissions, and access levels across the platform. The system admin can also process verification codes for employees when they submit a forgot password request.
- Mode of Operation: Includes secure processes for user management and access control.
- User Class: Targets system administrators for managing platform-wide security and access policies.
- Object Class: Manages user accounts, roles, and permissions securely.
- Functional Hierarchy: Includes modules for user account management, role-based access control, and permission assignment.

   ![adduser](https://github.com/user-attachments/assets/217dbb05-357c-4916-8e2e-686d703b75bc){:width="500px"}
   <small>Figure 21: Adding a new user</small>

   ![shhs](https://github.com/user-attachments/assets/b37065fc-1eaa-46a1-ac8e-7570e96f014a){:width="500px"}
   <small>Figure 22: Editing user information and Resetting Password</small>

   ![vandd](https://github.com/user-attachments/assets/8d2dfe62-a594-490b-b51a-a472e3b644a4){:width="500px"}
   <small>Figure 23: Viewing and Deleting User</small>

   ![code](https://github.com/user-attachments/assets/0bcf8d23-89d7-4ef0-b7e5-953a60c97cf0){:width="500px"}
   <small>Figure 24: View Password Change Requests</small>


### Non-functional Requirements

- **Performance:** The system should handle multiple concurrent users without performance degradation, ensuring timely payroll processing and report generation.
   
- **Scalability:** The system should accommodate growing employee numbers and increased data volume.
   
- **Security:** Strong authentication, authorization mechanisms, and data encryption must protect sensitive information, ensuring compliance with data privacy regulations.
   
- **Usability:** An intuitive interface should require minimal training for end-users.
   
- **Reliability:** The system should have minimal downtime, ensuring continuous availability.
   
- **Maintainability:** Modular design facilitates easy maintenance and updates, supported by comprehensive documentation.
   
- **Compliance:** The system must adhere to relevant payroll regulations and standards.

---

## Conclusion
The MotorPH Payroll System Expansion represents a significant advancement in our organization's ability to manage payroll, HR functions, and employee self-service effectively. By addressing key user needs and incorporating robust features, the system enhances operational efficiency, accuracy, and compliance with regulatory requirements.

Throughout the development process, close collaboration among stakeholders—project managers, developers, testers, and end-users—has ensured that the system aligns closely with organizational goals and user expectations. As we conclude the MotorPH Payroll System project, ongoing feedback and iterative improvements have been crucial in refining the system and maximizing its benefits for all users. 

---

## Appendix

### Glossary

- **Authentication:** The process of verifying the identity of a user attempting to access the system.
- **Controller:** In MVC architecture, the component that handles user input and interacts with the model to update the view.
- **CRUD:** Create, Read, Update, Delete - basic operations performed on database records.
- **Deduction:** Amounts subtracted from an employee's gross salary, such as taxes and insurance contributions.
- **DBMS:** Database Management System, used for storing and managing data (e.g., MySQL).
- **Employee:** An individual who works for the organization and receives compensation.
- **Entity:** An object with a distinct identity, typically represented as a table in the database.
- **Frontend:** The user-facing part of the application, typically involving the user interface.
- **Gross Salary:** The total salary earned by an employee before deductions.
- **HR:** Human Resources, the department responsible for managing employee-related functions.
- **HR Dashboard:** A real-time dashboard for HR administrators displaying key HR metrics and visualizations.
- **IT Administrator:** A user role responsible for managing IT-related aspects of the system.
- **Inheritance:** A class-based programming concept where one class derives properties and behaviors from another class.
- **JavaFX:** A software platform used for creating and delivering desktop applications with a modern user interface.
- **Leave Request:** An employee's application for time off from work.
- **Model:** In MVC architecture, the component that represents the application's data and business logic.
- **MVC:** Model-View-Controller, a design pattern for organizing code in applications.
- **Net Salary:** The amount of salary received by an employee after deductions.
- **Pag-IBIG:** A government-mandated savings program in the Philippines.
- **PhilHealth:** The Philippine Health Insurance Corporation, providing health insurance to employees.
- **Payslip:** A document detailing an employee's earnings and deductions for a specific period.
- **Reporting Tools:** Software tools used to generate and manage reports.
- **Role:** A defined set of permissions that determines access levels and capabilities within the system.
- **Self-Service Portal:** A web-based interface that allows employees to manage personal information, submit leave requests, and view payslips.
- **Session Management:** The process of securely managing and maintaining user sessions within the application.
- **System Administrator:** A user role responsible for managing the overall operation and security of the system.
- **User Interface (UI):** The graphical layout and interactive elements of the application that users interact with.
- **User Management:** The process of managing user accounts, roles, and permissions within the system.

### Diagrams

### Use Case Diagram

[![UseCaseDiagram](https://github.com/Jasmin172002/documentation/assets/125138169/4db3b507-c970-4494-ade5-8b21aa7bc433)](https://github.com/Jasmin172002/documentation/assets/125138169/4db3b507-c970-4494-ade5-8b21aa7bc433)
<small>Figure 25: Use Case Diagram of the Expanded Payroll System</small>

The use case diagram illustrates the various interactions between different actors and the payroll system. Below is an explanation of the use case diagram components:

**Actors:**
- Employee: Interacts with personal account details, attendance records, payslip viewing, leave requests, and time tracking.
- Payroll Administrator: Manages payroll reports, payslip generation, and payroll summaries.
- IT Administrator: Handles system security and user role management.
- HR Administrator: Manages employee records, attendance, leave requests, and approvals.

**Use Cases:**
- Employee:
  - Time Tracking: Records time in and time out.
  - View Payslip: Access payslips by month or year.
  - View Leave Status: Check approved leave request status.
  - Login: Secure access to the system.
  - Manage Leave: View remaining leave credits and submit leave requests.

- IT Administrator:
  - Role Management: Administers role-based access control.
  - User Management: Manages user accounts.

- Payroll Administrator:
  - Generate Reports: Creates monthly payroll reports and summaries.
  - Generate Payslip: Calculates and saves employee payslips.

- HR Administrator:
  - Employee Management: Adds, modifies, and deletes employee records.
  - Attendance and Leave: Monitors attendance records and manages leave requests.

**Interactions:**
- All actors log in to access their respective functionalities.
- Generate Payslip involves computing allowances, deductions, and saving payslips.
- Role-Based Access Control ensures secure user access across the system.
- HR Administrator manages employee records, attendance, and leave requests.

### Class Diagram

[![AOOP_S2101 (3)](https://github.com/Jasmin172002/documentation/assets/125138169/6f12c90b-2fd4-47ce-8e9d-b4e0de974db1)](https://github.com/Jasmin172002/documentation/assets/125138169/6f12c90b-2fd4-47ce-8e9d-b4e0de974db1)
<small>Figure 26: Class Diagram of the Expanded Payroll System</small>

This class diagram illustrates the relationships and dependencies between key classes in the payroll system, defining how data flows and interacts within the system's architecture.

**Classes and Associations:**
- Employee
  - 1..* Department
  - 1..* Allowance
  - 1..1 Timesheet (Composition)
  - 1..* Payslip (Aggregation)
  - 1..1 User (Association)
  - 1..* Role (Aggregation)
  - 1..* LeaveRequest (Association)

- Allowance
  - 1..* Employee

- EmployeePayrollSummaryReport
  - 1..* Deduction (Composition)
  - 1..* Timesheet (Composition)
  - 1..1 Payslip (Aggregation)

- Tax
  - 1..1 TaxCategory (Association)

- Timesheet
  - 1..1 Employee

- Payslip
  - 1..* PayslipViewer (Association)
  - 1..* PayslipImpl (Inheritance)

- User
  - 1..1 Employee

- Role
  - 1..1 Permission (Aggregation)

- Position
  - 1..* Employee

- LeaveRequest
  - 1..1 LeaveRequestCategory (Association)

### Entity-relationship Diagram (ERD)

![Entity Relationship Diagram for MotorPH Payroll System drawio](https://github.com/Jasmin172002/AOOPSRS/assets/125138169/50ba213b-0766-4e13-9ec2-8b0a219c3d8d)
  <small>Figure 27: Entity-Relationship Diagram (ERD) of the Expanded Payroll System</small>

  The figure above represents the entity relationships for the payroll system. Below is the list of entities:

- Employee
- Allowance
- Deduction
- Payslip
- Tax
- Tax Category
- Leave Request
- Leave Request Category
- Position
- Timesheet
- User
- Role
- Permission
- Department

The relationships within the ERD outline the connections between different entities, defining how they interact and correlate with each other:

- Employee - Position:
  This one-to-many relationship ensures that each employee is associated with one or more positions within the organization, while each position can be occupied by multiple employees.

- Employee - Timesheet:
  In this one-to-many relationship, each employee can have multiple timesheet entries, but each timesheet entry is linked to only one employee, facilitating accurate tracking of work hours.

- Employee - Payslip:
  This one-to-many relationship allows each employee to have multiple payslips, with each payslip uniquely associated with one employee, streamlining payroll management.

- Employee - Allowance:
  The one-to-many relationship between employee and allowance permits each employee to have multiple allowances, ensuring flexible compensation options tailored to individual employee needs.

- Employee - Deduction:
  With a one-to-many relationship, each employee can have multiple deductions, while each deduction entry is linked to only one employee, simplifying payroll deductions.

- Employee - Leave Request:
  This one-to-many relationship enables each employee to submit multiple leave requests, ensuring efficient management of employee absences and vacation time.

- Employee - Department:
  In this one-to-one relationship, each employee is associated with only one department, ensuring clear organizational structure and hierarchy.

- Allowance - Payslip:
  The one-to-one relationship between payslip and allowance ensures that each payslip corresponds to a single total allowance amount, maintaining accuracy in payroll calculations.

- Payslip - Deduction:
  The one-to-one relationship between payslip and deduction ensures that each payslip corresponds to a single total deduction amount, maintaining accuracy in payroll calculations.

- Leave Request - Leave Request Category:
  This one-to-one relationship links each leave request to a specific category, facilitating proper categorization and management of employee leave requests.

- Employee - User:
  The one-to-one relationship between employee and user associates each employee with a unique user account, ensuring secure access to system resources.

- User - Role:
  In this one-to-one relationship, each user is linked to exactly one role, defining their permissions and access rights within the system.

- Role - Permission:
  With a one-to-many relationship, each role can have multiple permissions associated with it, allowing for flexible and granular control over system access and functionality.

With a focus on performance, scalability, security, usability, reliability, maintainability, and compliance, the MotorPH Payroll System Expansion is poised to support our organization's growth and operational excellence in the years to come.



