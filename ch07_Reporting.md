# Chapter 7: Reporting

## Introduction
Reporting in Pega enables users to gain insights into case data, monitor performance, and support decision-making. Business Architects configure reports using App Studio to ensure stakeholders have access to relevant, real-time information.

---

## Insights
Insights are reusable, role-based reports that display key metrics and trends.

- **Use Cases**:
    - Track open cases by status
    - Monitor SLA compliance
    - View workload by operator

Insights can be embedded in dashboards and portals for easy access.

---

## Visualizations

Visualizations enhance the readability and impact of reports by presenting data graphically.

- **Types of Visualizations**:
    - **Tables**: Default format for listing records
    - **Bar Charts**: Compare values across categories
    - **Pie Charts**: Show proportions of a whole
    - **Line Charts**: Track trends over time

Choose the visualization type based on the story you want the data to tell.

---

## Filters

Filters allow users to narrow down report results based on specific criteria.

- **Examples**:
    - Show only cases with status = “Pending”
    - Filter by date range or assigned operator

Filters can be predefined or configured by users at runtime, improving report flexibility and relevance.

---

## Sorting

Sorting organizes report results in a meaningful order.

- **Examples**:
    - Sort by creation date (newest first)
    - Sort by priority or SLA deadline

Sorting helps users quickly identify the most important or urgent items in a report.

---

## Dashboards
Dashboards provide a consolidated view of multiple insights and widgets.

- **Use Cases**:
    - Manager dashboards showing team performance
    - Case worker dashboards with assigned tasks and KPIs

Dashboards can be customized per persona to align with role-specific needs.

---

## Summary
Reporting in Pega empowers users to make informed decisions through real-time insights, visualizations, and dashboards. By configuring filters, sorting, and visual formats, Business Architects ensure that reports are both actionable and user-friendly.

## Practice Scenarios

**Scenario: SLA Monitoring Dashboard**

A manager wants to monitor SLA compliance. The BA creates **Insights** showing overdue cases by department. **Filters** allow viewing by date range or case type. **Sorting** highlights the most delayed cases. **Visualizations** like bar charts and pie charts make trends easy to interpret.

**Key Concepts**: Insights, filters, sorting, visualizations

## Practice Exam-Style Questions


### **Question 1**
What is an Insight in Pega?

A. A tool for configuring integrations  
B. A reusable, role-based report that displays key metrics  
C. A rule that defines routing logic  
D. A portal layout configuration

---

### **Question 2**
Which visualization type is best suited for showing proportions of a whole?

A. Bar Chart  
B. Line Chart  
C. Pie Chart  
D. Table

---

### **Question 3**
What is the purpose of filters in Pega reports?

A. To change the report layout  
B. To restrict access to the report  
C. To narrow down report results based on specific criteria  
D. To define SLA escalation paths

---

### **Question 4**
Which sorting option would help a manager identify the most overdue cases?

A. Sort by case type  
B. Sort by operator name  
C. Sort by SLA deadline (ascending)  
D. Sort by creation date

---

### **Question 5**
What is the benefit of using dashboards in Pega?

A. They allow users to configure access groups  
B. They provide a consolidated view of multiple reports and widgets  
C. They automate deployment processes  
D. They validate data models

---

### **Question 6**
Which of the following is NOT a valid visualization format in Pega?

A. Table  
B. Pie Chart  
C. Gantt Chart  
D. Bar Chart

---

### **Question 7**
How can Business Architects ensure reports are relevant to different user roles?

A. By assigning reports to access groups  
B. By embedding Insights into persona-specific portals  
C. By configuring SLA rules  
D. By using data transforms

---

### **Question 8**
Which feature allows users to interact with reports by selecting criteria at runtime?

A. Static filters  
B. Dynamic filters  
C. SLA monitor  
D. Integration Designer

---

## ✅ Answer Key with Explanations

| Question | Correct Answer | Explanation |
|----------|----------------|-------------|
| 1        | B. A reusable, role-based report that displays key metrics | Insights are designed to provide tailored reporting for different roles. |
| 2        | C. Pie Chart | Pie charts are ideal for showing proportions of a whole. |
| 3        | C. To narrow down report results based on specific criteria | Filters help users focus on relevant data. |
| 4        | C. Sort by SLA deadline (ascending) | Sorting by SLA deadline helps identify cases nearing or past due. |
| 5        | B. They provide a consolidated view of multiple reports and widgets | Dashboards centralize reporting for quick access and decision-making. |
| 6        | C. Gantt Chart | Gantt charts are not a standard visualization format in Pega reporting. |
| 7        | B. By embedding Insights into persona-specific portals | This ensures users see reports relevant to their role. |
| 8        | B. Dynamic filters | Dynamic filters allow users to customize report views at runtime. |

