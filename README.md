# Insurai
AI-powered insurance assistant for smart claim analysis and recommendations
 InsurAI – Insurance Management System

InsurAI is a full-stack web application developed as part of an academic milestone project.  
It focuses on **user authentication, email verification, password recovery, and agent availability management** for an insurance platform.

The system is designed to demonstrate backend development using **Node.js**, database integration using **MySQL**, and secure user workflows.

 🚀 Features

- User Registration & Login
- Email Verification using Gmail SMTP
- Forgot Password & Reset Password
- Role-based access (Customer / Agent)
- Agent Availability Management
- Secure token-based verification

---

## 🧑‍💼 User & Agent Modules

### 👤 User Module
- Register with email verification
- Login only after verification
- Reset password via email link

### 🧑‍💼 Agent Module
- Login as agent
- Set availability (date & time)
- View stored availability records


## 🛠️ Technologies Used

### Frontend
- HTML
- CSS
- JavaScript

### Backend
- Node.js
- Express.js

### Database
- MySQL

### Email Service
- Nodemailer (Gmail App Password)

## 🗄️ Database Design

### Users Table
- `id`
- `name`
- `email`
- `password`
- `role`
- `is_verified`
- `verification_token`
- `reset_token`

### Agent Availability Table
- `id`
- `agent_id` (Foreign Key → users.id)
- `available_date`
- `start_time`
- `end_time`

## 🔐 Authentication Flow

1. User registers with email & password
2. Verification email is sent
3. User clicks verification link
4. Account is activated
5. User can log in
6. Password reset is available via email

---

## ▶️ How to Run the Project

### 1️⃣ Install Dependencies
```bash
npm install

2️⃣ Start server

node server.js


