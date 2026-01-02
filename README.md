 Employee Management System

<div align="center">

![MERN Stack](https://img.shields.io/badge/Stack-MERN-green)
![React](https://img.shields.io/badge/React-18.2.0-blue)
![Node.js](https://img.shields.io/badge/Node.js-Express-green)
![MongoDB](https://img.shields.io/badge/Database-MongoDB-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow)

A comprehensive full-stack web application designed to streamline HR operations, attendance tracking, and employee management processes.

[Features](#-features) • [Tech Stack](#-technologies-used) • [Installation](#-installation) • [Usage](#-usage) • [Screenshots](#-screenshots)

</div>

---

## 📋 Overview

The Employee Management System (EMS) is a modern, feature-rich web application built to simplify and automate human resource management tasks. From attendance tracking to leave management, this system provides an all-in-one solution for managing your workforce efficiently.

Built with the powerful MERN stack (MongoDB, Express.js, React, Node.js), it offers a responsive, intuitive interface with real-time data visualization and role-based access control.

## ✨ Features

### 🔐 Authentication & Authorization
- Secure JWT-based authentication system
- Role-based access control (Super Admin & Regular Users)
- Password encryption using bcrypt
- Protected routes and API endpoints

### 👤 User & Profile Management
- Comprehensive employee profiles with personal details
- Profile picture upload with image optimization
- Secure credential management
- Employee ID and Aadhar/PAN card integration
- Edit and update personal information

### ⏰ Attendance Management
- **Real-time Clock In/Out System** with timestamp tracking
- **Monthly Attendance Reports** with visual analytics
- **Attendance Calendar** view for easy tracking
- **Late Arrival Detection** and reporting
- **Attendance Statistics** dashboard with charts
- Automatic attendance calculation and summaries
- Export attendance data functionality

### 📅 Leave Management
- Submit leave requests with reason and date range
- View personal leave history and status
- Admin approval/rejection workflow
- Real-time leave status updates
- Leave balance tracking
- Dashboard showing who's on leave today

### 📊 Advanced Dashboard
- **Interactive Charts** using Recharts and Nivo
- Real-time employee statistics
- Department-wise employee distribution
- Monthly attendance trends
- Leave approval pending notifications
- Quick access to key metrics

### 👥 Employee Management (Admin)
- Complete employee directory
- Add, edit, and manage employee records
- View detailed employee profiles
- Bulk employee data operations
- Employee search and filtering

## 🛠 Technologies Used

### Frontend
- **React 18.2** - Modern UI library with hooks
- **React Router DOM** - Client-side routing
- **Ant Design** - Enterprise-level UI components
- **React Bootstrap** - Responsive UI framework
- **Recharts** - Composable charting library
- **Nivo** - Advanced data visualization
- **React Calendar** - Interactive calendar component
- **Axios** - HTTP client for API requests
- **React Hook Form** - Form validation and management

### Backend
- **Node.js** - JavaScript runtime environment
- **Express.js** - Fast, minimalist web framework
- **MongoDB** - NoSQL database for data persistence
- **Mongoose** - MongoDB object modeling
- **JWT** - Secure token-based authentication
- **Bcrypt.js** - Password hashing
- **Multer** - File upload middleware
- **Sharp** - Image processing and optimization
- **Node-Schedule** - Task scheduling for automated jobs

### Additional Tools
- **Nodemon** - Auto-restart during development
- **Concurrently** - Run multiple npm scripts simultaneously
- **Crypto-js** - Cryptographic functions
- **Moment.js** - Date and time manipulation
- **PDFKit** - PDF generation for reports

## 📁 Project Structure

```
empp/
├── backend/                 # Node.js backend
│   ├── controllers/        # Route controllers
│   ├── models/            # Mongoose schemas
│   ├── routes/            # API routes
│   ├── middleware/        # Custom middleware
│   ├── database/          # Database configuration
│   ├── uploads/           # File uploads directory
│   └── server.js          # Entry point
│
├── frontend/               # React frontend
│   ├── public/            # Static files
│   └── src/
│       ├── Attendance/    # Attendance module
│       ├── Dashboard/     # Dashboard components
│       ├── User/          # User management
│       ├── UserProfile/   # Profile components
│       ├── Navigation/    # Navigation components
│       ├── UI/            # Reusable UI components
│       ├── context/       # React context
│       └── utils/         # Utility functions
│
└── README.md
```

## 🖼 Screenshots

## Dashboard

![Dashboard](./images/dashboard.png)

## Profile Page

![Profile](./images/profile.png)

## 🚀 Installation

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or Atlas account)
- npm or yarn package manager

### Step 1: Clone the Repository
```bash
git clone https://github.com/yourusername/employee-management-system.git
cd employee-management-system
```

### Step 2: Backend Setup
```bash
cd backend
npm install
```

Create a `.env` file in the `backend` directory with the following variables:
```env
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
PORT=5000
NODE_ENV=development
```

### Step 3: Frontend Setup
```bash
cd ../frontend
npm install
```

### Step 4: Run the Application

**Option 1: Run both servers concurrently (Recommended)**
```bash
cd backend
npm run ems
```

**Option 2: Run separately**

Backend:
```bash
cd backend
npm start
```

Frontend (in a new terminal):
```bash
cd frontend
npm start
```

The application will be available at:
- Frontend: `http://localhost:3000`
- Backend API: `http://localhost:5000`

## 💡 Usage

### For Regular Users:
1. **Login** - Access the system using your credentials
2. **View Dashboard** - See your attendance summary and quick stats
3. **Mark Attendance** - Clock in/out for the day
4. **Apply for Leave** - Submit leave requests with date range and reason
5. **View Profile** - Check and update your personal information
6. **Track Attendance** - View your monthly attendance calendar and reports

### For Super Admin:
1. **Employee Management** - Add, edit, or remove employee records
2. **Approve Leaves** - Review and approve/reject leave requests
3. **View Reports** - Access comprehensive attendance and leave reports
4. **Monitor Attendance** - Track late arrivals and overall attendance metrics
5. **Manage All Profiles** - View and edit all employee profiles
6. **Dashboard Analytics** - View organization-wide statistics and trends

## 🔑 Default Credentials
After setup, you can create a super admin account through the backend or database directly.

## 🎯 Key Highlights

- ✅ **Responsive Design** - Works seamlessly on desktop, tablet, and mobile
- ✅ **Real-time Updates** - Live attendance tracking and leave status
- ✅ **Data Visualization** - Interactive charts and graphs for better insights
- ✅ **Secure Authentication** - JWT-based secure login system
- ✅ **File Upload** - Profile picture upload with image optimization
- ✅ **RESTful API** - Well-structured backend API endpoints
- ✅ **Scalable Architecture** - Modular code structure for easy maintenance
- ✅ **Error Handling** - Comprehensive error handling and validation
