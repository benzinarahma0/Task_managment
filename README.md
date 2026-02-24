# 🧩 Task Management: Header & Footer Architecture Guide

Welcome contributors! To keep our UI consistent and our user flow logical, we use different headers and footers depending on the user's authentication state (Logged In vs. Logged Out).

---

## 📸 Project Preview

*This section will feature our AI-generated project concept image to give contributors a vision of the final goal.*

---

## 🚀 Getting Started & Tutorial

To get a copy of this project running on your local machine, follow the visual guide below:

### 🔑 Accessing the Dashboard

To test the application and access the **Logged-In** state features, use the following test credentials on the `sign_in.html` page:

| Field | Value |
| --- | --- |
| **Email** | `user@gmail.com` |
| **Password** | `user` |

---

## 🌐 Live Demo: Interface Overview

Explore the different views of the application below:

| Page | State | Component Focus |
| --- | --- | --- |
| **[Landing Page](https://www.google.com/search?q=index.html)** | 🔓 Logged-Out | Conversion & "Sign Up" |
| **[Dashboard](https://www.google.com/search?q=dashboard.html)** | 🔒 Logged-In | Task Management & Core Navigation |
| **[Task List](https://www.google.com/search?q=task_list.html)** | 🔒 Logged-In | Detailed Task Overview |
| **[Support](https://www.google.com/search?q=support.html)** | 🎧 Hybrid | Public Access & User Help |

---

## 📁 Component Location

All master templates for our headers and footers are located in the `Header & Footer/` directory:

* `Logged-Out-Header.html`
* `Logged-Out-Footer.html`
* `Logged-In-Header.html`
* `Logged-In-Footer.html`

---

## 🚦 Architecture States

### 🔓 1. Logged-Out State (Public Pages)

These components are for visitors who are not signed into the application.

* **Header Focus:** Conversion (displays "Sign In" and "Sign Up" buttons).
* **Footer Focus:** General information, hiding internal app-specific tools.

**Files applying this state:** `index.html`, `sign_in.html`, `sign_up.html`.

### 🔒 2. Logged-In State (App Pages)

These components are for authenticated users who are actively managing their tasks.

* **Header Focus:** Core navigation (Dashboard, Tasks) and a "Log out" button.
* **Footer Focus:** Quick links to internal app features like "Mes Tâches" and "Équipe".

**Files applying this state:** `dashboard.html`, `task_list.html`, `CreateTask.html`, `GroupMembers.html`.

---

## 🎧 Special Case: `support.html`

The Support page is a hybrid. It needs to be accessible to both public visitors and active users.

* **Current Setup:** Uses the **Logged-Out** components by default for seamless public navigation.
* **Future Plan:** Once a backend is integrated, the server will conditionally swap these components based on the active user session.

---

## 🛠️ Contribution Rules for Navigation

If you need to update a navigation link, change the logo, or add a new icon:

1. **Edit Templates:** Modify files inside the `Header & Footer/` folder first.
2. **Sync Views:** Copy and paste the updated blocks into the corresponding `.html` files to maintain consistency across the project.

---

**Would you like me to generate the actual AI image for the "Project Preview" section now?**
