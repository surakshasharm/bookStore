# 📚 BookStore App

A full-stack **MERN** (MongoDB, Express, React, Node.js) bookstore web application where users can browse books, explore free and paid courses, and access protected content after authentication.

---

## 🚀 Features

- 🏠 **Home Page** — Hero banner with a responsive navbar and featured book sections
- 📖 **Free Books Section** — Carousel slider showcasing free-category books fetched from the database
- 🔐 **Authentication** — User signup and login with hashed passwords using `bcryptjs`
- 🛡️ **Protected Routes** — The courses page is accessible only to logged-in users
- 🌙 **Dark Mode** — Toggle between light and dark themes, with preference saved to `localStorage`
- 📱 **Responsive Design** — Mobile-first layout using Tailwind CSS and DaisyUI
- 🔔 **Toast Notifications** — Real-time feedback via `react-hot-toast`

---

## 🛠️ Tech Stack

### Frontend
| Technology | Purpose |
|---|---|
| React 18 | UI Library |
| React Router DOM v6 | Client-side routing |
| Tailwind CSS + DaisyUI | Styling & components |
| Axios | HTTP requests |
| React Hook Form | Form handling |
| React Slick | Book carousel slider |
| React Hot Toast | Notifications |
| Vite | Build tool |

### Backend
| Technology | Purpose |
|---|---|
| Node.js + Express | REST API server |
| MongoDB + Mongoose | Database & ODM |
| bcryptjs | Password hashing |
| dotenv | Environment variable management |
| CORS | Cross-origin requests |
| Nodemon | Development auto-restart |

---

## 📁 Project Structure

```
bookStoreApp/
├── Backend/
│   ├── controller/
│   │   ├── book.controller.js      # Get all books
│   │   └── user.controller.js      # Signup & Login logic
│   ├── model/
│   │   ├── book.model.js           # Book schema (name, price, category, image, title)
│   │   └── user.model.js           # User schema (fullname, email, password)
│   ├── route/
│   │   ├── book.route.js           # /book routes
│   │   └── user.route.js           # /user routes
│   ├── index.js                    # Express app entry point
│   └── package.json
│
└── Frontend/
    ├── src/
    │   ├── components/
    │   │   ├── Banner.jsx           # Hero section
    │   │   ├── Cards.jsx            # Book card component
    │   │   ├── Course.jsx           # All books grid
    │   │   ├── Footer.jsx           # Footer
    │   │   ├── Freebook.jsx         # Free books carousel
    │   │   ├── Login.jsx            # Login modal
    │   │   ├── Logout.jsx           # Logout button
    │   │   ├── Navbar.jsx           # Navigation bar
    │   │   └── Signup.jsx           # Signup page
    │   ├── context/
    │   │   └── AuthProvider.jsx     # Global auth context
    │   ├── courses/
    │   │   └── Courses.jsx          # Courses page
    │   ├── home/
    │   │   └── Home.jsx             # Home page
    │   ├── App.jsx                  # Routes configuration
    │   └── main.jsx                 # React entry point
    └── package.json
```

---

## ⚙️ Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or above)
- [MongoDB](https://www.mongodb.com/) (local instance or MongoDB Atlas)

---

### 1. Clone the Repository

```bash
git clone https://github.com/surakshasharm/bookStoreApp.git
cd bookStoreApp
```

---

### 2. Backend Setup

```bash
cd Backend
npm install
```

Create a `.env` file inside the `Backend` directory:

```env
PORT=4000
MongoDBURI=your_mongodb_connection_string_here
```

Start the backend server:

```bash
npm start
```

The server will run at `http://localhost:4000`

---

### 3. Frontend Setup

```bash
cd ../Frontend
npm install
npm run dev
```

The app will run at `http://localhost:5173`

---

## 🔌 API Endpoints

### Books
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/book` | Fetch all books |

### Users
| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/user/signup` | Register a new user |
| POST | `/user/login` | Login an existing user |

---

## 🔒 Authentication Flow

1. User registers via the **Signup** page — password is hashed with `bcryptjs` before storing.
2. User logs in — credentials are verified and user data is stored in React's **AuthContext**.
3. Protected routes (e.g. `/course`) check for an authenticated user and redirect to `/signup` if not logged in.

---

## 🌐 Environment Variables

| Variable | Description |
|----------|-------------|
| `PORT` | Port for the Express server (default: `4000`) |
| `MongoDBURI` | MongoDB connection string |

---

## 📸 Pages Overview

- **`/`** — Home page with navbar, hero banner, and free books carousel
- **`/course`** — Protected courses page showing all books in a grid (requires login)
- **`/signup`** — User registration page

---

## 🤝 Contributing

Contributions, issues and feature requests are welcome!

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/your-feature-name`
5. Open a Pull Request

---

## 👨‍💻 Author

**Suraksha** — [@surakshasharma](https://github.com/surakshasharm)

---
