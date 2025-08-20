# Chapter 2: Case Management

## Introduction
Case Management in Pega enables organizations to model and automate business processes as structured workflows. It allows users to manage work through stages, steps, and rules that reflect real-world scenarios.

---

## Case Lifecycle
The case lifecycle defines the path a case follows from creation to resolution. It is composed of stages and steps that represent the business process.

- **Stages**: High-level phases of work (e.g., Intake, Review, Approval).
- **Steps**: Tasks or actions within each stage.

---

## Stages and Steps
Stages organize work into meaningful phases. Steps within stages can be:

- **Processes**: Groups of steps that execute together.
- **Single Steps**: Individual actions like collecting information or performing a decision.

---

## Automation Shapes

Automation shapes streamline case progression by executing predefined actions automatically. Common automation shapes include:

- **Change Stage**: Moves a case to a different stage based on conditions.
- **Change Case Status**: Updates the case status (e.g., from "Pending" to "Resolved").
- **Update Case**: Modifies data in the current or related case.
- **Create Case**: Instantiates a new child or peer case.
- **Post to Pulse**: Adds a message to the case's Pulse feed for collaboration.

These shapes reduce manual effort and ensure consistent behavior across cases.

---

## Skip Stage / Skip Process

Pega allows skipping stages or processes based on business logic or user input. This enhances flexibility in case flows.

- **Skip Stage**: Configured using conditions in the stage rule or via automation shapes.
- **Skip Process**: Applied within a stage to bypass specific steps or subprocesses.

Use cases include:
- Fast-tracking VIP customer requests.
- Bypassing approval for low-risk transactions.

Skipping logic should be clearly documented to ensure transparency and auditability.

---

## Wait Steps

Wait steps introduce pauses in case progression until a condition is met. They help synchronize with external events or dependencies.

Types of wait steps:
- **Wait for Time**: Delays case for a set duration.
- **Wait for Case**: Pauses until a child or related case reaches a specific status.
- **Wait for Event**: Triggers continuation based on a business event or signal.

Wait steps improve orchestration in complex workflows.

---

## Routing
Routing determines how assignments are delivered to users or work queues. Common routing options include:

- **To a specific user**
- **To a work queue**
- **Based on business logic or roles**

Routing ensures that work reaches the right person at the right time.

---

## Team Management

Team management defines how work is distributed among users and roles.

Key concepts:
- **Work Groups**: Logical collections of operators sharing responsibilities.
- **Work Queues**: Buckets of assignments routed to teams.
- **Team Roles**: Define access and responsibilities (e.g., Case Worker, Case Manager).
- **Skill-based Routing**: Assigns tasks based on user skills and availability.

Effective team setup ensures balanced workloads and faster case resolution.

---

## Case Hierarchy
Cases can be structured hierarchically to reflect dependencies and relationships.

- **Parent Case**: The main case that oversees related work.
- **Child Case**: A subprocess that supports the parent case.

---

## Child Case Configuration

Child cases can be created manually or automatically using automation shapes.

Key configuration options:
- **Create Automatically**: Triggered when a stage or step begins.
- **Create Manually**: Initiated by a user action.
- **Data Propagation**: Share data between parent and child using data transforms.
- **Status Synchronization**: Parent case can wait for child case completion using wait steps.

Proper child case design improves modularity and reuse across applications.

---

## Optional Actions
Optional actions allow users to perform tasks outside the standard case flow, such as:

- **Adding attachments**
- **Sending correspondence**
- **Escalating cases**

These actions enhance flexibility and user control.

---

## SLAs
Service Level Agreements (SLAs) define time expectations for completing assignments or resolving cases.

- **Goal**: Desired completion time.
- **Deadline**: Maximum allowable time.
- **Passed Deadline**: Escalation or notification triggers.

SLAs help maintain performance and accountability.

---

## Summary
Case Management in Pega provides a robust framework for modeling business processes. By leveraging stages, steps, routing, automation, and hierarchy, Business Architects can design scalable and efficient workflows that align with organizational goals.

