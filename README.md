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
- All endpoints tested and verified using VS Code’s built-in REST client plugin , no need to switch between POSTMAN and VSCODE – **Thunder Client** ⚡

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

Test it live at : https://contact-manager-backend-p5l2.onrender.com

Start your server locally

    Run: npm start

    Ensure it shows: Server running on port 5001

Register a new user

    Method: POST

    URL: http://localhost:5001/api/users/register

    Body (JSON):

    {
      "username": "Archana",
      "email": "archana@gmail.com",
      "password": "strongPassword123"
    }

    Click Send

Login the registered user

    Method: POST

    URL: http://localhost:5001/api/users/login

    Body (JSON):

    {
      "email": "archana@gmail.com",
      "password": "strongPassword123"
    }

    Click Send

    Copy the accessToken from the response

Use the token for protected routes

    In Thunder Client/Postman, go to Headers

    Add:

    Key: Authorization
    Value: Bearer <paste your token here>

Create a new contact

    Method: POST

    URL: http://localhost:5001/api/contacts

    Headers:

        Authorization: Bearer <your_token>

    Body (JSON):

    {
      "name": "Jaya",
      "email": "jaya@example.com",
      "phone": "9999999999"
    }

    Click Send

Get all contacts

    Method: GET

    URL: http://localhost:5001/api/contacts

    Headers:

        Authorization: Bearer <your_token>

    Click Send
