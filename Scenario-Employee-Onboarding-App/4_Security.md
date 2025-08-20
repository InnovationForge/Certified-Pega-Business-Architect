## Scenario: Launching a New Employee Onboarding App

A multinational company is building an onboarding application using the Pega Platform. The app will be accessed by different types of users—new hires, HR managers, and IT support staff—each with specific responsibilities and access needs. The BA must ensure that the application enforces appropriate security controls to protect sensitive employee data and ensure users only access what they’re authorized to.

---

## Security in Pega: Key Concepts and BA Engagement

### 1. **Personas**
- **Definition**: Represent the roles of users interacting with the application.
- **In the Scenario**:
    - Personas include New Hire, HR Manager, IT Support.
- **BA's Role**:
    - Define personas during DCO sessions.
    - Use personas to guide UI design, access control, and routing logic.

---

### 2. **Operators**
- **Definition**: Individual user accounts used to log into the Pega application.
- **In the Scenario**:
    - Each HR Manager and IT Support staff member has an operator ID.
- **BA's Role**:
    - Understand how operators relate to personas.
    - Ensure that operator setup aligns with role-based access needs.

---

### 3. **Access Groups**
- **Definition**: Collections of roles and permissions assigned to operators.
- **In the Scenario**:
    - HR Managers belong to an access group that allows document review and approval.
    - IT Support belongs to an access group that allows provisioning tasks.
- **BA's Role**:
    - Collaborate with system architects to define access groups.
    - Ensure access groups reflect business responsibilities and security policies.

---

### 4. **Roles**
- **Definition**: Define what actions users can perform within the application.
- **In the Scenario**:
    - HR role includes viewing and editing employee data.
    - IT role includes accessing system provisioning tasks.
- **BA's Role**:
    - Map roles to personas and access groups.
    - Validate that roles support the intended user experience and security boundaries.

---

### 5. **Authentication**
- **Definition**: Verifying the identity of users before granting access.
- **In the Scenario**:
    - Users log in using corporate credentials (e.g., SSO or LDAP).
- **BA's Role**:
    - Ensure authentication methods meet organizational standards.
    - Confirm that sensitive onboarding data is protected from unauthorized access.

---

### 6. **Authorization**
- **Definition**: Controlling what authenticated users are allowed to do.
- **In the Scenario**:
    - HR Managers can approve documents, but cannot provision IT access.
    - New Hires can upload documents but cannot view internal HR notes.
- **BA's Role**:
    - Define authorization rules based on business logic.
    - Ensure that users only see and interact with data relevant to their role.

---

### 7. **Visibility Rules**
- **Definition**: Control what UI elements are shown to users based on context.
- **In the Scenario**:
    - New Hires see a simplified dashboard.
    - HR Managers see additional tabs for document verification.
- **BA's Role**:
    - Configure visibility rules in App Studio.
    - Ensure the UI is tailored to each persona’s needs and permissions.

---

### 8. **Data Privacy and Compliance**
- **Definition**: Ensuring sensitive data is handled according to legal and organizational policies.
- **In the Scenario**:
    - Employee personal data must be protected under GDPR or similar regulations.
- **BA's Role**:
    - Identify sensitive data fields.
    - Work with compliance teams to ensure proper handling and auditability.

---

## Summary

In the Employee Onboarding App scenario, the Business Architect applies **Security** concepts to ensure that users interact with the application safely and appropriately. By defining personas, access groups, roles, and visibility rules, the BA ensures that each user has the right level of access and that sensitive data is protected.

Understanding how these security concepts are implemented in Pega is essential for the Certified Pega Business Architect exam. It demonstrates your ability to design secure, role-based applications that meet both business and compliance requirements.

