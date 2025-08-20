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

## Practice Scenarios

**Scenario: Loan Application System**

A bank needs a loan application system. The BA defines data objects like **Customer**, **Loan**, and **Credit Score**. A **calculated value** determines loan eligibility based on income and credit score. **Validation rules** ensure the loan amount doesn’t exceed 5× income. **Default values** like “Loan Type = Personal” are set. Integration with a credit bureau is configured using REST connectors.

**Key Concepts**: Data objects, calculated values, validation, default values, integration

Here are **sample multiple-choice questions** for the **Data and Integration** chapter, aligned with the Certified Pega Business Architect 24.2 syllabus. These questions cover key concepts such as data objects, relationships, data pages, transforms, validation, calculated values, and integration tools.

---

## Practice Exam-Style Questions

### **Question 1**
What is the primary purpose of a data object in Pega?

A. To define user roles  
B. To store reusable business data structures  
C. To configure routing rules  
D. To manage access groups

---

### **Question 2**
Which type of data relationship allows a customer to have multiple orders?

A. One-to-One  
B. One-to-Many  
C. Many-to-One  
D. Many-to-Many

---

### **Question 3**
Which scope level of a data page ensures that the data is shared across all users?

A. Thread  
B. Requestor  
C. Node  
D. Session

---

### **Question 4**
What is the role of a data transform in Pega?

A. To validate user input  
B. To route cases to operators  
C. To manipulate and map data between objects  
D. To define access roles

---

### **Question 5**
Which rule type is best suited for enforcing business logic validations?

A. Data Page  
B. Decision Table  
C. Data Transform  
D. Validation Rule

---

### **Question 6**
What is a calculated value?

A. A field that stores static data  
B. A field that derives its value from other fields using expressions  
C. A field used for routing decisions  
D. A field that defines access permissions

---

### **Question 7**
Which of the following is an example of a default property value?

A. Loan Amount = Income × 5  
B. Country = “Netherlands”  
C. SLA = 2 days  
D. Status = Resolved-Completed

---

### **Question 8**
Which integration tool in App Studio provides a visual interface to manage data sources?

A. Deployment Manager  
B. Integration Designer  
C. Estimator Tool  
D. Case Type Backlog

---

### **Question 9**
Which connector type would you use to retrieve data from an external REST API?

A. SOAP Connector  
B. SQL Connector  
C. REST Connector  
D. Email Listener

---

### **Question 10**
What is the benefit of using reusable data objects across case types?

A. Reduces UI complexity  
B. Improves security  
C. Promotes consistency and modularity  
D. Enhances SLA configuration

---

## ✅ Answer Key with Explanations

| Question | Correct Answer | Explanation |
|----------|----------------|-------------|
| 1        | B. To store reusable business data structures | Data objects define reusable entities like Customer or Product. |
| 2        | B. One-to-Many | A customer having multiple orders is a one-to-many relationship. |
| 3        | C. Node | Node scope shares data across all users on the same server node. |
| 4        | C. To manipulate and map data between objects | Data transforms are used to copy, set, or modify data. |
| 5        | D. Validation Rule | Validation rules enforce business logic constraints on data. |
| 6        | B. A field that derives its value from other fields using expressions | Calculated values are dynamically computed based on other inputs. |
| 7        | B. Country = “Netherlands” | Default values pre-populate fields to streamline data entry. |
| 8        | B. Integration Designer | Integration Designer visually manages data sources and connectors. |
| 9        | C. REST Connector | REST connectors are used to integrate with RESTful APIs. |
| 10       | C. Promotes consistency and modularity | Reusable data objects ensure consistent data modeling across cases. |

---

Would you like me to generate similar question sets for the next chapter (e.g., Security)? I can also compile these into a printable quiz or interactive format.