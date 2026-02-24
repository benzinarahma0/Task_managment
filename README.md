# 🧩 Task Management System

A modular task management web application built with structured Header & Footer architecture to handle Logged-In and Logged-Out states.

---

## 🌐 Live Demo

🔗 **Landing Page:**  
https://benzinarahma0.github.io/Task_managment/index.html  

🔐 **Login Page:**  
https://benzinarahma0.github.io/Task_managment/sign_in.html  

---

# 📥 How to Download the Project

Follow the steps shown below to download the repository:

<img src="./readme/Code%20Download.gif" width="800"/>

### Alternative Method (ZIP Download)

1. Click the green **Code** button
2. Select **Download ZIP**
3. Extract the folder
4. Open `index.html` in your browser

---

# 🔑 How to Access the Application

Use the following credentials to test the internal features:

| Field | Value |
|-------|-------|
| Email | `user@gmail.com` |
| Password | `user` |

<img src="./readme/Access_guide.jpg" width="800"/>

---

## 🌐 Interface Overview

Use the links below to navigate directly to specific views of the application:

| Page | State | Component Focus | Direct Link |
| --- | --- | --- | --- |
| **Landing Page** | 🔓 Logged-Out | Conversion & "Sign Up" | **[Open](https://benzinarahma0.github.io/Task_managment/index.html)** |
| **Dashboard** | 🔒 Logged-In | Task Management & Navigation | **[Open](https://benzinarahma0.github.io/Task_managment/dashboard.html)** |
| **Task List** | 🔒 Logged-In | Detailed Task Overview | **[Open](https://benzinarahma0.github.io/Task_managment/task_list.html)** |
| **Support** | 🎧 Hybrid | Public Access & User Help | **[Open](https://benzinarahma0.github.io/Task_managment/support.html)** |
| **Create Task** | 🔒 Logged-In | Task Entry Form | **[Open](https://benzinarahma0.github.io/Task_managment/CreateTask.html)** |
| **Team Members** | 🔒 Logged-In | Collaborative Overview | **[Open](https://benzinarahma0.github.io/Task_managment/GroupMembers.html)** |

---

# 🏗 Architecture Overview

All master UI templates are centralized inside:


## 🔓 Logged-Out State (Public Pages)

Used for:
- `index.html`
- `sign_in.html`
- `sign_up.html`

Includes:
- Conversion-focused header
- Public footer

---

## 🔒 Logged-In State (Application Pages)

Used for:
- `dashboard.html`
- `task_list.html`
- `CreateTask.html`
- `GroupMembers.html`

Includes:
- Application navigation header
- Internal tools footer

---

# 🛠 Contribution Guidelines

To maintain UI consistency:

1. Update templates inside `Header & Footer/`
2. Sync changes across related pages
3. Keep links using:


---

# 📌 Notes

- The Support page currently defaults to the Logged-Out state.
- Future backend integration can dynamically switch UI based on session state.

---

## 👩‍💻 Author

Developed as part of a modular front-end architecture project.
