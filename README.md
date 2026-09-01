<div align="center">

# 📝 To-Do List Application

**One task at a time. One step closer to your goals.**

A modern, responsive, and lightweight **To-Do List web application** for creating, managing, organizing, and tracking everyday tasks — right in your browser, with zero setup.

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](#-technology-stack)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)](#-technology-stack)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=flat&logo=javascript&logoColor=black)](#-technology-stack)
[![No Backend](https://img.shields.io/badge/Backend-None-lightgrey)](#-overview)
[![License](https://img.shields.io/badge/License-Educational-green)](#-license)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-brightgreen)](#-contributing)

[Features](#-features) • [Demo](#-screenshots) • [Getting Started](#-getting-started) • [Usage](#-usage) • [Roadmap](#%EF%B8%8F-future-improvements) • [Contributing](#-contributing)

</div>

---

## 📌 Overview

The To-Do List Application provides a centralized, distraction-free workspace for managing daily tasks and monitoring their completion status.

The project is built around three core principles:

| Principle | What it means |
|---|---|
| 🎯 **Simplicity** | Keep task management quick and clutter-free |
| ⚡ **Efficiency** | Make common actions accessible with minimal interaction |
| 📱 **Responsiveness** | Deliver a consistent experience across desktop, tablet, and mobile |

It's implemented entirely as a **client-side web application** — no backend server, no database, no build step required.

---

## ✨ Features

### 📋 Task Management

| Feature | Description |
| --- | --- |
| ➕ Create Task | Add a new task with a title and optional description |
| ✏️ Edit Task | Modify the details of an existing task |
| ✅ Complete Task | Mark tasks as completed or return them to active status |
| 🗑️ Delete Task | Permanently remove a task |
| 📋 Task Overview | View and manage all tasks from a centralized interface |

### 🔎 Task Filtering

Tasks can be filtered based on their current status:

- **All** — Display every task
- **Active** — Display pending tasks only
- **Completed** — Display finished tasks only

### 💾 Persistent Data

Task data is stored in the browser using the **LocalStorage API**, so tasks remain available after:

- ✅ Page refreshes
- ✅ Closing and reopening the browser
- ✅ Returning to the app later

> **Note:** Since data is stored locally, tasks are device/browser-specific and are **not** synchronized across devices.

### 📱 Responsive Design

The interface adapts cleanly across:

🖥️ Desktop · 💻 Laptop · 📱 Tablet · 📲 Mobile

Layout, typography, spacing, and controls all scale to the available screen space without sacrificing readability or accessibility.

---

## 🛠️ Technical Highlights

- Modular frontend structure
- Client-side application state handling
- Dynamic DOM rendering
- CRUD-style task operations
- LocalStorage-based persistence
- Real-time interface updates
- Status-based task filtering
- Event-driven interactions
- Form validation and input handling
- Responsive CSS layout (mobile-first)
- Lightweight — no frameworks, no build tools
- No backend or database required

---

## 💻 Technology Stack

| Technology | Purpose |
| --- | --- |
| **HTML5** | Semantic application structure and markup |
| **CSS3** | Styling, responsive layout, spacing, and visual presentation |
| **JavaScript (ES6+)** | Application logic, state handling, and user interactions |
| **LocalStorage API** | Persistent client-side task storage |

### Architecture

```text
User Interface
      │
      ▼
HTML + CSS
      │
      ▼
JavaScript Application Logic
      │
      ├── Task Creation
      ├── Task Editing
      ├── Task Completion
      ├── Task Deletion
      └── Task Filtering
      │
      ▼
LocalStorage API
      │
      ▼
Browser Storage
```

---

## 🔄 Application Workflow

```text
                    ┌───────────────────┐
                    │    Create Task    │
                    └─────────┬─────────┘
                              │
                              ▼
                    ┌───────────────────┐
                    │    Active Task    │
                    └─────────┬─────────┘
                              │
                    ┌─────────┴─────────┐
                    ▼                   ▼
             ┌─────────────┐     ┌─────────────┐
             │  Edit Task  │     │ Delete Task │
             └──────┬──────┘     └─────────────┘
                    │
                    ▼
             ┌─────────────────┐
             │  Save Changes   │
             └────────┬────────┘
                      │
                      ▼
             ┌─────────────────┐
             │ Mark Completed  │
             └────────┬────────┘
                      │
                      ▼
             ┌─────────────────┐
             │ Completed Task  │
             └─────────────────┘
```

---

## 💾 Data Persistence

The application uses the browser's **LocalStorage API** to persist task data across sessions.

### Persistence Flow

```text
┌─────────────────┐
│   User Action   │
└────────┬────────┘
         │
         ▼
┌───────────────────┐
│ Application State  │
└────────┬───────────┘
         │
         ▼
┌─────────────────┐
│   LocalStorage   │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Browser Storage │
└─────────────────┘
```

When a task is created, updated, completed, or deleted, the stored task data is updated accordingly. On load, previously stored tasks are retrieved from LocalStorage and rendered in the interface.

### Storage Characteristics

| Property | Value |
| --- | --- |
| Storage type | Browser LocalStorage |
| Persistence | ✅ Yes |
| Backend required | ❌ No |
| Cloud synchronization | ❌ No |
| Multi-device synchronization | ❌ No |
| Data scope | Browser/device-specific |

---

## 🗂️ Project Structure

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

### File Responsibilities

| File / Directory | Purpose |
| --- | --- |
| `index.html` | Application structure and UI elements |
| `style.css` | Styling and responsive layout |
| `script.js` | Task logic, event handling, filtering, and LocalStorage operations |
| `screenshots/` | Project screenshots used for documentation |
| `README.md` | Project documentation |

---

## 🚀 Getting Started

### Prerequisites

You only need:

- A modern web browser
- A code editor such as Visual Studio Code
- Git *(optional, for cloning the repository)*

No backend server, database, or additional runtime environment is required.

### Quick Start

```bash
git clone <repository-url>
cd To-Do-List
open index.html   # or double-click the file in your file explorer
```

### Recommended Development Setup

For a smoother development experience, open the project in **Visual Studio Code** with the **Live Server** extension so changes reload automatically in the browser.

---

## 📖 Usage

### ➕ Create a Task

1. Enter the task title.
2. Add an optional description.
3. Select **Add Task**.
4. The new task appears in the task list.

### ✏️ Edit a Task

1. Locate the task you want to modify.
2. Select **Edit**.
3. Update the task information.
4. Save the changes.

### ✅ Complete a Task

Use the task checkbox/control to toggle its status:

```text
Active → Completed
Completed → Active
```

### 🗑️ Delete a Task

Select **Delete** to permanently remove a task from the application.

### 🔎 Filter Tasks

Use the filter controls to quickly switch between task views:

```text
ALL → ACTIVE → COMPLETED
```

---

## 🖼️ Screenshots

<div align="center">

### Dashboard
<img src="screenshots/home.png" alt="To-Do List Dashboard" width="700" />

### Add Task
<img src="screenshots/add-task.png" alt="Add Task" width="700" />

### Edit Task
<img src="screenshots/edit-task.png" alt="Edit Task" width="700" />

### Completed Tasks
<img src="screenshots/completed-tasks.png" alt="Completed Tasks" width="700" />

</div>

---

## 🌐 Browser Support

| Browser | Supported |
| --- | --- |
| Chrome | ✅ |
| Firefox | ✅ |
| Edge | ✅ |
| Safari | ✅ |
| Opera | ✅ |
| Internet Explorer | ❌ Not supported |

> Requires a browser with LocalStorage support (all modern browsers).

---

## 🎨 Design & User Experience

### Simplicity
The interface minimizes unnecessary elements and keeps the primary task workflow easy to understand.

### Responsiveness
The layout adapts to different viewport sizes to provide a consistent experience across desktop and mobile devices.

### Efficiency
Common operations — adding, completing, editing, deleting, and filtering tasks — are available directly from the main interface.

### Visual Hierarchy
Task titles, descriptions, completion states, and available actions are organized to make task information easy to scan at a glance.

### Usability
Clear controls and predictable interactions help users manage their tasks without unnecessary complexity.

---

## 🎯 Project Objectives

This project demonstrates practical frontend development skills, including:

- Building a functional task-management application
- Implementing CRUD operations
- Managing client-side application state
- Working with the DOM
- Handling user interactions and events
- Implementing persistent browser storage
- Building responsive interfaces
- Implementing task filtering
- Handling form input and validation
- Organizing frontend code effectively
- Creating a practical, real-world web application

---

## 🧠 Key Learning Outcomes

- JavaScript application logic
- DOM manipulation
- Event handling
- CRUD operations
- LocalStorage integration
- Data serialization and retrieval
- State management
- Conditional rendering
- Task filtering
- Form validation
- Responsive CSS
- User interaction design
- Frontend project organization

---

## 🗺️ Future Improvements

The current implementation covers the core functionality required for task management. Planned enhancements are grouped by phase below.

### Phase 1 — Productivity
- [ ] Task priorities
- [ ] Due dates
- [ ] Reminders
- [ ] Categories and tags
- [ ] Task search
- [ ] Task sorting
- [ ] Drag-and-drop ordering

### Phase 2 — User Experience
- [ ] Dark / Light theme
- [ ] Browser notifications
- [ ] Advanced filtering
- [ ] Keyboard shortcuts
- [ ] Improved accessibility (ARIA, focus management)
- [ ] Better empty-state messages
- [ ] Improved mobile interactions

### Phase 3 — Full-Stack Expansion
- [ ] User authentication
- [ ] REST API integration
- [ ] Backend service
- [ ] Database integration
- [ ] Cloud synchronization
- [ ] Multi-device access
- [ ] User-specific task management
- [ ] Collaborative task management

---

## ❓ FAQ

**Will I lose my tasks if I clear my browser cache?**
Yes — since tasks live in LocalStorage, clearing site data or browser storage will remove them. Export/backup functionality is on the future roadmap.

**Can I use this on multiple devices?**
Not yet. Tasks are stored locally per browser/device. Multi-device sync is planned for Phase 3.

**Does this require an internet connection?**
No. Once loaded, the app works fully offline since everything runs client-side.

---

## 📊 Project Information

| Property | Details |
| --- | --- |
| **Project Name** | To-Do List Application |
| **Category** | Web Development |
| **Application Type** | Task Management |
| **Architecture** | Client-Side Web Application |
| **Frontend** | HTML5, CSS3, JavaScript |
| **Storage** | Browser LocalStorage |
| **Interface** | Responsive Web UI |
| **Backend** | None |
| **Database** | None |
| **Status** | ✅ Completed |

---

## 🤝 Contributing

Contributions, improvements, and feature suggestions are welcome!

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

When contributing, please:

- Keep changes focused and scoped to a single feature or fix
- Maintain the existing project structure and coding style
- Ensure existing functionality continues to work correctly
- Add clear commit messages describing your changes

---

## 📄 License

This project is developed for **educational and portfolio purposes**.

You are free to modify, extend, and adapt the project for learning and development purposes.

---

## ⭐ Support

If this project helped you learn something new, consider giving it a ⭐ **Star** on GitHub — it helps others discover it too.

---

<div align="center">

### 📝 Built to keep tasks simple, organized, and actionable.

**One task at a time. One step closer to your goals.**

</div>
