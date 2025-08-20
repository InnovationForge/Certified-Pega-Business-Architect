## Scenario: Launching a New Employee Onboarding App

A multinational company is building an onboarding application using the Pega Platform. The goal is to automate and streamline the onboarding process for new hires. The BA is responsible for designing the case structure, defining stages and steps, and ensuring the case lifecycle supports business outcomes.

---

## Case Management in Pega: Key Concepts and BA Engagement

### 1. **Case Types**
- **Definition**: A case type represents a business transaction or process in Pega.
- **In the Scenario**: The BA defines a case type called `Employee Onboarding`.
- **BA's Role**:
    - Identify the purpose and outcome of the case.
    - Ensure the case type aligns with the Microjourney defined in the Discover phase.

---

### 2. **Stages and Steps**
- **Definition**: Stages represent major milestones; steps are tasks within each stage.
- **In the Scenario**:
    - Stages: Document Collection, Training Assignment, System Access, Welcome.
    - Steps: Upload documents, assign training, provision access, send welcome email.
- **BA's Role**:
    - Design the case lifecycle in App Studio.
    - Ensure each stage reflects a logical progression toward the onboarding goal.

---

### 3. **Processes**
- **Definition**: A process is a sequence of steps within a stage.
- **In the Scenario**:
    - The BA defines processes like “Verify Documents” and “Assign Training Modules.”
- **BA's Role**:
    - Configure processes using App Studio.
    - Ensure processes are reusable and follow best practices.

---

### 4. **Routing**
- **Definition**: Determines who performs each task in the case.
- **In the Scenario**:
    - Document verification routed to HR.
    - IT provisioning routed to IT support.
- **BA's Role**:
    - Define routing logic based on roles and work groups.
    - Use App Studio to configure assignments and queues.

---

### 5. **SLAs (Service Level Agreements)**
- **Definition**: Time-based goals for completing tasks or stages.
- **In the Scenario**:
    - SLA for document upload: 2 days.
    - SLA for system access provisioning: 1 day.
- **BA's Role**:
    - Set SLAs to ensure timely onboarding.
    - Monitor SLA compliance and adjust as needed.

---

### 6. **Child Cases**
- **Definition**: Sub-cases that support the parent case.
- **In the Scenario**:
    - Child case for IT provisioning.
    - Child case for benefits enrollment.
- **BA's Role**:
    - Identify when child cases are needed.
    - Configure relationships and dependencies between parent and child cases.

---

### 7. **Optional Actions**
- **Definition**: Actions that users can take outside the main case flow.
- **In the Scenario**:
    - HR can optionally resend the welcome email.
    - New hire can update contact details.
- **BA's Role**:
    - Define optional actions that enhance flexibility.
    - Ensure they are accessible and intuitive in the UI.

---

### 8. **Wait Steps**
- **Definition**: Pauses in the case until a condition is met.
- **In the Scenario**:
    - Wait for document upload before proceeding to training.
- **BA's Role**:
    - Use wait steps to control flow and dependencies.
    - Ensure business logic is respected.

---

### 9. **Case Status**
- **Definition**: Indicates the current state of the case.
- **In the Scenario**:
    - Statuses: “Pending Documents,” “Training In Progress,” “Completed.”
- **BA's Role**:
    - Define meaningful statuses for tracking and reporting.
    - Ensure status updates reflect real progress.

---

### 10. **Case Hierarchy and Reuse**
- **Definition**: Organizing cases for reuse and scalability.
- **In the Scenario**:
    - BA reuses components like training assignment across multiple onboarding types.
- **BA's Role**:
    - Promote reuse of processes and data objects.
    - Design scalable case structures.

---

## Summary

In the Employee Onboarding App scenario, the Business Architect applies **Case Management** principles to design a structured, efficient, and scalable onboarding process. By defining case types, stages, routing, SLAs, and optional actions, the BA ensures that the application meets business needs and delivers a smooth experience for all users.

Understanding how each Case Management concept fits into a real-world scenario is essential for success in the Certified Pega Business Architect exam. It demonstrates your ability to translate business requirements into functional case designs using the Pega Platform.

