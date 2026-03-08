<div align="center">

# MERN AUTH 🔐

A complete Authentication System with **Email Verification** and **Password Reset** using a secure 6-digit OTP sent directly to the user's email.

</div>

<br /><hr /><br />

<div align="center">

</div>

<br /><hr /><br />

## Project Overview

This project is a **full-featured Authentication System** built with the **MERN Stack (MongoDB, Express, React, Node.js)** and **JWT (JsonWebToken)** for secure authentication.

### Key Features:

* **Email Verification**: Securely verify user email addresses.
* **Password Reset**: Reset passwords using a 6-digit OTP sent via email.
* **JWT Authentication**: Secure user login and route protection.

---

## Features

### Backend

* REST APIs for user authentication.
* **Email Verification** via OTP.
* **Password Reset** using OTP.
* Secure JWT-based authentication and authorization.

### Frontend

* Responsive UI built with **React** and **Tailwind CSS**.
* Pages for:

  * Login
  * Registration
  * Password Reset with OTP verification
* Fully integrated with backend APIs.

---

## Tech Stack

**Backend:**

* **Node.js** – Server-side runtime
* **Express.js** – API framework
* **MongoDB** – Database
* **JWT** – Token-based authentication

**Frontend:**

* **React** – UI library
* **Tailwind CSS** – Utility-first styling

---

## Installation & Setup

### Prerequisites

* Node.js installed
* MongoDB setup
* Valid email account for testing email verification (Gmail SMTP or similar)

### Backend Setup

```bash
# Clone repository
git clone <repository-url>

# Navigate to backend
cd server

# Install dependencies
npm install

# Configure environment variables in .env file
PORT=4000
MONGO_URI=<your-mongodb-uri>
JWT_SECRET=<your-jwt-secret>
SMTP_EMAIL=<your-email>
SMTP_PASSWORD=<your-email-password>

# Start backend server
npm run server
```

Backend runs at `http://localhost:4000`.

### Frontend Setup

```bash
# Navigate to frontend
cd client

# Install dependencies
npm install

# Start frontend
npm run dev
```

Frontend runs at `http://localhost:5173`.

---

## Project Structure

### Backend

```
server/
├── models/       # Mongoose models
├── routes/       # Express routes
├── controllers/  # Request handlers
├── utils/        # Utilities (email sender, OTP generator)
├── middleware/   # Authentication middleware
├── config/       # Configuration files
└── server.js     # Entry point
```

### Frontend

```
client/src/
├── assets/       # Images, templates, email templates
├── components/   # Reusable UI components (Header, Navbar)
├── context/      # App context & state management
├── pages/        # Pages (Login, Register, ResetPassword, EmailVerify)
├── App.jsx       # Main App component
├── index.css     # Global styles
└── main.jsx      # Frontend entry point
```

---

## Usage

1. **Register:** Sign up with your email. A 6-digit OTP will be sent for verification.
2. **Login:** Authenticate using email and password.
3. **Password Reset:** Enter your email to receive an OTP for resetting your password.

---

## Future Enhancements

* Multi-factor authentication (MFA)
* Rate limiting & captcha for security
* Social login support (Google, Facebook, etc.)