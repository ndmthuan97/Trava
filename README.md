<p align="center">
  <img src="images/trava.png" alt="Trava Logo" width="200"/>
</p>

# 🚀 Trava - All-in-One Productivity & Team Collaboration Platform

**Trava** is a robust, modern ecosystem designed to streamline personal productivity and enhance team collaboration. By integrating a high-performance .NET backend with a responsive Angular frontend, Trava provides a seamless experience for managing workspaces, tasks, and real-time interactions.

---

## 🏛️ System Architecture

The project is built with a focus on scalability, maintainability, and performance, utilizing industry-standard architectural patterns.

### Backend (.NET 8)
*   **Clean Architecture:** Strict separation of concerns (Domain, Application, Infrastructure, API).
*   **CQRS Pattern:** Implementation via **MediatR** to decouple read and write operations.
*   **Performance:** Integrated **Redis** caching and **PostgreSQL** for reliable data persistence.

### Frontend (Angular 18)
*   **Modular Design:** Scalable architecture with feature-based modules.
*   **Modern UI:** Built with **PrimeNG 18** and **Tailwind CSS** for a premium, responsive experience.
*   **Real-time Integration:** Leverages **Supabase** for authentication and real-time data synchronization.

---

## 🛠️ Technology Stack

| Component | technologies |
| :--- | :--- |
| **Frameworks** | .NET 8.0, Angular 18.2 |
| **Database & Caching** | PostgreSQL, Redis, Supabase (Auth/DB) |
| **UI & Styling** | Tailwind CSS 3.4, PrimeNG 18, PrimeIcons |
| **Communication** | RESTful API, RxJS, HttpClient |
| **Utilities** | MediatR, AutoMapper, FluentValidation, Chart.js |

---

## ✨ Core Features

### 🏢 Workspace Management (Spaces)
*   **Dual Mode:** Support for both **Private** (Personal) and **Team** spaces.
*   **Granular Permissions:** Role-based access control within shared environments.
*   **Invitations:** Secure mechanism for inviting and managing team members.

### ✅ Advanced Task Management
*   **Hierarchical Structure:** Parent tasks and sub-tasks for complex workflows.
*   **Detailed Tracking:** Manage priorities (Low to Urgent), effort (Points), and deadlines.
*   **Engagement:** Real-time comments and activity tracking on every task.

### 📊 Real-time Insights & Notifications
*   **Dynamic Dashboard:** Visual statistics and progress tracking via Chart.js.
*   **Smart Notifications:** Instant updates on task assignments and workspace changes.
*   **Responsive Experience:** Fully optimized for Desktop, Tablet, and Mobile.

---

## 📂 Project Structure

```bash
trava/
├── trava-backend/        # .NET 8 Clean Architecture Source
│   ├── Trava.API/        # Presentation Layer
│   ├── Trava.Application/# Core Logic & CQRS
│   ├── Trava.Domain/     # Entities & Enums
│   └── Trava.Infrastructure/ # Persistence & Services
└── trava-frontend/       # Angular 18 Enterprise Frontend
    ├── src/app/core/     # Global Services & Guards
    ├── src/app/features/ # Feature Modules (Dashboard, Tasks, Spaces)
    └── src/app/shared/   # Reusable UI Components
```

---

## 🚀 Quick Start

### 1. Prerequisites
*   [.NET 8.0 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
*   [Node.js](https://nodejs.org/) (v18+) & [Angular CLI](https://angular.dev/tools/cli)
*   [PostgreSQL](https://www.postgresql.org/) & [Redis](https://redis.io/)

### 2. Backend Setup
```bash
cd trava-backend/src/Trava.Infrastructure
dotnet ef database update --startup-project ../Trava.API/
cd ../Trava.API
dotnet run
```

### 3. Frontend Setup
```bash
cd trava-frontend
npm install
npm start
```

---
Developed with ❤️ by **Minh Thuan**.
