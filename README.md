# 🧩 Header & Footer Architecture Guide

Welcome contributors! To keep our UI consistent and our user flow logical, we use different headers and footers depending on the user's authentication state (Logged In vs. Logged Out). 

This guide explains which header/footer components belong to which pages. Please review this before creating new views or updating navigation links!

---

## 📁 Component Location
All master templates for our headers and footers are located in the `Header & Footer/` directory:
* `Logged-Out-Header.html`
* `Logged-Out-Footer.html`
* `Logged-In-Header.html`
* `Logged-In-Footer.html`

---

## 🔓 1. Logged-Out State (Public Pages)
These components are for visitors who are not signed into the application. 
* **Header Focus:** Conversion (displays "Sign In" and "Sign Up" buttons).
* **Footer Focus:** General information, hiding internal app-specific tools.

**Components to use:**
* **Header:** `Logged-Out-Header.html`
* **Footer:** `Logged-Out-Footer.html`

**Files applying this state:**
* `index.html` (Landing Page)
* `sign_in.html`
* `sign_up.html`

---

## 🔒 2. Logged-In State (App Pages)
These components are for authenticated users who are actively managing their tasks.
* **Header Focus:** Core navigation (Dashboard, Tasks) and a "Log out" button.
* **Footer Focus:** Quick links to internal app features like "Mes Tâches" and "Équipe".

**Components to use:**
* **Header:** `Logged-In-Header.html`
* **Footer:** `Logged-In-Footer.html`

**Files applying this state:**
* `dashboard.html`
* `task_list.html`
* `CreateTask.html`
* `GroupMembers.html`

---

## 🎧 Special Case: `support.html`
The Support page is a hybrid. It needs to be accessible to both public visitors (e.g., someone who forgot their password) and active users. 

* **Static HTML Setup:** By default in this repository, `support.html` uses the **Logged-Out** header and footer so public visitors can navigate it seamlessly.
* **Future Dynamic Setup:** When a backend is integrated, the server should conditionally swap these components to the Logged-In versions if an active user session is detected. 

---

## 🛠️ Contribution Rules for Navigation
If you need to update a navigation link, change the logo, or add a new social media icon:
1. Make your changes in the respective template files inside the `Header & Footer/` folder first.
2. Copy and paste those updated blocks into the corresponding `.html` files listed above to keep everything synced.