## Practice Scenarios

**Scenario: Insurance Claim Processing**

An insurance provider wants to automate claim handling. The BA designs a case type with stages: **Intake**, **Assessment**, **Approval**, and **Resolution**. A **child case** is created for fraud investigation if flagged. **Automation shapes** like “Change Stage” and “Update Case” are used to streamline transitions. A **wait step** pauses the case until the fraud check completes. Routing is configured based on **team roles** and **skills**.

**Key Concepts**: Case lifecycle, child cases, automation shapes, routing, wait steps

Here are **sample multiple-choice questions** for the **Case Management** chapter, aligned with the Certified Pega Business Architect 24.2 syllabus. These questions cover key concepts such as case lifecycle, automation, routing, child cases, SLAs, and team management.

---

## Practice Exam-Style Questions

### **Question 1**
Which of the following best describes a stage in a Pega case lifecycle?

A. A single task performed by a user  
B. A reusable rule that defines data  
C. A high-level phase of work in a case  
D. A condition used to route assignments

---

### **Question 2**
What is the purpose of a wait step in a case flow?

A. To skip a stage based on business logic  
B. To pause case progression until a condition is met  
C. To route a case to a work queue  
D. To update a case status automatically

---

### **Question 3**
Which automation shape is used to change the status of a case?

A. Change Stage  
B. Update Case  
C. Change Case Status  
D. Post to Pulse

---

### **Question 4**
What is a child case typically used for?

A. To replace the parent case  
B. To perform a subprocess that supports the parent case  
C. To store user preferences  
D. To manage access groups

---

### **Question 5**
Which routing method assigns tasks based on user skills?

A. Route to Operator  
B. Route to Work Queue  
C. Route to Skill  
D. Route to Role

---

### **Question 6**
What does skipping a stage in a case lifecycle allow?

A. Repeating the same stage multiple times  
B. Bypassing unnecessary steps based on conditions  
C. Automatically resolving the case  
D. Creating a child case

---

### **Question 7**
Which of the following is NOT a valid use of a service level agreement (SLA)?

A. To define the goal and deadline for completing a task  
B. To route a case to a different user  
C. To trigger escalation when deadlines are missed  
D. To monitor performance against time expectations

---

### **Question 8**
What is the role of a work group in team management?

A. To define the portal layout  
B. To group related data objects  
C. To organize operators who share responsibilities  
D. To configure access roles

---

### **Question 9**
Which configuration allows a parent case to wait for a child case to complete?

A. Routing rule  
B. Wait step  
C. Data transform  
D. SLA escalation

---

### **Question 10**
What is the benefit of using automation shapes in a case flow?

A. They allow manual data entry  
B. They simplify UI design  
C. They reduce manual effort and enforce consistency  
D. They configure access groups

---

## ✅ Answer Key with Explanations

| Question | Correct Answer | Explanation |
|----------|----------------|-------------|
| 1        | C. A high-level phase of work in a case | Stages represent major phases in the case lifecycle. |
| 2        | B. To pause case progression until a condition is met | Wait steps delay case flow until a time/event/case condition is satisfied. |
| 3        | C. Change Case Status | This shape updates the status of a case automatically. |
| 4        | B. To perform a subprocess that supports the parent case | Child cases handle specific tasks that contribute to the parent case. |
| 5        | C. Route to Skill | Skill-based routing assigns tasks based on user capabilities. |
| 6        | B. Bypassing unnecessary steps based on conditions | Skip logic allows dynamic case progression. |
| 7        | B. To route a case to a different user | SLAs are for time-based tracking, not routing. |
| 8        | C. To organize operators who share responsibilities | Work groups help manage team assignments and queues. |
| 9        | B. Wait step | Wait steps can pause a parent case until a child case reaches a specific status. |
| 10       | C. They reduce manual effort and enforce consistency | Automation shapes streamline case behavior without user intervention. |

---

Would you like me to generate similar question sets for the next chapter (e.g., Data & Integration)? I can also compile these into a quiz format or printable study guide.
