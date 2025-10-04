# 🔐 Secure Authentication API – Node.js, Express & MongoDB

---

## 📘 Overview

A clean, modular, and secure authentication system built using **Node.js**, **Express**, and **MongoDB**. Designed for production-ready applications that require reliable user registration and login functionality with **JWT-based token authentication** and **bcrypt password encryption**.

This backend system is **frontend-agnostic** and can easily integrate with React, Vue, Angular, or mobile clients.

---

## 🧩 Key Features

- 🔑 JWT-based user login (stateless, secure)
- 🔒 Password hashing using bcrypt (one-way encryption)
- 🧱 Modular code structure (controllers, models, routes)
- 🧪 Fully tested with Postman
- 🌍 Easily deployable (Heroku, Render, Railway)
- ⚙️ Ready for scaling with role-based access, email auth, etc.

---

## 🏗️ System Architecture

```
                        +------------------------+
                        |      Frontend App      |
                        |  (React, Vue, Mobile)  |
                        +-----------+------------+
                                    |
                                    |
                        +-----------v------------+
                        |  Express.js API Server  |
                        +-----------+------------+
                                    |
                   +-------------------------------+
                   |         Auth Controller       |
                   |   - JWT Signing / Verification|
                   |   - Bcrypt Password Hashing   |
                   +-------------------------------+
                                    |
                        +-----------v------------+
                        |     MongoDB Database    |
                        |    (Users Collection)   |
                        +------------------------+
```

---

## ⚙️ Tech Stack

| Layer         | Technology        |
|---------------|------------------|
| Backend       | Node.js, Express |
| Database      | MongoDB (Mongoose) |
| Auth System   | JWT, bcrypt      |
| Tools         | Postman, Git     |
| Deployment    | Heroku / Render  |

---

## 📁 Folder Structure

```
project-root/
│
├── config/               # DB connection
├── controllers/          # Business logic
├── models/               # Mongoose schema
├── routes/               # Route handlers
├── middleware/           # Auth middleware
├── .env                  # Env variables
└── server.js             # App entry point
```

---

## 🚀 Getting Started

### 1. Clone the repo
```bash
git clone https://github.com/abdulrehmansonu/Mern-Stack-Web-Development.git
```

### 2. Navigate to the project folder
```bash
cd "03.nodejs/7.express login signup with database"
```

### 3. Install dependencies
```bash
npm install
```

### 4. Set environment variables in `.env`
```env
PORT=5000
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_secret_key
```

### 5. Start the server
```bash
npm start
```

---

## 🔗 API Endpoints

| Method | Endpoint        | Description             |
|--------|------------------|-------------------------|
| POST   | `/api/register`  | Register new user       |
| POST   | `/api/login`     | Login and receive token |

- Responses include a signed **JWT token**
- Use token in `Authorization` header for protected routes

---

## 🔐 Security Practices

- ✅ Passwords hashed before storing (bcrypt)
- ✅ Tokens signed using environment secret (JWT)
- ✅ No sensitive data hardcoded
- ✅ Validation & error handling for all inputs

---

## 🔄 Scalability Ready

This project is written with future scalability in mind. You can easily extend it to include:

- 🧑‍💼 Role-based access (admin/user)
- 📧 Email verification
- 🔁 Token refresh system
- 🛡️ Rate limiting & brute-force protection

---

## 🌐 Deployment Ready

Compatible with most Node-supporting platforms:

- Heroku ✅
- Render ✅
- Railway ✅
- VPS / Docker ✅

Use `dotenv` for environment variables, and don't forget to whitelist your IPs in MongoDB Atlas.

---

## 👨‍💻 Author

**Abdul Rehman**  
Backend Developer | Node.js | MongoDB | API Architect  
📧 Email: your-email@example.com  
🌍 Portfolio: [abdulrehman.xyz](https://abdulrehman.xyz)
🐙 GitHub: [@abdulrehmansonu](https://github.com/abdulrehmansonu)

---

## 📄 License

Licensed under the [MIT License](LICENSE).

---

## 🤝 Let's Work Together

> Looking to build a secure backend for your app?  
> I specialize in **modular, scalable APIs** for startups and enterprise-grade apps.  
> Contact me today to get started!
