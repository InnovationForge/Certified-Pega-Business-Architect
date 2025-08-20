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
