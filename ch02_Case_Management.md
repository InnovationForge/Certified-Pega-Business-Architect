# **Case Management**
Case Management is at the heart of Pega’s application design. It enables you to model business processes as structured workflows that reflect real-world scenarios. This chapter explores how to design case lifecycles, manage tasks, automate decisions, and handle exceptions like skipping stages or pausing cases. You'll also learn how to route work, configure SLAs, and enhance user interactions through optional actions and child cases.


## **1. Design a Case Lifecycle, Set Case Statuses, Add Instructions to Tasks**

### ✅ Definition:
A **case lifecycle** defines the stages and steps a case follows from creation to resolution.

### ✅ Key Concepts:
- **Stages**: Major milestones (e.g., "Intake", "Approval", "Resolution").
- **Steps**: Tasks within stages (e.g., "Collect Info", "Review Request").
- **Case Status**: Indicates progress (e.g., "New", "Pending-Approval", "Resolved-Completed").
- **Instructions**: Help users understand what to do at each step.

### ✅ Best Practices:
- Use **clear, business-friendly names** for stages and steps.
- Set **status updates** at key transition points.
- Add **instructions** to guide users, especially for manual tasks.

---

## **2. Add a Service Level Agreement (SLA); Configure Urgency, Goals, Deadlines, Passed Deadlines**

### ✅ Definition:
An **SLA** defines time expectations for completing tasks or cases.

### ✅ SLA Components:
- **Goal**: Ideal time to complete (e.g., 2 hours).
- **Deadline**: Maximum acceptable time (e.g., 4 hours).
- **Passed Deadline**: Time after the deadline (e.g., escalation).
- **Urgency**: Numeric value (0–100) that influences prioritization.

### ✅ Real-World Example:
For a customer complaint case:
- Goal: Respond within 1 day.
- Deadline: Resolve within 3 days.
- Passed Deadline: Notify manager.

### ✅ Tip:
Use **escalation actions** (e.g., reassign, notify) to handle missed deadlines.

---

## **3. Route Assignments to Users, Work Groups, Work Queues**

### ✅ Routing Options:
- **To a specific user**: Direct assignment.
- **To a work group**: Group of users with shared responsibilities.
- **To a work queue**: Tasks are placed in a queue for users to pick up.

### ✅ Best Practices:
- Use **skill-based routing** for specialized tasks.
- Use **round-robin or load balancing** for even distribution.
- Ensure **work queues** are monitored to avoid bottlenecks.

---

## **4. Configure and Send Email Correspondence**

### ✅ Use Cases:
- Notify users of case updates.
- Send confirmations to customers.
- Escalate issues to managers.

### ✅ Configuration:
- Use **correspondence rules**.
- Include **dynamic content** (e.g., case ID, status).
- Trigger emails on **events** (e.g., stage entry, SLA breach).

---

## **5. Identify Duplicate Cases**

### ✅ Purpose:
Prevent redundant work and ensure data integrity.

### ✅ Methods:
- Use **duplicate case search** based on key fields (e.g., email, ID).
- Configure **match rules** to define what constitutes a duplicate.

### ✅ Tip:
Prompt users with a warning or merge option when duplicates are found.

---

## **6. Identify and Add Optional Actions**

### ✅ Definition:
**Optional actions** are tasks users can perform outside the main flow.

### ✅ Examples:
- Update contact info.
- Add supporting documents.
- Request supervisor review.

### ✅ Configuration:
- Add as **case-wide actions** or **stage-specific actions**.

---

## **7. Add Optional Actions to a Workflow**

### ✅ Implementation:
- Use **optional processes** or **optional steps**.
- Display as buttons or links in the UI.

### ✅ Tip:
Ensure optional actions are **clearly labeled** and **accessible** without disrupting the main flow.

---

## **8. Automate Workflow Decisions Using Conditions**

### ✅ Use Cases:
- Route based on case data (e.g., loan amount).
- Skip steps if not applicable (e.g., no documents required).

### ✅ Tools:
- **When rules**: Boolean expressions.
- **Decision tables/trees**: Structured logic.
- **Conditions on stages/steps**: Control visibility and execution.

---

## **9. Pause and Resume Case Processing; Wait Steps**

### ✅ Purpose:
Handle scenarios where external input or time delay is needed.

### ✅ Wait Types:
- **Wait for time**: Pause for a set duration.
- **Wait for event**: Resume when a child case or external signal completes.

### ✅ Tip:
Use **wait steps** to model real-world delays (e.g., waiting for customer response).

---

## **10. Skip a Stage or Process**

### ✅ Use Case:
Skip unnecessary stages based on conditions (e.g., fast-track approvals).

### ✅ Configuration:
- Use **when conditions** on stages.
- Use **skip stage shape** in the flow.

---

## **11. Configure Child Cases**

### ✅ Definition:
**Child cases** are sub-processes that support the main case.

### ✅ Use Cases:
- Onboarding: Create child cases for equipment setup, training.
- Insurance: Create child cases for document verification.

### ✅ Configuration:
- Define **case hierarchy**.
- Use **case types** and **case relationships**.

---

## **12. Understand When to Use Automation Shapes**

### ✅ Automation Shapes:
- **Change Stage**
- **Update Case**
- **Send Email**
- **Create Case**
- **Post to Pulse**

### ✅ Use Cases:
- Automate transitions, notifications, and data updates.

### ✅ Tip:
Use automation shapes to **reduce manual effort** and **ensure consistency**.

---

## **13. Create and Manage Teams of Users**

### ✅ Teams in Pega:
- Defined by **work groups** and **roles**.
- Managed via **Access Groups** and **Operator IDs**.

### ✅ Best Practices:
- Align teams with **business functions**.
- Assign **roles and permissions** based on responsibilities.
- Use **team dashboards** for visibility.
