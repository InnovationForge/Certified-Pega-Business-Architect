# **User Experience**
User Experience (UX) in Pega focuses on creating intuitive, role-based interfaces that support efficient task completion. This chapter guides you through grouping fields into views, configuring UI elements, and customizing portal content. You'll also explore how to control form appearance, visibility, and behavior using dynamic layouts and controls, ensuring a seamless experience across devices and personas.


## 🟨 **1. Group Fields to Create Views**

### ✅ Definition:
A **view** in Pega is a user interface layout that presents fields grouped logically to support a task or decision.

### ✅ Key Concepts:
- **Field Groups**: Organize related fields (e.g., Contact Info, Address).
- **Sections**: Visual containers for field groups.
- **Views**: Can be reused across case types and personas.

### ✅ Real-World Example:
In a customer onboarding case:
- View: “Customer Details”
    - Group: Personal Info → Name, DOB, Gender
    - Group: Contact Info → Email, Phone

### ✅ Best Practices:
- Group fields by **business meaning**, not just technical type.
- Keep views **clean and focused**—avoid clutter.
- Use **labels and instructions** to guide users.

---

## 🟨 **2. Add and Remove Fields in Views**

### ✅ How-To:
- Use **App Studio** to drag and drop fields into views.
- Fields can be added from:
    - Case type properties
    - Data objects
    - Calculated fields

### ✅ Removing Fields:
- Simply delete from the view layout.
- Does **not delete the property**—just removes it from the UI.

### ✅ Tip:
Use **preview mode** to test how the view looks for different personas and case statuses.

---

## 🟨 **3. Configure User Interface Elements and Portal Content**

### ✅ UI Elements:
- **Controls**: Input fields, dropdowns, buttons, checkboxes.
- **Layouts**: Dynamic layouts, grids, repeating structures.
- **Navigation**: Tabs, menus, breadcrumbs.

### ✅ Portal Content:
- **Portals** are role-based interfaces (e.g., User Portal, Manager Portal).
- Configure:
    - **Landing pages**
    - **Widgets** (e.g., My Worklist, Reports)
    - **Navigation menus**

### ✅ Real-World Example:
For a Claims Adjuster:
- Portal: Claims Portal
- Content: Dashboard with open claims, recent activity, and quick actions

### ✅ Best Practices:
- Tailor portals to **persona needs**.
- Keep navigation **simple and intuitive**.
- Use **responsive design** for mobile compatibility.

---

## 🟨 **4. Configure Form Appearance, Visibility Settings, and Controls**

### ✅ Form Appearance:
- Control layout using **dynamic layouts**.
- Use **headers, icons, and spacing** for clarity.
- Apply **styles** via skin rules (handled by UI team).

### ✅ Visibility Settings:
- Use **when rules** to show/hide fields based on conditions.
- Example: Show “Manager Comments” only if role = Manager.

### ✅ Controls:
- Choose appropriate controls for field types:
    - Text input for strings
    - Date picker for dates
    - Dropdown for predefined options
    - Checkbox for Boolean values

### ✅ Real-World Example:
In a loan application:
- “Collateral Details” section appears only if loan type = Secured
- “Loan Amount” uses a numeric input with validation

### ✅ Tips:
- Use **read-only controls** for review stages.
- Avoid overuse of conditional visibility—it can confuse users.
- Test forms across **personas and devices**.

---

## ✅ Summary Tips for Exam Success:

- Understand how **views** are built and reused across case types.
- Be able to **add/remove fields** and know the impact on data vs UI.
- Know how to configure **portals and UI elements** for different user roles.
- Be familiar with **visibility rules and control types** for dynamic forms.

---

Would you like a **visual mockup** of a sample portal layout or a **practice quiz** to reinforce these user experience concepts?