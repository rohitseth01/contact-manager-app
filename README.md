# Contact Manager App (Backend API)

This is a RESTful API built with **Node.js**, **Express**, and **MongoDB** for managing user contacts. Users can register, log in, and securely manage their personal contacts.

## 🚀 Features

- User Registration & Login (JWT-based Authentication)
- Create, Read, Update, Delete (CRUD) Contacts
- Protected routes with token validation
- Password hashing using bcrypt
- MongoDB connection using Mongoose

## 🛠️ Technologies Used

- Node.js
- Express.js
- MongoDB (Mongoose)
- JWT (jsonwebtoken)
- bcrypt
- dotenv

## 📦 Installation

1. **Clone the repository**

git clone https://github.com/your-username/contact-manager-app.git
cd contact-manager-app

2.Install dependencies

npm install
Configure environment variables

3.Create a .env file in the root directory:

PORT=5000
CONNECTION_STRING=mongodb+srv://<username>:<password>@cluster0.mongodb.net
ACCESS_TOKEN_SECRET=your_secret_key

4.Run the server

# Development
npm run dev

# Production
npm start

📬 API Endpoints

Auth Routes
Method	Endpoint	Description---
POST	/api/users/register	Register user
POST	/api/users/login	Login user
GET	/api/users/current	Get current user

Contact Routes (Protected)
Method	Endpoint	Description---
GET	/api/contacts	Get all contacts
POST	/api/contacts	Create a new contact
GET	/api/contacts/:id	Get a contact by ID
PUT	/api/contacts/:id	Update a contact
DELETE	/api/contacts/:id	Delete a contact

🔐 For protected routes, pass JWT in headers:
Authorization: Bearer <your_access_token>

