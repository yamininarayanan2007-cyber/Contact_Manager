# CONTACT_MANAGER
# 🔐 Secure Authentication System (Node.js + MongoDB)

A secure backend authentication system built using **Node.js, Express.js, MongoDB, JWT, and Bcrypt**.  
This project demonstrates user registration, login, password encryption, and protected route access using JSON Web Tokens.

---

## 🚀 Features

- ✅ User Registration (Signup)
- ✅ User Login
- ✅ Password Hashing using Bcrypt
- ✅ JWT Token Generation
- ✅ Protected Routes
- ✅ MongoDB Database Integration
- ✅ Error Handling (400, 401, etc.)

---

## 🛠️ Tech Stack

- **Backend:** Node.js, Express.js  
- **Database:** MongoDB  
- **Authentication:** JWT (JSON Web Token)  
- **Password Encryption:** Bcrypt  
- **Testing Tool:** Postman  

---

## 📂 Project Structure

```

project-folder/
│
├── models/
│   └── User.js
├── routes/
│   └── auth.js
├── middleware/
│   └── authMiddleware.js
├── controllers/
│   └── authController.js
├── server.js
├── package.json
└── .env

````

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/your-repo-name.git
````

### 2️⃣ Navigate to Project Folder

```bash
cd your-repo-name
```

### 3️⃣ Install Dependencies

```bash
npm install
```

### 4️⃣ Create `.env` File



### 5️⃣ Start the Server

```bash
npm start
```

Server will run on:

```
http://localhost:5000
```

---

## 🔐 API Endpoints

### 🟢 Register User

**POST** `/api/auth/register`

**Body (JSON):**

```json
{
  "name": "Yamini",
  "email": "yamini@gmail.com",
  "password": "123456"
}
```

---

### 🔵 Login User

**POST** `/api/auth/login`

**Body (JSON):**

```json
{
  "email": "yamini@gmail.com",
  "password": "123456"
}
```

**Response:**

```json
{
  "token": "your_jwt_token_here",
  "user": {
    "id": "mongo_user_id",
    "name": "Yamini",
    "email": "yamini@gmail.com"
  }
}
```

---

### 🟡 Protected Route

**GET** `/api/auth/me`

**Headers:**

```
Authorization: Bearer your_jwt_token_here
```

---

## 🔒 Security Implementation

* Passwords are hashed using **bcrypt**
* Authentication handled using **JWT**
* Protected routes require valid token
* Proper HTTP status codes used:

  * `400 Bad Request`
  * `401 Unauthorized`
  * `500 Server Error`

---

## 🧪 Testing

All APIs were tested using **Postman**.

---

## 📹 Project Demonstration

🎥 Project Demo Video
📄 Documentation Report

---

## 📌 Conclusion

This project demonstrates a secure and scalable backend authentication system that follows modern web security standards.

