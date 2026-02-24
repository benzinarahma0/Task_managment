# 🧩 Task Management: Header & Footer Architecture Guide

Welcome to the **Task Management** repository! This project utilizes a modular UI architecture, employing specific header and footer configurations to manage the user experience across public and authenticated states.

## 🚀 Live Demo & Repository Walkthrough

You can explore the live application or view the guide below to understand the repository structure.

* **🌐 [Access the Live Project**](https://www.google.com/search?q=https://benzinarahma0.github.io/Task_managment/index.html)
* **📂 Repository Walkthrough:**

---

## 🔑 Getting Started: Testing the App

To experience the internal features of the application, use the following test credentials on the login page.

### 🛠️ Authentication Workflow

| Field | Credential |
| --- | --- |
| **Email** | `user@gmail.com` |
| **Password** | `user` |
| **Login Page** | **[Go to Sign In](https://www.google.com/search?q=https://benzinarahma0.github.io/Task_managment/sign_in.html)** |

---

## 🌐 Interface Overview

Use the links below to navigate directly to specific views of the application:

| Page | State | Component Focus | Direct Link |
| --- | --- | --- | --- |
| **Landing Page** | 🔓 Logged-Out | Conversion & "Sign Up" | **[Open](https://www.google.com/search?q=https://benzinarahma0.github.io/Task_managment/index.html)** |
| **Dashboard** | 🔒 Logged-In | Task Management & Navigation | **[Open](https://www.google.com/search?q=https://benzinarahma0.github.io/Task_managment/dashboard.html)** |
| **Task List** | 🔒 Logged-In | Detailed Task Overview | **[Open](https://www.google.com/search?q=https://benzinarahma0.github.io/Task_managment/task_list.html)** |
| **Support** | 🎧 Hybrid | Public Access & User Help | **[Open](https://www.google.com/search?q=https://benzinarahma0.github.io/Task_managment/support.html)** |
| **Create Task** | 🔒 Logged-In | Task Entry Form | **[Open](https://www.google.com/search?q=https://benzinarahma0.github.io/Task_managment/CreateTask.html)** |
| **Team Members** | 🔒 Logged-In | Collaborative Overview | **[Open](https://www.google.com/search?q=https://benzinarahma0.github.io/Task_managment/GroupMembers.html)** |

---

## 📁 Architecture & File Structure

Master templates for our headers and footers are centralized in the `Header & Footer/` directory.

### 🔓 1. Logged-Out State (Public Pages)

Used for visitors who are not yet signed in.

* **Header:** Focuses on conversion with "Sign In" and "Sign Up" buttons.
* **Footer:** Contains general site info and social links.
* **Target Files:** `index.html`, `sign_in.html`, `sign_up.html`.

### 🔒 2. Logged-In State (App Pages)

Used for authenticated users actively managing tasks.

* **Header:** Features core navigation (Dashboard, Tasks) and a "Log out" button.
* **Footer:** Provides quick access to internal tools like "Mes Tâches" and "Équipe."
* **Target Files:** `dashboard.html`, `task_list.html`, `CreateTask.html`, `GroupMembers.html`.

> [!TIP]
> **Support Page Hybridity**
> The **[Support Page](https://www.google.com/search?q=https://benzinarahma0.github.io/Task_managment/support.html)** currently defaults to the Logged-Out state. Future backend integrations will allow this page to dynamically detect session status and swap components accordingly.

---

## 🛠️ Contribution Guidelines

To ensure UI consistency across all pages, please follow these steps for any updates:

1. **Modify Templates:** First, update the files within the `Header & Footer/` directory.
2. **Sync Views:** Copy the updated HTML snippets into the respective pages listed in the architecture section.
3. **Validate Links:** Ensure all links maintain the `https://benzinarahma0.github.io/Task_managment/` root for consistency in the live environment.
