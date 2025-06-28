# 📇 Contact Manager App (Backend API)

This is a RESTful API built with **Node.js**, **Express**, and **MongoDB** for managing user contacts. Users can register, log in, and securely manage their personal contacts.

---

## 🚀 Features

- ✅ User Registration & Login (JWT-based Authentication)  
- ✅ Create, Read, Update, Delete (CRUD) Contacts  
- ✅ Protected routes with token validation  
- ✅ Password hashing using bcrypt  
- ✅ MongoDB connection using Mongoose  

---

## 🛠️ Technologies Used

- Node.js  
- Express.js  
- MongoDB + Mongoose  
- JWT (jsonwebtoken)  
- bcrypt  
- dotenv  

---

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/contact-manager-app.git
   cd contact-manager-app
Install dependencies

bash
Copy
Edit
npm install
Configure environment variables
Create a .env file in the root directory:

ini
Copy
Edit
PORT=5000
CONNECTION_STRING=your_mongodb_connection_uri
ACCESS_TOKEN_SECRET=your_secret_key
Run the server

Development:

bash
Copy
Edit
npm run dev
Production:

bash
Copy
Edit
npm start
📬 API Endpoints
🔐 Auth Routes
Method	Endpoint	Description
POST	/api/users/register	Register user
POST	/api/users/login	Login user
GET	/api/users/current	Get current user

📇 Contact Routes (Protected)
Method	Endpoint	Description
GET	/api/contacts	Get all contacts
POST	/api/contacts	Create new contact
GET	/api/contacts/:id	Get contact by ID
PUT	/api/contacts/:id	Update contact
DELETE	/api/contacts/:id	Delete contact

🔐 Auth Header
For all protected routes, include the JWT token in headers:

makefile
Copy
Edit
Authorization: Bearer <your_access_token>
👤 Author
Name: Rohit Soni

College: NIT Raipur

Branch: Electronics and Communication Engineering
