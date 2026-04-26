# 🚀 QuickEMS — Employee Management System

A production-oriented full-stack Employee Management System designed to handle real-world HR workflows including employee lifecycle management, attendance tracking, leave processing, and payroll generation — all within a role-based architecture.

Unlike basic CRUD demos, QuickEMS focuses on **operational workflows, automation, and system design patterns used in real applications**.

---

## 🌐 Live Demo

👉 https://aarshems.vercel.app/

### Demo Credentials

**Admin**
- Email: admin@gmail.com  
- Password: Admin@1234  

**Employee**
- Email: vicky@gmail.com  
- Password: Vicky@1234    

---

## ✨ Why This Project Stands Out

- Implements **role-based product architecture** (Admin vs Employee systems)
- Handles **real HR workflows**, not just static CRUD
- Integrates **event-driven automation (Inngest)** for background jobs
- Demonstrates **end-to-end ownership**: UI → API → DB → workflows
- Built with **modern tooling (React 19, Vite 8, Express 5)**

---

## 🧠 Core Features

### 🔐 Authentication & Access Control
- JWT-based authentication
- Role-based route protection (Admin / Employee)
- Secure session validation & password updates

---

### 👥 Employee Management
- Admin-controlled employee lifecycle
- Soft deletion & employment status tracking
- Linked user-account + employee profile system

---

### 🕒 Attendance System
- Unified clock-in / clock-out API
- Automatic working hours calculation
- Smart attendance status classification
- Background reminders for missed checkout

---

### 📝 Leave Management
- Employee leave request workflow
- Admin approval/rejection system
- Automated reminders for pending approvals

---

### 💰 Payslip System
- Admin-generated payslips with computed salary breakdown
- Role-based access to payslip history
- Dedicated printable payslip view

---

### 📊 Dashboard & Insights
- Admin analytics (employees, attendance, leave)
- Employee dashboard (activity + latest payslip)

---

### ⚙️ Automation & Background Jobs
- Event-driven workflows using Inngest:
  - Auto checkout handling
  - Leave approval reminders
  - Daily attendance alerts
- Email notifications via Nodemailer

---

## 📸 Screenshots

### 🏠 Dashboard
<p align="center">
  <img src="./screenshots/dashboard.png" alt="Dashboard" width="800"/>
</p>

> Admin dashboard showing system overview, employee stats, attendance, and pending requests.

---

### 💰 Payslip View
<p align="center">
  <img src="./screenshots/payslip.png" alt="Payslip View" width="800"/>
</p>

> Detailed payslip with salary breakdown including basic salary, allowances, deductions, and net salary.

---

### ⚙️ Admin Panel
<p align="center">
  <img src="./screenshots/admin-panel.png" alt="Admin Panel" width="800"/>
</p>

> Admin interface to manage employees, generate payslips, and control system workflows.

---

### 🔐 Login Page
<p align="center">
  <img src="./screenshots/login.png" alt="Login Page" width="800"/>
</p>

> Secure login system with role-based access for Admin and Employee users.

---

## 🛠️ Tech Stack

### Frontend
- React 19
- Vite 8
- Tailwind CSS 4
- React Router 7
- Axios
- React Hot Toast
- Lucide React
- date-fns

### Backend
- Node.js (ESM)
- Express 5
- MongoDB + Mongoose
- JWT (jsonwebtoken)
- bcrypt
- Multer
- Inngest (event workflows)
- Nodemailer

---

## Folder Structure

```text
EMS/
├── client/
│   ├── public/
│   ├── src/
│   │   ├── api/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── context/
│   │   ├── pages/
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── package.json
│   └── vite.config.js
│
├── server/
│   ├── config/
│   ├── constants/
│   ├── controllers/
│   ├── inngest/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── seed.js
│   ├── server.js
│   └── package.json
│
└── README.md
```

---

## 🏗️ System Architecture

QuickEMS follows a layered architecture separating frontend, backend, and async workflows.

---

### 🔄 Flow

Client (React)  
↓  
Routes (Express)  
↓  
Controllers (Business Logic)  
↓  
Database (MongoDB)  
↓  
Async Jobs (Inngest)

---

### 🚧 Future Improvements

- Role hierarchy (HR / Manager roles)
- Advanced analytics dashboard
