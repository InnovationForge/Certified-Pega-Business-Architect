# Chapter 4: Security

## Introduction
Security in Pega ensures that users access only the data and functionality appropriate to their roles. Business Architects play a key role in defining personas, access groups, and security rules that align with business requirements.

---

## Personas
Personas represent user roles and their associated responsibilities within the application.

- **Examples**:
    - Case Worker
    - Case Manager
    - Customer Service Representative
      Each persona is mapped to specific views, actions, and data access.

---

## Access Groups
Access groups define what parts of the application a user can access.

- **Components**:
    - Application
    - Roles
    - Portal
    - Default ruleset stack

Access groups are assigned to operators and determine their runtime experience.

---

## Authentication vs Authorization

Understanding the distinction between authentication and authorization is critical for designing secure applications.

- **Authentication**: Verifies the identity of a user.
    - Examples: Login credentials, SSO, OAuth
    - Managed via identity providers and login mechanisms

- **Authorization**: Determines what the authenticated user is allowed to do.
    - Examples: Access to case types, ability to approve requests
    - Controlled via roles, access groups, and privilege settings

In short:
- **Authentication = Who are you?**
- **Authorization = What can you do?**

Both must be configured correctly to ensure secure and compliant access.

---

## Role-Based Access
Roles define permissions for actions and data visibility.

- **Examples**:
    - Case Worker: Can create and update cases
    - Manager: Can view reports and approve cases

Roles are assigned within access groups and can be reused across applications.

---

## Security Best Practices
- Use personas to simplify role management
- Limit access to sensitive data using field-level security
- Apply least privilege principle to roles
- Regularly audit access groups and operator mappings

---

## Summary
Security in Pega is a layered approach involving personas, access groups, roles, and authentication mechanisms. Business Architects ensure that users have the right access to perform their tasks while maintaining data protection and compliance.

## Practice Scenarios

**Scenario: Role-Based Access for a Healthcare App**

In a healthcare app, the BA defines **personas** for Nurse, Doctor, and Admin. Each persona has a tailored portal. **Access groups** are configured to restrict sensitive data (e.g., only doctors can view diagnosis history). **Authentication** is handled via SSO, while **authorization** ensures only authorized users can approve prescriptions.

**Key Concepts**: Personas, access groups, authentication vs authorization

Here are **sample multiple-choice questions** for the **Security** chapter, aligned with the Certified Pega Business Architect 24.2 syllabus. These questions cover key concepts such as personas, access groups, roles, authentication vs authorization, and best practices.

---

## Practice Exam-Style Questions

### **Question 1**
What is the primary purpose of a persona in Pega?

A. To define access permissions  
B. To represent a user group with shared goals and UI needs  
C. To configure authentication methods  
D. To manage deployment environments

---

### **Question 2**
Which of the following best describes an access group?

A. A list of users assigned to a team  
B. A set of rules that define UI controls  
C. A configuration that determines application access, roles, and portals  
D. A tool for estimating development effort

---

### **Question 3**
Which statement best explains the difference between authentication and authorization?

A. Authentication defines what a user can do; authorization verifies identity  
B. Authentication verifies identity; authorization defines what a user can do  
C. Authentication and authorization are interchangeable terms  
D. Authentication is only used for external users

---

### **Question 4**
Which of the following is managed within an access group?

A. SLA definitions  
B. Application name and default portal  
C. Data page scope  
D. Case routing logic

---

### **Question 5**
What is the role of an access role in Pega?

A. To define the layout of a portal  
B. To determine which rules a user can execute  
C. To configure integration endpoints  
D. To manage case lifecycle stages

---

### **Question 6**
Which of the following is a best practice when configuring security for personas?

A. Assign all users the same access group for simplicity  
B. Use field-level security to restrict sensitive data  
C. Avoid using roles to manage permissions  
D. Allow unrestricted access during testing

---

### **Question 7**
Which configuration ensures that only managers can approve high-value cases?

A. Routing rule  
B. SLA escalation  
C. Access role with privilege  
D. Data transform

---

### **Question 8**
What does authentication typically involve in a Pega application?

A. Assigning access roles  
B. Verifying user identity through login or SSO  
C. Defining case types  
D. Configuring dashboards

---

## ✅ Answer Key with Explanations

| Question | Correct Answer | Explanation |
|----------|----------------|-------------|
| 1        | B. To represent a user group with shared goals and UI needs | Personas help define user experiences and expectations. |
| 2        | C. A configuration that determines application access, roles, and portals | Access groups control what users can access and how. |
| 3        | B. Authentication verifies identity; authorization defines what a user can do | This is the standard distinction between the two concepts. |
| 4        | B. Application name and default portal | Access groups include application, portal, and roles. |
| 5        | B. To determine which rules a user can execute | Access roles define rule-level permissions. |
| 6        | B. Use field-level security to restrict sensitive data | This ensures data protection and compliance. |
| 7        | C. Access role with privilege | Privileges within access roles control specific actions like approvals. |
| 8        | B. Verifying user identity through login or SSO | Authentication confirms the user's identity before granting access. |

---

Would you like me to generate similar question sets for the next chapter (e.g., User Experience)? I can also compile these into a printable quiz or interactive format.