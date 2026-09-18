<div align="center">📝 To-Do List Application. 

One task at a time. One step closer to your goals.

A modern, responsive, and lightweight task management web application built with HTML5, CSS3, and vanilla JavaScript. Create, organize, update, complete, filter, and delete tasks directly from your browser — with persistent storage and zero backend setup.

<br>""HTML5" (https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)" (#-technology-stack)
""CSS3" (https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)" (#-technology-stack)
""JavaScript" (https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)" (#-technology-stack)
""LocalStorage" (https://img.shields.io/badge/Storage-LocalStorage-orange?style=for-the-badge)" (#-data-persistence)
""Backend" (https://img.shields.io/badge/Backend-None-lightgrey?style=for-the-badge)" (#-architecture)
""Status" (https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)" (#-project-information)

<br>"Features" (#-features) • "Getting Started" (#-getting-started) • "Usage" (#-usage) • "Architecture" (#-architecture) • "Screenshots" (#-screenshots) • "Roadmap" (#-future-improvements)

</div>---

📌 Overview

The To-Do List Application is a client-side task management system designed to make everyday task tracking simple, fast, and distraction-free.

The application allows users to:

- Create new tasks
- Add optional task descriptions
- Edit existing tasks
- Mark tasks as completed
- Delete tasks
- Filter tasks by status
- Persist tasks across browser sessions
- Use the application across desktop, tablet, and mobile devices

The entire application runs inside the browser, making it lightweight and easy to deploy.

Core Principles

Principle| Description
🎯 Simplicity| Keep task management straightforward and clutter-free
⚡ Efficiency| Perform common actions with minimal interaction
📱 Responsiveness| Maintain usability across different screen sizes
💾 Persistence| Preserve tasks using browser-based LocalStorage
🧩 Maintainability| Keep the frontend structure simple and easy to understand

---

✨ Features

📋 Task Management

Feature| Description
➕ Create Task| Add a task with a title and optional description
✏️ Edit Task| Modify an existing task's information
✅ Complete Task| Toggle tasks between active and completed states
🗑️ Delete Task| Permanently remove unwanted tasks
📋 Task Overview| View all tasks from a centralized interface

🔎 Task Filtering

Quickly switch between different task states:

- All — Display every task
- Active — Display pending tasks
- Completed — Display finished tasks

💾 Persistent Storage

Tasks are stored using the browser's LocalStorage API.

Your data remains available after:

- 🔄 Refreshing the page
- 🌐 Closing and reopening the browser
- 🔁 Returning to the application later

«Important: LocalStorage is browser/device-specific. Tasks are not automatically synchronized between different devices or browsers.»

📱 Responsive Interface

The UI adapts to:

Desktop · Laptop · Tablet · Mobile

Responsive layouts, spacing, typography, and controls are designed to remain usable across different viewport sizes.

⚡ Lightweight

The application has:

- ❌ No backend
- ❌ No database
- ❌ No framework
- ❌ No build system
- ❌ No external runtime dependency
- ✅ Pure HTML, CSS, and JavaScript

---

🛠️ Technical Highlights

The project demonstrates practical frontend development concepts:

- Modular frontend organization
- CRUD-style task operations
- Client-side state management
- Dynamic DOM manipulation
- Event-driven programming
- LocalStorage integration
- JSON serialization and deserialization
- Conditional rendering
- Status-based filtering
- Form validation
- Responsive CSS
- Real-time UI updates
- Browser-based persistence
- Mobile-friendly interface

---

🧰 Technology Stack

Technology| Purpose
HTML5| Semantic structure and application markup
CSS3| Styling, layout, responsiveness, and visual presentation
JavaScript ES6+| Application logic, state handling, DOM manipulation, and events
LocalStorage API| Persistent client-side task storage

Why Vanilla JavaScript?

This project intentionally uses vanilla JavaScript instead of a frontend framework to demonstrate a strong understanding of:

- DOM manipulation
- Event handling
- JavaScript state management
- Browser APIs
- CRUD operations
- Data persistence

---

🏗️ Architecture

The application follows a simple client-side architecture:

┌──────────────────────┐
│      User Interface  │
│      HTML + CSS      │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ JavaScript Application│
│       Logic          │
└──────────┬───────────┘
           │
     ┌─────┼──────────────┐
     │     │              │
     ▼     ▼              ▼
  Create  Update        Delete
  Task    Task          Task
     │     │              │
     └─────┼──────────────┘
           │
           ▼
┌──────────────────────┐
│    Task Filtering    │
│   Active / Completed │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│   LocalStorage API   │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│    Browser Storage   │
└──────────────────────┘

---

🔄 Application Workflow

                 ┌───────────────┐
                 │   Open App    │
                 └───────┬───────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Load LocalStorage│
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Render Task List │
                └────────┬────────┘
                         │
             ┌───────────┼───────────┐
             ▼           ▼           ▼
        Create Task   Edit Task   Delete Task
             │           │           │
             └───────────┼───────────┘
                         ▼
                ┌─────────────────┐
                │ Update App State │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Save to Storage │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Update UI        │
                └─────────────────┘

---

💾 Data Persistence

The application uses LocalStorage to store task information directly inside the user's browser.

Persistence Flow

User Action
     │
     ▼
Application State
     │
     ▼
Serialize Task Data
     │
     ▼
LocalStorage
     │
     ▼
Browser Storage

When the application starts, previously stored tasks are retrieved and rendered automatically.

Storage Characteristics

Property| Value
Storage Technology| LocalStorage API
Persistence| ✅ Yes
Backend Required| ❌ No
Database Required| ❌ No
Cloud Sync| ❌ No
Multi-device Sync| ❌ No
Internet Required| ❌ No
Storage Scope| Browser / Device

---

🗂️ Project Structure

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

File Responsibilities

File / Directory| Responsibility
"index.html"| Defines the application's structure and UI
"style.css"| Handles styling, layout, responsiveness, and visual design
"script.js"| Contains task logic, DOM manipulation, filtering, and LocalStorage operations
"screenshots/"| Contains screenshots used for project documentation
"README.md"| Project documentation

---

🚀 Getting Started

Prerequisites

You only need:

- A modern web browser
- Visual Studio Code or another code editor
- Git (optional)

No Node.js, npm, backend server, or database is required.

---

📥 Installation

1. Clone the Repository

git clone https://github.com/your-username/To-Do-List.git

2. Navigate to the Project

cd To-Do-List

3. Open the Project

Open the folder in Visual Studio Code.

4. Run the Application

You can simply open:

index.html

in your browser.

Recommended

For development, use the Live Server extension in Visual Studio Code.

Right-click:

index.html

and select:

Open with Live Server

---

📖 Usage

➕ Create a Task

1. Enter the task title.
2. Add an optional description.
3. Click Add Task.
4. The task will appear in the task list.

---

✏️ Edit a Task

1. Locate the task.
2. Click Edit.
3. Modify the title or description.
4. Save the changes.

---

✅ Complete a Task

Use the task checkbox or completion control to toggle the task between:

Active → Completed

and:

Completed → Active

---

🗑️ Delete a Task

Click Delete on the task you want to remove.

«Deleted tasks are permanently removed from the application's LocalStorage.»

---

🔎 Filter Tasks

Use the filter controls to display:

All
│
├── Active
│
└── Completed

This makes it easier to focus on unfinished or completed tasks.

---

🖼️ Screenshots

<div align="center">🏠 Dashboard

<img src="screenshots/home.png" alt="To-Do List Dashboard" width="750"/><br><br>

➕ Add Task

<img src="screenshots/add-task.png" alt="Add Task Interface" width="750"/><br><br>

✏️ Edit Task

<img src="screenshots/edit-task.png" alt="Edit Task Interface" width="750"/><br><br>

✅ Completed Tasks

<img src="screenshots/completed-tasks.png" alt="Completed Tasks" width="750"/></div>---

🎨 Design & User Experience

🎯 Simplicity

The interface focuses on the essential task-management workflow without unnecessary complexity.

📱 Responsiveness

The layout adapts to different screen sizes while maintaining readable content and accessible controls.

⚡ Efficiency

Frequently used operations such as adding, completing, editing, deleting, and filtering tasks are available directly from the main interface.

👁️ Visual Hierarchy

Task titles, descriptions, completion states, and actions are visually organized for quick scanning.

♿ Usability

The interface is designed with clear controls, predictable interactions, and responsive layouts in mind.

---

🎯 Project Objectives

This project was developed to demonstrate practical frontend development skills.

Development Objectives

- Build a functional task-management application
- Implement CRUD operations
- Manage application state on the client side
- Work with the DOM
- Handle browser events
- Implement persistent storage
- Create responsive layouts
- Implement task filtering
- Validate user input
- Organize frontend code effectively

---

🧠 Key Learning Outcomes

Through this project, the following concepts are demonstrated:

HTML5
  ↓
Semantic Structure

CSS3
  ↓
Responsive UI

JavaScript
  ↓
DOM + Events + State

LocalStorage
  ↓
Persistent Data

CRUD
  ↓
Create + Read + Update + Delete

Filtering
  ↓
Active + Completed Tasks

Skills Practiced

- JavaScript fundamentals
- DOM manipulation
- Event handling
- CRUD operations
- LocalStorage
- JSON data handling
- Client-side state management
- Conditional rendering
- Form validation
- Responsive CSS
- UI/UX principles
- Frontend project organization

---

🌐 Browser Support

Browser| Support
Chrome| ✅ Supported
Firefox| ✅ Supported
Microsoft Edge| ✅ Supported
Safari| ✅ Supported
Opera| ✅ Supported
Internet Explorer| ❌ Not supported

«The application requires a modern browser with LocalStorage support.»

---

🗺️ Future Improvements

The current version focuses on the core task-management experience. Future development can expand the application into a more complete productivity platform.

Phase 1 — Productivity

- [ ] Task priorities
- [ ] Due dates
- [ ] Reminders
- [ ] Categories
- [ ] Tags
- [ ] Task search
- [ ] Task sorting
- [ ] Drag-and-drop ordering

Phase 2 — User Experience

- [ ] Dark / Light theme
- [ ] Browser notifications
- [ ] Advanced filtering
- [ ] Keyboard shortcuts
- [ ] Improved accessibility
- [ ] Better empty states
- [ ] Improved mobile interactions
- [ ] Task statistics dashboard

Phase 3 — Full-Stack Expansion

- [ ] User authentication
- [ ] REST API
- [ ] Backend service
- [ ] Database integration
- [ ] Cloud synchronization
- [ ] Multi-device access
- [ ] User-specific task management
- [ ] Collaborative task management

---

❓ FAQ

Will I lose my tasks if I clear browser data?

Yes. Since tasks are stored in LocalStorage, clearing the site's browser data can remove stored tasks.

An export/backup feature can be added in a future version.

Can I use the application on multiple devices?

Not currently.

Tasks are stored locally in the browser, so they are not synchronized across devices.

Does the application require an internet connection?

No.

Once the application files are available locally, the core functionality runs entirely in the browser.

Does the project require a backend?

No.

The current version is completely client-side.

Does the application use a database?

No.

Task data is stored using the browser's LocalStorage API.

---

📊 Project Information

Property| Details
Project Name| To-Do List Application
Category| Web Development
Application Type| Task Management
Architecture| Client-Side Web Application
Frontend| HTML5, CSS3, JavaScript
Storage| Browser LocalStorage
Backend| None
Database| None
Framework| None
Interface| Responsive Web UI
Status| ✅ Completed

---

🤝 Contributing

Contributions, improvements, bug fixes, and feature suggestions are welcome.

Contribution Workflow

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

Contribution Guidelines

- Keep changes focused on a specific feature or fix.
- Follow the existing project structure.
- Maintain consistent coding style.
- Test existing functionality after making changes.
- Use descriptive commit messages.
- Update documentation when adding major features.

---

📄 License

This project is developed for educational and portfolio purposes.

You may modify, extend, and adapt the project for learning and development.

---

⭐ Support

If this project helped you learn something new, consider giving the repository a ⭐ Star on GitHub.

Your support helps the project reach more developers and learners.

---

<div align="center">📝 Built to keep tasks simple, organized, and actionable.

One task at a time. One step closer to your goals.

Made with HTML • CSS • JavaScript • LocalStorage

</div>
