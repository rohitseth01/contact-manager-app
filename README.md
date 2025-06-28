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

## 📦 Installation & Setup

```bash
# 1. Clone the repository
git clone https://github.com/your-username/contact-manager-app.git
cd contact-manager-app

# 2. Install dependencies
npm install

# 3. Create a .env file in the root directory and add:
PORT=5000
CONNECTION_STRING=your_mongodb_connection_uri
ACCESS_TOKEN_SECRET=your_jwt_secret_key

# 4. Start the development server
npm run dev

# For production build
npm start

📁 Project Structure
lua
Copy
Edit
contact-manager-app/
│
├── controllers/
│   ├── contactController.js
│   └── userController.js
│
├── models/
│   ├── contactModel.js
│   └── userModel.js
│
├── routes/
│   ├── contactRoutes.js
│   └── userRoutes.js
│
├── middleware/
│   ├── errorHandler.js
│   └── validateTokenHandler.js
│
├── config/
│   └── dbConnection.js
│
├── .env
├── .gitignore
├── server.js
├── package.json
└── README.md
🌐 API Endpoints
🔐 User Auth Routes
Method	Endpoint	Description
POST	/api/users/register	Register user
POST	/api/users/login	Login user
GET	/api/users/current	Get current user (protected)

📇 Contact Routes (Protected)
Method	Endpoint	Description
GET	/api/contacts	Get all contacts
POST	/api/contacts	Create new contact
GET	/api/contacts/:id	Get contact by ID
PUT	/api/contacts/:id	Update contact
DELETE	/api/contacts/:id	Delete contact

🔐 Authentication Header (Required for Protected Routes)
Add the following header to all protected routes after login:

makefile
Copy
Edit
Authorization: Bearer <your_access_token>
🛑 .gitignore
Make sure your project has a .gitignore file with the following contents to avoid pushing sensitive/local files:

lua
Copy
Edit
node_modules/
.env
*.log
npm-debug.log*
👤 Author
Name: Rohit Soni

College: NIT Raipur

Branch: Electronics and Communication Engineering (ECE)

Year: 3rd Year

Tech Stack: MERN Stack Developer

vbnet
Copy
Edit
