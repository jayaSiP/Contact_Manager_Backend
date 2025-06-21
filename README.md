# # 📞 Contact Manager Backend API

A secure and powerful backend system for managing personal contacts — built with **Node.js**, **Express**, **MongoDB**, and **JWT authentication**. 

> 💬 Tested with Thunder Client (because who wants to open Postman every time? 😎)

---

## 🚀 Features

✨ **User Authentication**
- Register new users with **hashed passwords** (🔐 using `bcrypt`)
- Login with JWT-based tokens
- Protected routes with middleware

📇 **Contact Management**
- CRUD (Create, Read, Update, Delete) operations for contacts
- Contacts are linked to individual users only (🔐 secure & scoped)

🛡️ **Authorization & Validation**
- Only authenticated users can access/modify their own contacts
- Backend input validation and structured error handling

🧪 **Tested with Thunder Client**
- All endpoints tested and verified using VS Code’s built-in REST client plugin – **Thunder Client** ⚡

---

## 🛠️ Tech Stack

| Tool | Usage |
|------|-------|
| 🟢 Node.js | Backend runtime |
| 🚀 Express | REST API framework |
| 🍃 MongoDB | Database |
| 🔐 bcrypt | Password hashing |
| 🪪 JWT | Secure authentication |
| ⚡ Thunder Client | API testing |

---

## 📁 Project Structure

