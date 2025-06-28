📇 Contact Manager API
A RESTful API for managing contacts, built with Node.js, Express, MongoDB, and JWT authentication.

🚀 Features
User registration and login

JWT-based authentication

CRUD operations on contacts (Create, Read, Update, Delete)

Protected routes using middleware

MongoDB with Mongoose for database operations

Error handling middleware

🛠 Tech Stack
Node.js

Express.js

MongoDB (via Mongoose)

JWT (jsonwebtoken)

bcrypt

dotenv

📁 Project Structure
lua
Copy
Edit
├── config/
│   └── dbConnection.js
├── controllers/
│   ├── contactController.js
│   └── userController.js
├── middleware/
│   ├── errorHandler.js
│   └── validateTokenHandler.js
├── models/
│   ├── contactModel.js
│   └── userModel.js
├── routes/
│   ├── contactRoutes.js
│   └── userRoutes.js
├── .env
├── .gitignore
├── package.json
├── server.js
🔐 Environment Variables
Create a .env file in the root folder with:

ini
Copy
Edit
PORT=5000
CONNECTION_STRING=your_mongodb_connection_uri
ACCESS_TOKEN_SECRET=your_jwt_secret_key
🚦 Installation & Run
bash
Copy
Edit
# Clone the repository
git clone https://github.com/yourusername/contact-manager-app.git
cd contact-manager-app

# Install dependencies
npm install

# Run in dev mode
npm run dev

# Or run in production
npm start
📮 API Endpoints
🔑 Auth Routes (Public)
POST /api/users/register – Register user

POST /api/users/login – Login and receive token

👤 User Info (Private)
GET /api/users/current – Get current user (requires token)

📇 Contact Routes (Private)
GET /api/contacts – Get all contacts

POST /api/contacts – Create a new contact

GET /api/contacts/:id – Get contact by ID

PUT /api/contacts/:id – Update contact by ID

DELETE /api/contacts/:id – Delete contact by ID

🛡 Add Authorization: Bearer <access_token> in headers for private routes.

✅ Sample Request Headers
http
Copy
Edit
Authorization: Bearer your_jwt_token
Content-Type: application/json
👤 Author
Name: Rohit Soni

College: NIT Raipur

Branch: Electronics and Communication Engineering
