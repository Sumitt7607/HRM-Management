# HR Cloud - HRM Management System

A premium, modern Human Resource Management (HRM) system designed for streamlined employee administration, attendance tracking, payroll management, and leave requests. 

The project is structured as a monorepo containing a React frontend powered by Vite and a robust Node.js/Express backend connected to MongoDB.

---

## 🏗️ Project Architecture

This application consists of two main components:

1. **[CMS-Frontend](file:///c:/Users/Sumit%20Kushwaha/OneDrive/Desktop/HRM%20Management/CMS-Frontend)**: A React-based web application with modern typography, custom CSS styling, smooth transitions, and a fully responsive layout.
2. **[CMS-Backend](file:///c:/Users/Sumit%20Kushwaha/OneDrive/Desktop/HRM%20Management/CMS-Backend)**: An Express REST API that handles secure authentication (JWT), data persistence (MongoDB/Mongoose), role-based access control, and HR business logic.

```
HRM Management/
├── CMS-Frontend/          # React + Vite client-side app
└── CMS-Backend/           # Express server & API endpoints
```

---

## ✨ Features

### 👑 Admin Dashboard
- **Employee Management**: Create, view, update, and manage employee records.
- **Leave Approval**: Review, approve, or reject employee leave requests.
- **Payroll Processing**: Calculate, generate, and track monthly payroll slips.
- **Attendance Insights**: Monitor overall attendance logs and active timesheets.

### 👤 Employee Dashboard
- **Timesheet Management**: Track and log daily work hours.
- **Leave Requests**: Submit and track status of leave applications.
- **Payroll Slips**: View and download personal salary slips.
- **Stats Counter**: View summarized statistics of worked hours and pending tasks.

---

## 🛠️ Technology Stack

### Frontend
- **Framework**: React.js (Vite)
- **Routing**: React Router DOM
- **Animations**: Framer Motion
- **Icons**: Lucide React
- **Styling**: Pure CSS with CSS variables
- **HTTP Client**: Axios

### Backend
- **Framework**: Express.js
- **Runtime**: Node.js
- **Database**: MongoDB & Mongoose
- **Security**: Bcrypt.js (Password Hashing) & JSON Web Tokens (JWT)
- **Environment**: Dotenv

---

## 🚀 Quick Start Guide

### Prerequisites
Make sure you have [Node.js](https://nodejs.org/) (v18+) installed.

---

### Step 1: Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd CMS-Backend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Configure environment variables. Create a `.env` file inside the `CMS-Backend` directory:
   ```env
   MONGODB_URI=your_mongodb_connection_string
   PORT=5000
   JWT_SECRET=your_jwt_secret
   FRONTEND_URL=http://localhost:5173
   ```

4. **Seed the database** (Optional but recommended for testing):
   ```bash
   node seed.js
   ```
   *Creates credentials for testing:*
   - **Admin Account**: `admin@gmail.com` | `password`
   - **Employee Account**: `test@gmail.com` | `123`

5. Start the backend development server:
   ```bash
   npm run dev
   ```

---

### Step 2: Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd ../CMS-Frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Configure environment variables. Create a `.env` file inside the `CMS-Frontend` directory:
   ```env
   VITE_API_URL=http://localhost:5000/api
   ```

4. Start the frontend development server:
   ```bash
   npm run dev
   ```

---

## 🌐 Deployment

Both the frontend and backend are configured for simple deployment on **Vercel** with corresponding `vercel.json` configurations in their respective directories.
