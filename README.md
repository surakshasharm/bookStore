# 📚 Book Store Web Application

A full-stack **Book Store Web Application** built using the **MERN stack (MongoDB, Express, React, Node.js)**.  
The application allows users to browse books and interact with the system through a modern web interface while the backend handles database operations and API requests.

This project demonstrates **full-stack development, REST API design, database integration, and frontend UI implementation.**

---

# 🚀 Features

- 📖 Browse available books
- 👤 User authentication system
- 📚 Book data stored in MongoDB
- 🔌 RESTful API for backend communication
- 🎨 Responsive frontend built with React
- ⚡ Fast development setup using Vite
- 🔒 Environment variable configuration using dotenv

---

# 🏗️ Tech Stack

## Frontend
- React.js
- Vite
- JavaScript
- CSS
- Axios (API communication)

## Backend
- Node.js
- Express.js
- MongoDB
- Mongoose
- CORS
- dotenv

---

# 📂 Project Structure
bookStoreApp
│
├── Backend
│ ├── controller
│ │ ├── book.controller.js
│ │ └── user.controller.js
│ │
│ ├── model
│ │ ├── book.model.js
│ │ └── user.model.js
│ │
│ ├── route
│ │ ├── book.route.js
│ │ └── user.route.js
│ │
│ └── index.js
│
├── Frontend
│ ├── src
│ │ ├── components
│ │ ├── App.jsx
│ │ └── main.jsx
│ │
│ ├── public
│ └── index.html
│
└── README.md

---

# ⚙️ Installation & Setup

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/bookstore-app.git
cd bookstore-app
2️⃣ Setup Backend
cd Backend
npm install
```

Create a .env file inside the Backend folder:

PORT=4000
MongoDBURI=your_mongodb_connection_string

Run the backend server:

npm start
3️⃣ Setup Frontend

Open a new terminal:

cd Frontend
npm install
npm run dev

The frontend will run on:

http://localhost:5173
🔌 API Endpoints
Book Routes
Method	Endpoint	Description
GET	/book	Get all books
POST	/book	Add a new book
User Routes
Method	Endpoint	Description
POST	/user/signup	Register a new user
POST	/user/login	User login
📸 Screenshots

Add screenshots of your application here.

Example:

Homepage

Book listing page

Login / Signup page

🎯 Learning Outcomes

This project helped in understanding:

Full stack application architecture

REST API development

MongoDB database integration

React component structure

Client-server communication

Environment configuration

📌 Future Improvements

Add book search functionality

Implement user authorization

Add book categories and filters

Improve UI design and responsiveness

Deploy application using cloud services

👩‍💻 Author

Suraksha Sharma
B.Tech CSE (Minor in Data Science)


If you want, I can also give you a **much stronger README (like top GitHub projects)** with:

- repo **badges**
- **demo section**
- **screenshots layout**
- **portfolio-ready styling**

It makes your GitHub look significantly more polished for recruiters. 🚀
