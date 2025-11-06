
# JWT Authentication System (React + Node + MongoDB)

![Node.js](https://img.shields.io/badge/Backend-Node.js-green?style=for-the-badge)
![Express.js](https://img.shields.io/badge/Framework-Express.js-lightgrey?style=for-the-badge)
![MongoDB](https://img.shields.io/badge/Database-MongoDB-brightgreen?style=for-the-badge)
![React](https://img.shields.io/badge/Frontend-React-blue?style=for-the-badge)
![JWT](https://img.shields.io/badge/Auth-JWT-yellow?style=for-the-badge)

A complete **JWT-based Authentication System** built with the **MERN Stack**.  
Users can **Sign Up**, **Log In**, and access **protected dashboard pages**.  
Authentication tokens are stored using **HTTP-only cookies** for enhanced security.

---

## 🚀 Key Features

- User **Signup & Login**
- Password hashing using **bcrypt-inzi**
- **JWT Authentication** with expiration
- **HTTP-only Cookies** for secure token handling
- Protected routes (only authenticated users can access dashboard/profile)
- Logout functionality
- Clean and modular code structure

---

## 🛠️ Tech Stack 

| Layer | Technology |
|------|------------|
| Frontend | React.js, React Router, Fetch/Axios |
| Backend | Node.js, Express.js |
| Database | MongoDB + Mongoose |
| Authentication | JWT (jsonwebtoken) |
| Password Security | bcrypt-inzi |
| Cookies | cookie-parser |
| CORS Handling | cors |

---

## 📁 Folder Structure

```
Project/
│
├── backend/
│   ├── server.mjs
│   ├── package.json
│   ├── ...
│
└── frontend/
    ├── src/
    │   ├── components/
    │   │   ├── Login.jsx
    │   │   ├── Signup.jsx
    │   │   └── Dashboard.jsx
    │   └── App.js
    └── package.json
```

---

## 📌 API Routes

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/signup` | Register a new user |
| POST | `/login` | Authenticate user + issue JWT cookie |
| POST | `/logout` | Clear session cookie |
| GET | `/profile` | Get logged-in user's profile (Protected) |
| GET | `/users` | Get all users (Protected) |

---

## 🔐 Authentication Workflow

```
User Login →
Password Verified →
JWT Created →
Token Stored in HTTP-only Cookie →
Protected Routes Check Token →
Access Granted ✅
```

---

## ▶️ How to Run the Project

### 1) Run Backend

```
cd backend
npm install
npm run dev
```

Set environment variables:

```
MONGODBURI=your-mongodb-connection-string
SECRET=your-jwt-secret
```

### 2) Run Frontend

```
cd frontend
npm install
npm start
```

---

## ✅ Security Note

Using **HTTP-only cookies** prevents JavaScript from accessing JWT token, reducing risk of **XSS attacks**  
and making the app more secure than localStorage-based authentication.

---

## © License
This project is open-source. Free to use & customize.
