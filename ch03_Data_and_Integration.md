# Chapter 3: Data and Integration

## Introduction
Data and Integration in Pega enable applications to manage, transform, and validate business information. Business Architects define data models and configure integrations to ensure seamless communication between systems.

---

## Data Objects
Data objects represent reusable structures that define the information used in a case.

- **Examples**: Customer, Product, Address
- **Usage**: Referenced in case types to capture and display data

Data objects can be reused across multiple case types, promoting consistency and modularity.

---

## Data Relationships
Relationships define how data objects interact with each other.

- **One-to-One**: A customer has one address
- **One-to-Many**: A customer has many orders
- **Many-to-Many**: Students enrolled in multiple courses

These relationships help model real-world scenarios accurately.

---

## Data Pages
Data pages are the mechanism for loading data into the application.

- **Types**:
    - **Read-only**: For reference data
    - **Editable**: For user-modifiable data
- **Sources**:
    - Connector
    - Report Definition
    - Lookup

Data pages support caching and scope control (Thread, Requestor, Node).

---

## Calculated Values

Calculated values are derived fields based on other data inputs. They are defined using expressions or decision logic.

- **Examples**:
    - Total Price = Quantity × Unit Price
    - Age = Current Date − Date of Birth

Calculated values improve data accuracy and reduce manual entry. They can be configured in App Studio using expressions or decision tables.

---

## Validation Rules with Business Logic

Validation rules ensure data integrity by enforcing business constraints.

- **Types**:
    - Required fields
    - Format checks (e.g., email, phone)
    - Business logic (e.g., loan amount must be less than income × 5)

Validation can be applied at field level, step level, or case level. Use decision tables or expressions to define complex logic.

---

## Default Property Values

Default values pre-populate fields to streamline data entry and reduce errors.

- **Examples**:
    - Country = “Netherlands”
    - Priority = “Medium”
    - Date = Current Date
      Defaults can be set in the data model or via data transforms during case creation.

---

## Integration Overview
Integration allows Pega applications to communicate with external systems.

- **Connectors**: Outbound calls (e.g., REST, SOAP, SQL)
- **Services**: Inbound calls (e.g., exposing Pega as a REST endpoint)

Integrations are configured using Integration Designer in App Studio.

---

## Integration Designer
Integration Designer provides a visual interface to manage data sources and connections.

- **Features**:
    - View all data objects and their sources
    - Configure REST/SOAP connectors
    - Map fields between systems

It simplifies integration setup and maintenance.

---

## Data Transforms
Data transforms manipulate and map data between objects.

- **Use Cases**:
    - Copy data from one object to another
    - Set default values
    - Prepare data for display or submission

Data transforms are reusable and can be invoked in processes or actions.

---

## Summary
Data and Integration in Pega empower Business Architects to design robust, scalable applications. By leveraging data objects, relationships, validation, and integration tools, you can ensure that your application meets business needs while maintaining data integrity and performance.
