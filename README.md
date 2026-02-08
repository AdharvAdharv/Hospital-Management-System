# 🏥 Hospital Management System

## 📌 Project Overview
The **Hospital Management System** is a web application designed to streamline hospital operations. It allows patients to book and manage their appointments while providing administrators with tools to handle doctors, appointments, and user data. Built using the **MERN Stack**, the system ensures a seamless and efficient healthcare management experience.

### 🎯 Objectives
- Enhance hospital appointment management
- Reduce manual work for hospital staff
- Improve the patient experience with easy booking and profile management
- Provide an intuitive admin dashboard for better control over hospital operations


## ✨ Features

### 👤 User Module
- 📝 Register
- 🔐 Login
- 📅 Book Appointment
- 📜 View Previous Appointments
- ❌ Cancel Appointments
- 🏷️ View & Edit Profile
- 🚪 Logout

### 🛠️ Admin Module
- 🔑 Login
- ➕ Create Doctor
- 📝 Edit & Manage Doctors
- 👥 View Registered Users
- 📆 View Appointments

---

## 🛠 Technologies Used
- **MongoDB** 🗄️ (Database)
- **Express.js** 🚀 (Backend Framework)
- **React.js** ⚛️ (Frontend Library)
- **Node.js** 🌳 (Runtime)
- **Tailwind CSS** 🎨 (Styling)

---

## 🔧 Other Tools & Libraries
- **JWT (JSON Web Token)** 🔑 (Authentication & Security)

---

## 🚀 Getting Started

### 🔄 Clone the Repository
```bash
git clone <Repository-url/>
cd Hospital-Management-System

```

### 📦 Install Dependencies

### Frontend
```bash
cd hospitalmanagement
npm install
```
### Backend
```bash
cd backend
npm install
```


### Backend Environment Setup (.env)

Create a .env file inside the backend folder.
```bash
cd backend
touch .env
```

Add the following content:
```bash
PORT=5000
SECRET_KEY=MARVEL
MONGO_URI=mongodb://localhost:27017/Hospital
```

⚠️ Make sure MongoDB is running on your system before starting the backend.

### ▶️ Run the Application
-Start Backend Server
```bash
cd backend
npm run dev
```

-You should see:

```bash
Server is listening at 5000
MongoDB connected successfully
```

-Start Frontend Server

-Open a new terminal:

```bash
cd hospitalmanagement
npm run dev
```

-You will get:
```bash
http://localhost:5001
```

-Open this in your browser.



### 🌐 API Configuration (Vite Proxy)

Make sure your vite.config.js is configured like this:
```bash

proxy: {
  '/api': {
    target: 'http://localhost:5000',
    changeOrigin: true,
    secure: false,
  }
}

```

This allows frontend and backend to communicate properly.


### 🔐 Security

-Passwords are encrypted

-JWT is used for authentication

-Protected routes for admin and users


Enjoy managing hospital appointments seamlessly! 🚀
