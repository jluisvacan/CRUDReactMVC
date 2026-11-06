# 🚀 CRUDReactMVC

[![.NET Core](https://img.shields.io/badge/.NET-8.0-512BD4?style=for-the-badge&logo=.net&logoColor=white)](https://dotnet.microsoft.com/)
[![ASP.NET Core Web API](https://img.shields.io/badge/Backend-ASP.NET%20Core-blue?style=for-the-badge)](https://learn.microsoft.com/en-us/aspnet/core/)
[![React](https://img.shields.io/badge/Frontend-React-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![Entity Framework Core](https://img.shields.io/badge/ORM-EF%20Core-green?style=for-the-badge)](https://learn.microsoft.com/en-us/ef/core/)


A modern Full-Stack web application combining an **ASP.NET Core** backend with a responsive **React** single-page frontend. This repository demonstrates seamless client-server integration, RESTful API consumption, and robust CRUD data management.

---

## 🌟 Key Features

* **Full-Stack Integration:** Decoupled architecture serving REST API endpoints from .NET to a React client.
* **Complete CRUD Operations:** Full lifecycle management (Create, Read, Update, Delete) with real-time UI updates.
* **Component-Based UI:** Modular React components structured for reusability, state management, and maintenance.
* **Data Persistence:** Entity Framework Core integration for streamlined database context mapping and migrations.
* **Input Validation & Error Handling:** Robust client-side validation paired with server-side response protocols.

---

## 🛠️ Tech Stack

### **Backend**
* **Framework:** ASP.NET Core (.NET) Web API / MVC Controllers
* **ORM:** Entity Framework Core
* **Language:** C#

### **Frontend**
* **Library:** React.js
* **Styles & UI:** CSS3 / Bootstrap / Modern JavaScript (ES6+)
* **HTTP Client:** Fetch API / Axios for asynchronous API communication

### **Tools & Environment**
* **Tooling:** Visual Studio / VS Code, Node.js, npm, .NET CLI

---

## 📂 Project Structure

The project follows standard Full-Stack conventions, organizing the backend domain services alongside client-side React resources:

```text
CRUDReactMVC/
│
├── CRUDReactMVC.sln            # Solution file tying both projects together
│
├── CRUDReactMVC.Server/        # Backend ASP.NET Core Web API Project
│   ├── Controllers/            # API endpoints handling HTTP requests (GET, POST, PUT, DELETE)
│   ├── Data/                   # EF Core DbContext, context configuration, and seed data
│   ├── Models/                 # Domain entity models (e.g., Pelicula.cs) and DTOs
│   ├── Migrations/             # Database migration history (Entity Framework Core)
│   ├── Properties/             # Launch settings and development configurations
│   ├── Program.cs              # Service configurations, CORS policies, and pipeline middleware
│   └── appsettings.json        # Database connection strings and environment variables
│
└── crudreactmvc.client/        # Frontend React SPA Project
    ├── public/                 # Static assets and HTML entry points
    ├── src/                    # React source code components, styles, and logic
    │   ├── App.jsx / App.js    # Root application component
    │   └── main.jsx / index.js # DOM rendering entry point
    ├── package.json            # Node.js dependencies, scripts, and package management
    └── vite.config.js / ...    # Frontend build tool configurations
├── package.json                # Node.js manifest defining project metadata, scripts, and dependencies
├── package-lock.json           # Automated lockfile ensuring deterministic dependency tree resolution
```
## ⚙️ Getting Started
Follow these steps to set up and run the Full-Stack application locally.

## Prerequisites
- .NET 8.0 SDK
- Node.js (v16.x or higher) and npm

## Installation & Execution
### 1. Clone the repository:
```bash
git clone https://github.com/jluisvacan/CRUDReactMVC.git
cd CRUDReactMVC
```
### 2. Backend Setup:
Restore .NET packages and update the database:
```bash
dotnet restore
dotnet ef database update
```
### 3. Frontend Setup (if dependencies are located inside ClientApp):
```bash
cd ClientApp
npm install
cd ..
```

### 4. Run the Project:
```bash
dotnet run
```

### 5. Access the application:
```text
Open your browser and navigate to https://localhost:5015.
```

## 📈 Engineering Highlights
- **CORS & Middleware Configuration:** Properly configured Cross-Origin Resource Sharing (CORS) policies ensuring secure API access.

- **Asynchronous Operations:** Asynchronous async/await implementation across all API endpoints and HTTP frontend fetches for non-blocking UI rendering.

- **Clean State Management:** React hook implementation (useState, useEffect) managing seamless component lifecycles and API data flows.