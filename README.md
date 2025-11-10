# 🛒 ShopHut - Multi-Vendor E-commerce Platform

**ShopHut** is a modern **full-stack E-commerce web application** designed with a **multi-vendor/multi-seller system**, allowing multiple independent shops to sell their products on one unified platform.  
It features **dedicated dashboards** for **Users**, **Sellers**, and **Administrators**, providing a complete marketplace experience similar to **Amazon Marketplace** or **Etsy**.

---

## 🚀 Project Overview

ShopHut is built with a **scalable, modular architecture** divided into three components:

1. **Backend API** – Built using Node.js & Express.
2. **Frontend Web Application** – Developed with React & Redux Toolkit.
3. **Socket Server** – Handles real-time communication (chat & notifications).

This architecture ensures a smooth, responsive, and real-time shopping experience.

---

## 🧩 Architecture Overview

```
📦 ShopHut
├── 📁 backend          # Express + MongoDB REST API
│   ├── models/         # Mongoose models
│   ├── controllers/    # Route logic & business rules
│   ├── routes/         # API endpoints
│   ├── utils/          # Helpers (email, payments, etc.)
│   └── server.js       # Entry point
│
├── 📁 frontend         # React-based user interface
│   ├── src/
│   │   ├── components/ # Reusable UI components
│   │   ├── redux/      # Redux Toolkit slices
│   │   ├── pages/      # App pages (User, Seller, Admin)
│   │   └── App.js
│   └── package.json
│
├── 📁 socket           # Real-time server using Socket.io
│   └── server.js
│
└── 📄 README.md
```

---

## 🛠️ Technology Stack

### **Backend (Node.js + Express)**

| Category | Technology | Purpose |
|-----------|-------------|----------|
| **Server** | Node.js (v18.x), Express | Core backend framework |
| **Database** | MongoDB (Mongoose ODM) | Data storage and modeling |
| **Authentication** | bcrypt, jsonwebtoken, cookie-parser | Secure auth for users and sellers |
| **Payments** | Stripe | Payment gateway integration |
| **External Services** | Cloudinary, Nodemailer | Image hosting and email notifications |

---

### **Frontend (React)**

| Category | Technology | Purpose |
|-----------|-------------|----------|
| **Framework** | React | Single-page UI development |
| **State Management** | Redux Toolkit, react-redux | Global state handling |
| **Styling** | Tailwind CSS, Material UI | Responsive and elegant design |
| **Routing** | react-router-dom | Navigation & protected routes |
| **Real-time** | socket.io-client | Messaging & live updates |
| **Payments** | @stripe/react-stripe-js, @paypal/react-paypal-js | Payment UI components |

---

### **Real-time Socket Server**

| Technology | Purpose |
|-------------|----------|
| socket.io | Enables chat, live notifications, and order updates |
| express, cors | Minimal web server setup for socket connections |

---

## ✨ Core Features

### 👥 **User & Shop Features**
- 🔐 Secure registration, login, and profile management.
- 🛍️ Product browsing, wishlist, and shopping cart.
- 🚚 Order tracking and status updates.
- 💬 Real-time messaging between users and sellers.
- 💳 Multi-step checkout with Stripe & PayPal payments.
- 💸 Refund request and order management.
- ⭐ Product reviews & ratings.

---

### 🏪 **Seller (Shop) Dashboard**
- 🏷️ Create and manage products.
- 🎉 Manage flash sales and promotional events.
- 🎟️ Coupon creation and discount management.
- 📦 Handle customer orders and shipping.
- 💰 Request withdrawals from admin.
- 💬 Chat directly with customers via real-time inbox.

---

### 🧑‍💼 **Admin Dashboard**
- 👤 Manage all users, sellers, and shops.
- 🧾 Monitor all orders, products, and events.
- 💵 Handle seller withdrawal requests.
- ⚙️ Oversee platform-wide settings and data.

---

## ⚙️ Getting Started

### **1. Prerequisites**
Make sure you have the following installed:
- **Node.js (v18.x recommended)**
- **MongoDB** (Local or Atlas Cloud)
- **Cloudinary Account**
- **Stripe Account**

---

### **2. Backend Setup**
```bash
cd backend
npm install

# Create .env file and configure the following:
MONGO_URL=your_mongo_connection_string
JWT_SECRET_KEY=your_secret
STRIPE_API_KEY=your_stripe_api_key
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_cloud_key
CLOUDINARY_API_SECRET=your_cloud_secret

npm run dev
```

---

### **3. Frontend Setup**
```bash
cd frontend
npm install

# .env configuration
REACT_APP_API_URL=http://localhost:8000
REACT_APP_STRIPE_PUBLIC_KEY=your_stripe_public_key
REACT_APP_PAYPAL_CLIENT_ID=your_paypal_client_id

npm start
```

---

### **4. Socket Server Setup**
```bash
cd socket
npm install

# Create .env
PORT=4000
CORS_ORIGIN=http://localhost:3000

npm start
```

---

## 🧠 Learning & Development Focus
- REST API Design and CRUD Operations  
- Authentication and Authorization (JWT + Cookies)  
- Secure Payment Integration  
- File Uploads with Cloudinary  
- Email Notification System (Nodemailer)  
- Real-time Chat using Socket.io  
- Scalable State Management with Redux Toolkit  
- Modular Code Architecture  

---

## 🧰 Scripts

| Command | Description |
|----------|-------------|
| `npm start` | Start the application |
| `npm run dev` | Start in development mode |
| `npm run build` | Build production frontend |

---

## 📄 License

This project is licensed under the **MIT License** – you are free to use, modify, and distribute it with attribution.

---

## 💬 Contact

**Author:** Your Name  
**GitHub:** [@yourgithubusername](https://github.com/yourgithubusername)  
**Email:** your.email@example.com  

