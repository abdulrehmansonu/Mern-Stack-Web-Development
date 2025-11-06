# 🛍️ E-Commerce CRUD API — Node.js, Express & MongoDB

[![Node.js](https://img.shields.io/badge/Node.js-18-green?logo=node.js)](https://nodejs.org)
[![Express.js](https://img.shields.io/badge/Express-Framework-lightgrey?logo=express)](https://expressjs.com)
[![MongoDB](https://img.shields.io/badge/MongoDB-Database-green?logo=mongodb)](https://mongodb.com)
[![License](https://img.shields.io/badge/License-ISC-yellow)](LICENSE)

A **RESTful E-Commerce CRUD API** built with **Node.js, Express, and MongoDB (Mongoose)**.  
Supports **User Authentication (JWT)**, **Product Management**, and **CRUD Operations** with secure token-based access.

---

## 🚀 Features

✅ User Sign-Up / Login / Logout (JWT Auth)  
✅ Password Hashing using bcrypt-inzi  
✅ Cookie-based token management (HTTP-only cookies)  
✅ CRUD for Products: Create, Read, Update, Delete  
✅ MongoDB connection handling with real-time connection status logs  
✅ Secure, scalable backend suitable for full-stack e-commerce projects  

---

## 🧠 Tech Stack

- **Backend:** Node.js, Express.js  
- **Database:** MongoDB (via Mongoose ORM)  
- **Security:** JSON Web Tokens (JWT), bcrypt-inzi  
- **Utilities:** cookie-parser, cors  
- **Dev Tooling:** nodemon  

---

## ⚙️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd ecommerce-crud
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   Create a `.env` file in the project root:
   ```bash
   MONGODBURI=your_mongodb_connection_string
   SECRET=your_jwt_secret
   PORT=5001
   ```

4. **Run the server**
   ```bash
   npm run dev
   ```
   or for production:
   ```bash
   npm start
   ```

---

## 📦 API Endpoints

| Method | Endpoint | Description |
|--------|-----------|-------------|
| **POST** | `/signup` | Register a new user |
| **POST** | `/login` | Login and receive JWT token |
| **POST** | `/logout` | Logout and clear cookie |
| **GET** | `/profile` | Get logged-in user details |
| **GET** | `/products` | Fetch all products |
| **GET** | `/product/:id` | Fetch a product by ID |
| **POST** | `/product` | Add a new product |
| **PUT** | `/product/:id` | Update existing product |
| **DELETE** | `/product/:id` | Delete a product |

---

## 🧪 Example JSON for Product

```json
{
  "name": "Nike Air Zoom",
  "description": "High performance running shoes",
  "price": "150",
  "code": "NK001"
}
```

---

## 🧩 Project Structure

```
ecommerce-crud/
├── server.mjs
├── package.json
├── package-lock.json
├── .env
└── README.md
```

---

## 🔒 Security Notes

- All protected routes require a valid JWT in cookies.  
- HTTP-only cookies prevent XSS attacks.  
- Passwords are stored in hashed form using `bcrypt-inzi`.

---

## 🧑‍💻 Author

**Abdul Rehman Sonu**  
Backend Developer | MERN Stack Enthusiast  
🔗 [GitHub](https://github.com/abdulrehmansonu) • [LinkedIn](https://www.linkedin.com/in/abdulrehmansonu/)

---

⭐ *If you find this project helpful, please star the repo!*
