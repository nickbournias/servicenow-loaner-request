# Loaner Request App (ServiceNow)

## 📋 Overview

The **Loaner Request App** is a custom-built ServiceNow application designed to streamline the process of requesting and managing loaner equipment within an organization. Built as part of a Certified Application Developer (CAD) lab, this app demonstrates end-to-end development on the Now Platform, including form design, workflow automation, user access control, and UI enhancements.

---

## 🚀 Features

- ✅ **Submit Loan Requests**  
  End users can request laptops, monitors, or other equipment through a simple form.

- 🔄 **Approval Workflow**  
  Requests trigger an automated workflow that routes approvals to designated approvers.

- 📦 **Inventory Visibility**  
  Loaner items are tracked to ensure availability and prevent conflicts.

- ⏰ **Due Date Tracking**  
  Request forms include expected return dates, with optional reminders and escalation.

- 📊 **Reporting Dashboard (optional)**  
  Visualize outstanding, approved, and returned loaners using Performance Analytics widgets or reports.

---

## 🧱 Architecture

| Component             | Description                                        |
|-----------------------|----------------------------------------------------|
| **Table**             | `x_loanr_request` – Stores request records         |
| **Catalog Item**      | Loaner Request – Form for end-user submissions     |
| **Flow / Workflow**   | Approval flow for manager and/or IT review         |
| **Notifications**     | Alerts for approvals, rejections, and returns      |
| **ACLs / Roles**      | `loaner_user`, `loaner_admin` for access control   |
| **Script Includes**   | Utility functions for request validation (if used) |
| **UI Policy / Scripts** | Enhance form experience (e.g., field visibility)  |

---

## 🛠️ Setup & Configuration

1. **Clone the App (if using Source Control)**  
   - Go to **Studio → Source Control → Link to Source Control**
   - Use your Git URL and credentials
   - Choose `Load Application` after linking

2. **Create Loaner Items (Optional Seed Data)**  
   - Navigate to **Loaner Inventory** (if implemented)
   - Create items like "Dell Laptop", "MacBook Pro", etc.

3. **Assign Roles**  
   - `loaner_user`: Can submit requests  
   - `loaner_admin`: Can approve, manage inventory

4. **Test the Workflow**  
   - Submit a new request  
   - Log in as approver and complete approval/rejection  
   - Return and mark items as complete

---

## 📚 Tech Used

- **ServiceNow App Engine**
- **Flow Designer / Workflow Editor**
- **Form Designer**
- **ACLs, Roles, Notifications**
- **Studio and Source Control (Git)**

---

## 📄 License

This app was developed for educational and demonstration purposes as part of a ServiceNow Certified Application Developer course. Reuse and modification are permitted with attribution.


