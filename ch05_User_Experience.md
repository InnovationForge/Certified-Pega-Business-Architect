# Chapter 5: User Experience

## Introduction
User Experience (UX) in Pega focuses on designing intuitive, efficient, and role-based interfaces that support business processes. Business Architects define views, controls, and navigation patterns that align with user needs.

---

## Views
Views define how data is presented to users within a case.

- **Types of Views**:
    - **Collect Information**: Used to gather input from users.
    - **Display Information**: Shows read-only data.
    - **Confirm**: Summarizes data before submission.

Views are configured in App Studio and can be reused across case types.

---

## UI Controls
UI controls are the building blocks of views. They determine how users interact with data.

- **Examples**:
    - Text Input
    - Dropdown
    - Date Picker
    - Checkbox
    - Radio Button

Controls can be configured with validation, visibility, and formatting options.

---

## Control Types

Control types define the behavior and appearance of UI elements. Choosing the right control enhances usability and data accuracy.

- **Text Input**: For free-form text
- **Dropdown**: For selecting from predefined options
- **Checkbox**: For binary choices
- **Radio Button**: For mutually exclusive selections
- **Autocomplete**: For dynamic search and selection
  Use control types that match the data context and user expectations.

---

## Visibility Settings

Visibility settings determine when and how UI elements appear based on conditions.

- **Types**:
    - Always visible
    - Condition-based (e.g., show if status = “Pending”)
    - Role-based (e.g., visible only to managers)

Visibility improves clarity and reduces cognitive load by showing only relevant information.

---

## Portal Configuration
Portals define the overall layout and navigation experience for users.

- **Types of Portals**:
    - **User Portal**: For case workers and managers
    - **Admin Portal**: For system administrators
    - **Custom Portals**: Tailored to specific personas
      Portals include navigation menus, dashboards, and widgets. Business Architects configure portals in App Studio to align with user roles and workflows.

---

## UX Best Practices
- Keep interfaces clean and focused
- Use consistent labels and formatting
- Group related fields logically
- Minimize clicks and scrolling
- Test with real users for feedback

---

## Summary
User Experience in Pega is about designing interfaces that support business goals and user needs. By leveraging views, controls, visibility settings, and portals, Business Architects can create applications that are both functional and user-friendly.
