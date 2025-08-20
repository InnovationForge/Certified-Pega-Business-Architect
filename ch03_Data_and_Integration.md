# **Data and Integration**
Data is the foundation of any application, and Pega provides powerful tools to model, validate, and manipulate it. This chapter covers how to configure data objects and relationships, capture and present data through fields and views, and apply business logic for validation and calculations. You'll also learn how to use data transforms and default values to streamline data handling across your application.


## 🟨 **1. Configure Data Objects, Data Relationships, and Data Records**

### ✅ Definitions:
- **Data Object**: A reusable structure that defines a set of related fields (e.g., Customer, Product).
- **Data Relationship**: Defines how data objects relate to each other (e.g., one-to-many, one-to-one).
- **Data Record**: An instance of a data object (e.g., a specific customer).

### ✅ Key Concepts:
- Use **App Studio** to create and manage data objects.
- Define **relationships** to model real-world connections (e.g., a customer has multiple orders).
- Populate **data records** manually or via integration.

### ✅ Real-World Example:
In a retail app:
- Data Object: `Customer`
- Relationship: `Customer` → `Orders` (one-to-many)
- Data Record: John Doe with 3 orders

### ✅ Tip:
Use **reference data objects** to reuse data across multiple case types.

---

## 🟨 **2. Capture and Present Data; Fields, Field Types, and Views**

### ✅ Definitions:
- **Field**: A single piece of data (e.g., First Name).
- **Field Type**: Defines the kind of data (e.g., Text, Date, Boolean).
- **View**: A UI configuration that presents fields to users.

### ✅ Key Concepts:
- Use **App Studio** to add fields to data objects or case types.
- Choose appropriate **field types** to ensure data integrity.
- Configure **views** to control layout and visibility.

### ✅ Real-World Example:
In a loan application:
- Fields: Loan Amount (Decimal), Start Date (Date), Approved (Boolean)
- View: "Loan Details" section showing all fields

### ✅ Tip:
Use **dynamic views** to tailor the UI based on user roles or case status.

---

## 🟨 **3. Identify and Create Calculated Values**

### ✅ Definition:
**Calculated values** are fields whose values are derived from other fields using expressions or logic.

### ✅ Methods:
- Use **calculated fields** in data objects or case types.
- Use **expression builder** or **data transforms** to define logic.

### ✅ Real-World Example:
In an invoice case:
- `Total Amount` = `Quantity × Unit Price`
- Automatically updates when either field changes

### ✅ Tip:
Use **read-only calculated fields** to prevent manual overrides.

---

## 🟨 **4. Validate Data; Create and Configure Data Validation Rules Using Business Logic**

### ✅ Definition:
**Data validation** ensures that user input meets business requirements before processing.

### ✅ Methods:
- Use **edit validate rules** for format checks (e.g., email).
- Use **when rules** or **validation rules** for business logic (e.g., age > 18).
- Apply validations at **field level** or **case level**.

### ✅ Real-World Example:
In a registration form:
- Email must be valid format
- Date of birth must indicate age ≥ 18

### ✅ Tip:
Use **error messages** that are clear and actionable for users.

---

## 🟨 **5. Manipulate Application Data; Set Default Property Values, Configure Data Transforms**

### ✅ Definitions:
- **Default Property Values**: Predefined values assigned when a case or data object is created.
- **Data Transforms**: Rules that manipulate data (e.g., copy, set, map values).

### ✅ Use Cases:
- Set default status to "New" when a case is created.
- Use data transform to copy customer info from a parent case to a child case.

### ✅ Real-World Example:
In an onboarding case:
- Default role = "Employee"
- Data transform sets department based on location

### ✅ Tip:
Use **data transforms** during case creation, stage transitions, or integrations to ensure consistent data handling.

---

## ✅ Summary Tips for Exam Success:
- Understand **how data objects relate to case types** and how they support reuse.
- Be able to **identify the right field types** for different data needs.
- Know **where and how to apply validations** to enforce business rules.
- Practice **creating calculated fields and data transforms** in App Studio.
- Be familiar with **views and UI configurations** that present data effectively.

---

Would you like a **diagram of data relationships**, a **practice quiz**, or a **cheat sheet** summarizing these concepts for quick review?