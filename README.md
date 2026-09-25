<div align="center">
                       
# 📝 To-Do List Application
### **One task at a time. One step closer to your goals.**
A modern, responsive, and lightweight **task management web application** built with **HTML5, CSS3, and Vanilla JavaScript**.
Create, organize, update, complete, filter, and delete tasks directly from your browser — with **persistent LocalStorage support and zero backend setup**.

<p>
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/JavaScript-ES6%2B-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/Storage-LocalStorage-orange?style=for-the-badge" alt="LocalStorage">
</p>

<p>
  <img src="https://img.shields.io/badge/Backend-None-lightgrey?style=flat-square" alt="Backend">
  <img src="https://img.shields.io/badge/Database-None-lightgrey?style=flat-square" alt="Database">
  <img src="https://img.shields.io/badge/Framework-None-lightgrey?style=flat-square" alt="Framework">
  <img src="https://img.shields.io/badge/Status-Completed-success?style=flat-square" alt="Status">
</p>

**[Features](#-features) • [Architecture](#-architecture) • [Setup](#-getting-started) • [Usage](#-usage) • [Screenshots](#-screenshots) • [Roadmap](#-future-improvements)**

</div>

---

# 📌 Overview

The **To-Do List Application** is a client-side task management system designed to make everyday task tracking **simple, fast, and distraction-free**.

The application provides the essential tools required to manage tasks from a single interface:

* ➕ Create new tasks
* 📝 Add optional descriptions
* ✏️ Edit existing tasks
* ✅ Mark tasks as completed
* 🗑️ Delete tasks
* 🔎 Filter tasks by status
* 💾 Persist tasks across browser sessions
* 📱 Use the application across desktop, tablet, and mobile devices

The entire application runs inside the browser, making it lightweight, easy to understand, and simple to deploy.

---

# 🎯 Core Principles

| Principle              | Description                                               |
| ---------------------- | --------------------------------------------------------- |
| 🎯 **Simplicity**      | Keep task management straightforward and clutter-free     |
| ⚡ **Efficiency**       | Perform common actions with minimal interaction           |
| 📱 **Responsiveness**  | Maintain usability across different screen sizes          |
| 💾 **Persistence**     | Preserve tasks using browser-based LocalStorage           |
| 🧩 **Maintainability** | Keep the frontend structure simple and easy to understand |

---

# ✨ Features

## 📋 Task Management

| Feature              | Description                                        |
| -------------------- | -------------------------------------------------- |
| ➕ **Create Task**    | Add a task with a title and optional description   |
| ✏️ **Edit Task**     | Modify an existing task's information              |
| ✅ **Complete Task**  | Toggle tasks between active and completed states   |
| 🗑️ **Delete Task**  | Permanently remove unwanted tasks                  |
| 📋 **Task Overview** | View and manage tasks from a centralized interface |

---

## 🔎 Task Filtering

Quickly switch between different task states:

* **All** — Display every task
* **Active** — Display pending tasks
* **Completed** — Display finished tasks

This allows users to focus on the tasks that matter at any given moment.

---

## 💾 Persistent Storage

Task data is stored using the browser's **LocalStorage API**.

Tasks remain available after:

* 🔄 Refreshing the page
* 🌐 Closing and reopening the browser
* 🔁 Returning to the application later

> **⚠️ Important:** LocalStorage is browser/device-specific. Tasks are not automatically synchronized between different browsers or devices.

---

## 📱 Responsive Interface

The application is designed to work across:

**🖥️ Desktop · 💻 Laptop · 📱 Tablet · 📲 Mobile**

Responsive layouts, spacing, typography, and controls adapt to different viewport sizes while maintaining usability.

---

## ⚡ Lightweight Architecture

The application intentionally avoids unnecessary dependencies.

| Component          | Included? |
| ------------------ | --------- |
| Backend            | ❌         |
| Database           | ❌         |
| Frontend Framework | ❌         |
| Build System       | ❌         |
| External Runtime   | ❌         |
| HTML5              | ✅         |
| CSS3               | ✅         |
| Vanilla JavaScript | ✅         |
| LocalStorage       | ✅         |

> **Result:** A simple, lightweight application that can run directly in a modern browser.

---

# 🛠️ Technical Highlights

The project demonstrates practical frontend development concepts:

* 🧩 Modular frontend organization
* 🔄 CRUD-style task operations
* 🧠 Client-side state management
* 🌐 Dynamic DOM manipulation
* ⚡ Event-driven programming
* 💾 LocalStorage integration
* 🔄 JSON serialization and deserialization
* 🎨 Conditional rendering
* 🔎 Status-based filtering
* ✅ Form validation
* 📱 Responsive CSS
* 🔄 Real-time UI updates
* 💾 Browser-based persistence
* 📲 Mobile-friendly interface

---

# 🧰 Technology Stack

| Technology           | Purpose                                                         |
| -------------------- | --------------------------------------------------------------- |
| **HTML5**            | Semantic structure and application markup                       |
| **CSS3**             | Styling, layout, responsiveness, and visual presentation        |
| **JavaScript ES6+**  | Application logic, state handling, DOM manipulation, and events |
| **LocalStorage API** | Persistent client-side task storage                             |

---

## 💡 Why Vanilla JavaScript?

This project intentionally uses **Vanilla JavaScript instead of a frontend framework** to demonstrate a strong understanding of fundamental web development concepts.

The project provides hands-on experience with:

* DOM manipulation
* Event handling
* JavaScript state management
* Browser APIs
* CRUD operations
* JSON data handling
* Client-side persistence
* Conditional rendering

This makes the project particularly useful for understanding how modern frontend frameworks work underneath the abstraction layer.

---

# 🏗️ Architecture

The application follows a simple **client-side architecture**:

```text
                    ┌──────────────────────┐
                    │     User Interface   │
                    │       HTML + CSS     │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │ JavaScript Application│
                    │        Logic         │
                    └──────────┬───────────┘
                               │
              ┌────────────────┼────────────────┐
              │                │                │
              ▼                ▼                ▼
        Create Task       Update Task       Delete Task
              │                │                │
              └────────────────┼────────────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │    Task Filtering    │
                    │ Active / Completed   │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │   LocalStorage API   │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │   Browser Storage    │
                    └──────────────────────┘
```

### Architecture Characteristics

* Client-side only
* No server communication
* Browser-based persistence
* Event-driven interactions
* Dynamic DOM updates
* Simple application state flow

---

# 🔄 Application Workflow

```text
                 ┌───────────────┐
                 │    Open App   │
                 └───────┬───────┘
                         │
                         ▼
                 ┌─────────────────┐
                 │ Load LocalStorage│
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │ Render Task List│
                 └────────┬────────┘
                          │
             ┌────────────┼────────────┐
             ▼            ▼            ▼
       Create Task    Edit Task    Delete Task
             │            │            │
             └────────────┼────────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │ Update App State│
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │ Save Task Data  │
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │    Update UI    │
                 └─────────────────┘
```

---

# 💾 Data Persistence

The application stores task information directly inside the user's browser using **LocalStorage**.

## Persistence Flow

```text
User Action
     │
     ▼
Application State
     │
     ▼
Serialize Task Data
     │
     ▼
LocalStorage API
     │
     ▼
Browser Storage
```

When the application starts, previously stored tasks are retrieved from LocalStorage and rendered automatically.

### Storage Characteristics

| Property               | Value            |
| ---------------------- | ---------------- |
| **Storage Technology** | LocalStorage API |
| **Persistence**        | ✅ Yes            |
| **Backend Required**   | ❌ No             |
| **Database Required**  | ❌ No             |
| **Cloud Sync**         | ❌ No             |
| **Multi-device Sync**  | ❌ No             |
| **Internet Required**  | ❌ No             |
| **Storage Scope**      | Browser / Device |

---

# 🗂️ Project Structure

```text
To-Do-List/
│
├── index.html
├── style.css
├── script.js
│
├── screenshots/
│   ├── home.png
│   ├── add-task.png
│   ├── edit-task.png
│   └── completed-tasks.png
│
└── README.md
```

### 📄 File Responsibilities

| File / Directory | Responsibility                                                                |
| ---------------- | ----------------------------------------------------------------------------- |
| `index.html`     | Defines the application's structure and UI                                    |
| `style.css`      | Handles styling, layout, responsiveness, and visual design                    |
| `script.js`      | Contains task logic, DOM manipulation, filtering, and LocalStorage operations |
| `screenshots/`   | Contains screenshots used for project documentation                           |
| `README.md`      | Project documentation                                                         |

---

# 🚀 Getting Started

## 📋 Prerequisites

You only need:

* A modern web browser
* Visual Studio Code or another code editor
* Git *(optional)*

### No additional setup required

You do **not** need:

* Node.js
* npm
* A backend server
* A database
* A package manager
* A build tool

---

# 📥 Installation

## 1. Clone the Repository

```bash
git clone https://github.com/your-username/To-Do-List.git
```

## 2. Navigate to the Project

```bash
cd To-Do-List
```

## 3. Open the Project

Open the project folder in **Visual Studio Code**.

## 4. Run the Application

The simplest option is to open:

```text
index.html
```

directly in your browser.

### ⭐ Recommended Development Setup

For a better development experience, install the **Live Server** extension in Visual Studio Code.

Then:

```text
Right-click index.html
        ↓
Open with Live Server
```

The application will open automatically in your browser.

---

# 📖 Usage

## ➕ Create a Task

1. Enter the task title.
2. Add an optional description.
3. Click **Add Task**.
4. The task appears in the task list.

---

## ✏️ Edit a Task

1. Locate the task.
2. Click **Edit**.
3. Modify the title or description.
4. Save the changes.

---

## ✅ Complete a Task

Use the task checkbox or completion control to toggle between:

```text
Active
   ↓
Completed
```

and:

```text
Completed
   ↓
Active
```

---

## 🗑️ Delete a Task

Click **Delete** on the task you want to remove.

> Deleted tasks are permanently removed from the application's LocalStorage.

---

## 🔎 Filter Tasks

Use the filter controls to display:

```text
All
 │
 ├── Active
 │
 └── Completed
```

This makes it easier to focus on unfinished or completed tasks.

---

# 🖼️ Screenshots

<div align="center">

### 🏠 Dashboard

<img src="screenshots/home.png" alt="To-Do List Dashboard" width="750">

<br><br>

### ➕ Add Task

<img src="screenshots/add-task.png" alt="Add Task Interface" width="750">

<br><br>

### ✏️ Edit Task

<img src="screenshots/edit-task.png" alt="Edit Task Interface" width="750">

<br><br>

### ✅ Completed Tasks

<img src="screenshots/completed-tasks.png" alt="Completed Tasks" width="750">

</div>

---

# 🎨 Design & User Experience

## 🎯 Simplicity

The interface focuses on the essential task-management workflow without unnecessary complexity.

## 📱 Responsiveness

The layout adapts to different screen sizes while maintaining readable content and accessible controls.

## ⚡ Efficiency

Frequently used operations such as adding, completing, editing, deleting, and filtering tasks are available directly from the main interface.

## 👁️ Visual Hierarchy

Task titles, descriptions, completion states, and actions are visually organized for quick scanning.

## ♿ Usability

The interface uses clear controls, predictable interactions, and responsive layouts to support a straightforward user experience.

---

# 🎯 Project Objectives

This project was developed to demonstrate practical frontend development skills.

### Development Objectives

* Build a functional task-management application
* Implement CRUD operations
* Manage application state on the client side
* Work with the DOM
* Handle browser events
* Implement persistent storage
* Create responsive layouts
* Implement task filtering
* Validate user input
* Organize frontend code effectively

---

# 🧠 Key Learning Outcomes

The project demonstrates practical knowledge of:

```text
HTML5
   ↓
Semantic Structure
   ↓
CSS3
   ↓
Responsive UI
   ↓
JavaScript
   ↓
DOM + Events + State
   ↓
LocalStorage
   ↓
Persistent Data
   ↓
CRUD
   ↓
Create + Read + Update + Delete
   ↓
Filtering
   ↓
Active + Completed Tasks
```

### Skills Practiced

* JavaScript fundamentals
* DOM manipulation
* Event handling
* CRUD operations
* LocalStorage
* JSON data handling
* Client-side state management
* Conditional rendering
* Form validation
* Responsive CSS
* UI/UX principles
* Frontend project organization

---

# 🌐 Browser Support

| Browser           | Support         |
| ----------------- | --------------- |
| Chrome            | ✅ Supported     |
| Firefox           | ✅ Supported     |
| Microsoft Edge    | ✅ Supported     |
| Safari            | ✅ Supported     |
| Opera             | ✅ Supported     |
| Internet Explorer | ❌ Not supported |

> The application requires a modern browser with LocalStorage support.

---

# 🗺️ Future Improvements

The current version focuses on the core task-management experience.

Future development can expand the application into a more complete productivity platform.

## Phase 1 — Productivity

* [ ] Task priorities
* [ ] Due dates
* [ ] Reminders
* [ ] Categories
* [ ] Tags
* [ ] Task search
* [ ] Task sorting
* [ ] Drag-and-drop ordering

## Phase 2 — User Experience

* [ ] Dark / Light theme
* [ ] Browser notifications
* [ ] Advanced filtering
* [ ] Keyboard shortcuts
* [ ] Improved accessibility
* [ ] Better empty states
* [ ] Improved mobile interactions
* [ ] Task statistics dashboard

## Phase 3 — Full-Stack Expansion

* [ ] User authentication
* [ ] REST API
* [ ] Backend service
* [ ] Database integration
* [ ] Cloud synchronization
* [ ] Multi-device access
* [ ] User-specific task management
* [ ] Collaborative task management

---

# ❓ FAQ

### Will I lose my tasks if I clear browser data?

Yes.

Since tasks are stored in LocalStorage, clearing the site's browser data can remove stored tasks.

An export or backup feature can be introduced in a future version.

### Can I use the application on multiple devices?

Not currently.

Tasks are stored locally in the browser and are not synchronized across devices.

### Does the application require an internet connection?

**No.**

Once the application files are available locally, the core functionality runs entirely in the browser.

### Does the project require a backend?

**No.**

The current version is completely client-side.

### Does the application use a database?

**No.**

Task data is stored using the browser's LocalStorage API.

---

# 📊 Project Information

| Property             | Details                     |
| -------------------- | --------------------------- |
| **Project Name**     | To-Do List Application      |
| **Category**         | Web Development             |
| **Application Type** | Task Management             |
| **Architecture**     | Client-Side Web Application |
| **Frontend**         | HTML5, CSS3, JavaScript     |
| **Storage**          | Browser LocalStorage        |
| **Backend**          | None                        |
| **Database**         | None                        |
| **Framework**        | None                        |
| **Interface**        | Responsive Web UI           |
| **Status**           | ✅ Completed                 |

---

# 🤝 Contributing

Contributions, improvements, bug fixes, and feature suggestions are welcome.

### Contribution Workflow

```text
Fork Repository
      ↓
Create Feature Branch
      ↓
Implement Changes
      ↓
Test Changes
      ↓
Commit Changes
      ↓
Push Branch
      ↓
Open Pull Request
```

### Contribution Guidelines

* Keep changes focused on a specific feature or fix.
* Follow the existing project structure.
* Maintain consistent coding style.
* Test existing functionality after making changes.
* Use descriptive commit messages.
* Update documentation when adding major features.

---

# 📄 License

This project is developed for **educational and portfolio purposes**.

You may modify, extend, and adapt the project for learning and development.

---

# ⭐ Support

If this project helped you learn something new, consider giving the repository a ⭐ **Star** on GitHub.

Your support helps the project reach more developers and learners.

---

<div align="center">

# 📝 To-Do List Application

### **One task at a time. One step closer to your goals.**

**Made with HTML • CSS • JavaScript • LocalStorage**

</div>
