# 📦 Product Management API – Node.js, Express & MongoDB

---

## 📘 Overview

A robust RESTful API for managing product data, built with **Node.js**, **Express**, and **MongoDB**. This project demonstrates a full set of **CRUD (Create, Read, Update, Delete)** operations with proper routing, validation, and modular code architecture.

Designed for scalability and real-world integration with frontend apps (React, Vue, Angular) or mobile clients.

---

## 🧩 Core Features

- 📄 Create, Read, Update, Delete products
- 🔍 Retrieve individual products or all
- 🧱 Clean code architecture with separation of concerns
- 🧪 Tested via Postman and REST clients
- 🔐 Ready to integrate with authentication layer
- 🌍 Deployable to Heroku, Render, or VPS

---

## 🏗️ System Architecture

```
                        +------------------------+
                        |      Frontend App      |
                        |  (React / Mobile App)  |
                        +-----------+------------+
                                    |
                                    |
                        +-----------v------------+
                        |   Express.js API Layer  |
                        +-----------+------------+
                                    |
                    +-----------------------------+
                    |         Product Routes       |
                    |   - Create / Read / Update   |
                    |   - Delete / Get by ID       |
                    +-----------------------------+
                                    |
                        +-----------v------------+
                        |     MongoDB Database    |
                        |  (Products Collection)  |
                        +------------------------+
```

---

## ⚙️ Tech Stack

| Layer         | Technology        |
|---------------|------------------|
| Backend       | Node.js, Express |
| Database      | MongoDB (Mongoose) |
| Tools         | Postman, Git     |
| Deployment    | Heroku / Render  |

---

## 📁 Folder Structure

```
project-root/
│
├── config/               # MongoDB connection
├── controllers/          # CRUD logic
├── models/               # Mongoose schema
├── routes/               # Express routes
├── .env                  # Environment variables
└── server.js             # Entry point
```

---

## 🚀 Getting Started

### 1. Clone the repo
```bash
git clone https://github.com/abdulrehmansonu/Mern-Stack-Web-Development.git
```

### 2. Navigate to the project
```bash
cd "03.nodejs/8.product list (CRUD operation)"
```

### 3. Install dependencies
```bash
npm install
```

### 4. Create `.env` file and configure:
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
```

### 5. Run the server
```bash
npm start
```

---

## 🔗 API Endpoints

### 📌 Products

| Method | Endpoint        | Description                |
|--------|------------------|----------------------------|
| POST   | `/api/products`  | Create a new product       |
| GET    | `/api/products`  | Get all products           |
| GET    | `/api/products/:id` | Get product by ID       |
| PUT    | `/api/products/:id` | Update product by ID    |
| DELETE | `/api/products/:id` | Delete product by ID    |

---

## 🔐 Future Enhancements

- 🔑 Add JWT-based auth for protected routes
- 🧑‍💼 Add user ownership per product
- 🛒 Connect to cart/checkout logic (eCommerce-ready)
- 📦 Pagination & filtering for large datasets

---

## 🌐 Deployment Ready

You can deploy this backend easily on:

- Heroku ✅
- Render ✅
- Railway ✅
- VPS / Docker ✅

Just set the environment variables in your dashboard or `.env` file.

---

## 👨‍💻 Author

**Abdul Rehman**  
Backend Developer | REST API Specialist | MERN Stack  
📧 Email: your-email@example.com  
🌍 Portfolio: [abdulrehman.xyz](https://abdulrehman.xyz)  
🐙 GitHub: [@abdulrehmansonu](https://github.com/abdulrehmansonu)

---

## 📄 License

This project is licensed under the MIT License. Free to use and extend.

---

## 🤝 Looking for a Backend Expert?

> I build secure, production-grade APIs for mobile and web applications.  
> Available for freelance and full-time opportunities — let's connect!
