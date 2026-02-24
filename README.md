

# 🧩 Task Management: Header & Footer Architecture Guide

Welcome to the **Task Management** repository! This project focuses on a modular UI approach, using distinct header and footer states to guide users seamlessly through their task management journey.

## 🚀 Live Demo & Repository Walkthrough

Experience the interface live or watch the guide on how to navigate this repository.

* **🌐 [View Live Demo**](https://benzinarahma0.github.io/Task_managment/)
* **📂 Repository Navigation Guide:**

---

## 🔑 Getting Started: How to Test

To access the internal application features and see the **Logged-In** state in action, use the following test credentials on the login page:

### 🛠️ Login Workflow

| Field | Credential |
| --- | --- |
| **Email** | `user@gmail.com` |
| **Password** | `user` |

---

## 🌐 Interface Overview

| Page | State | Component Focus | Link |
| --- | --- | --- | --- |
| **Landing Page** | 🔓 Logged-Out | Conversion & "Sign Up" | [Open](https://www.google.com/search?q=https://benzinarahma0.github.io/Task_managment/index.html) |
| **Dashboard** | 🔒 Logged-In | Task Management & Navigation | [Open](https://www.google.com/search?q=https://benzinarahma0.github.io/Task_managment/dashboard.html) |
| **Task List** | 🔒 Logged-In | Detailed Task Overview | [Open](https://www.google.com/search?q=https://benzinarahma0.github.io/Task_managment/task_list.html) |
| **Support** | 🎧 Hybrid | Public Access & User Help | [Open](https://www.google.com/search?q=https://benzinarahma0.github.io/Task_managment/support.html) |

---

## 📁 Architecture & File Structure

All master templates for our headers and footers are organized in the `Header & Footer/` directory to ensure reusability.

### 🔓 1. Logged-Out State (Public Pages)

Used for visitors who are not yet authenticated.

* **Header:** Displays "Sign In" and "Sign Up" buttons.
* **Footer:** General links and info; internal tools are hidden.
* **Applied to:** `index.html`, `sign_in.html`, `sign_up.html`.

### 🔒 2. Logged-In State (App Pages)

Used for authenticated users managing their workflow.

* **Header:** Features "Dashboard," "Tasks," and "Log out."
* **Footer:** Quick links to "Mes Tâches" and "Équipe."
* **Applied to:** `dashboard.html`, `task_list.html`, `CreateTask.html`, `GroupMembers.html`.

> [!NOTE]
> **Special Case: `support.html**`
> Currently uses the **Logged-Out** components by default. In a future backend update, these will dynamically swap based on the user's active session.

---

## 🛠️ Contribution Rules

To maintain UI consistency, follow these steps when updating navigation:

1. **Edit the Master:** Modify the files inside the `Header & Footer/` folder first.
2. **Sync the Views:** Copy and paste the updated HTML blocks into the corresponding pages (e.g., if you change the Logged-In header, update `dashboard.html` and `task_list.html`).
3. **Verify Links:** Ensure all relative paths remain functional across different directory levels.
