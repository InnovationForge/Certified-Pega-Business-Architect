## Scenario: Launching a New Employee Onboarding App

A multinational company is building an onboarding application using the Pega Platform. The app must interact with various systems (e.g., HR databases, training platforms, email services) and manage employee-related data such as personal details, training records, and access credentials. The BA is responsible for defining the data model and ensuring integrations are aligned with business needs.

---

## Data and Integration in Pega: Key Concepts and BA Engagement

### 1. **Data Objects**
- **Definition**: Reusable structures that represent business entities (e.g., Employee, Department).
- **In the Scenario**:
    - The BA defines a `Employee` data object with fields like name, ID, role, and start date.
    - Other data objects may include `TrainingModule`, `ITAsset`, and `HRDocument`.
- **BA's Role**:
    - Identify and model relevant data objects.
    - Ensure data objects are reusable across case types and Microjourneys.

---

### 2. **Data Relationships**
- **Definition**: Connections between data objects (e.g., one-to-many, many-to-one).
- **In the Scenario**:
    - An `Employee` may be linked to multiple `TrainingModules`.
    - A `Department` may have many `Employees`.
- **BA's Role**:
    - Define relationships to support reporting and logic.
    - Ensure relationships reflect real-world business rules.

---

### 3. **Data Sources**
- **Definition**: External systems or services from which Pega retrieves or sends data.
- **In the Scenario**:
    - HR system provides employee records.
    - LMS (Learning Management System) provides training modules.
    - Email service sends onboarding communications.
- **BA's Role**:
    - Identify required integrations.
    - Collaborate with system architects to define data source configurations.

---

### 4. **Data Views**
- **Definition**: Configurations that define how data is displayed and used in the UI.
- **In the Scenario**:
    - A view showing employee details during onboarding.
    - A view listing assigned training modules.
- **BA's Role**:
    - Design intuitive views for each persona.
    - Ensure views support decision-making and task completion.

---

### 5. **Integration Connectors**
- **Definition**: Mechanisms to connect Pega with external systems (e.g., REST, SOAP, JDBC).
- **In the Scenario**:
    - REST connector to fetch employee data from HR system.
    - Email connector to send welcome messages.
- **BA's Role**:
    - Define integration needs and expected data formats.
    - Validate that integrations support business processes.

---

### 6. **Data Transforms**
- **Definition**: Rules used to map, manipulate, or copy data between objects or systems.
- **In the Scenario**:
    - Transform data from HR system into the `Employee` data object.
    - Map training completion status from LMS to onboarding case.
- **BA's Role**:
    - Specify transformation logic during DCO sessions.
    - Ensure data is correctly structured for use in the application.

---

### 7. **Validation Rules**
- **Definition**: Rules that ensure data meets business requirements before processing.
- **In the Scenario**:
    - Validate that all required documents are uploaded.
    - Ensure start date is not in the past.
- **BA's Role**:
    - Define validation criteria based on business policies.
    - Collaborate with developers to implement rules in App Studio.

---

### 8. **Calculated Fields**
- **Definition**: Fields whose values are derived from other data.
- **In the Scenario**:
    - Calculate onboarding progress percentage.
    - Derive employee tenure based on start date.
- **BA's Role**:
    - Identify useful calculated metrics.
    - Ensure they support reporting and decision-making.

---

## Summary

In the Employee Onboarding App scenario, the Business Architect applies **Data and Integration** concepts to ensure the application can manage employee data effectively and interact with external systems. By defining data objects, relationships, views, and integrations, the BA ensures the solution is both functional and aligned with business needs.

Understanding how each Data and Integration concept fits into a real-world scenario is essential for success in the Certified Pega Business Architect exam. It demonstrates your ability to design data models and integration strategies that support scalable, efficient applications.

