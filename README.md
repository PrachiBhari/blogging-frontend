📝 Blogging Website (MERN Stack)

A full-stack blogging platform built with the MERN stack — allowing users to create, read, update, and delete blog posts, manage their profiles, and explore posts from others.

🌐 Live Demo: [https://blogging-frontend.netlify.app/]
🖥 Frontend Repo: https://github.com/PrachiBhari/blogging-frontend

⚙️ Backend Repo: https://github.com/PrachiBhari/blogging-backend

📑 Table of Contents

✨ Features

🧱 Tech Stack

🚀 Getting Started

Prerequisites

Installation (Frontend & Backend)

🗂️ Project Structure

🧭 API Overview

✅ Usage Walk-through

🛠️ Future Enhancements

✨ Features
👥 User Features

User authentication (signup/login/logout)

Create, edit, and delete blog posts

Upload cover images (if implemented)

View list of all blogs with pagination/search

Read other users’ blogs with full content view

Like, comment, and share functionality

Profile management with author details and bio

🧑‍💻 Admin Features (optional if added)

View all registered users

Manage or delete inappropriate content

🧱 Tech Stack

Frontend:

React.js

React Router DOM

Axios (for API calls)

TailwindCSS / CSS Modules / styled-components (mention what you used)

Backend:

Node.js

Express.js

MongoDB with Mongoose ORM

JWT Authentication

bcrypt for password hashing

Multer or Cloudinary for image uploads (if used)

Other Tools:

Git & GitHub for version control

Postman for API testing

Netlify (Frontend Hosting)

Render / Railway / Vercel (Backend Hosting)

🚀 Getting Started
Prerequisites

Make sure you have installed:

Node.js (v16+ recommended)

npm 

MongoDB (local or Atlas connection string)

⚙️ Installation
1️⃣ Clone both repositories
# Frontend
git clone https://github.com/PrachiBhari/blogging-frontend.git
cd blogging-frontend
npm install
npm start

# Backend (open a new terminal)
git clone https://github.com/PrachiBhari/blogging-backend.git
cd blogging-backend
npm install
npm run dev   # or node index.js

2️⃣ Set up environment variables

In your backend folder, create a .env file:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret

3️⃣ Connect frontend & backend

In your frontend src/config.js or API file, update the base URL:

export const API_URL = "http://localhost:5000/api";

🗂️ Project Structure
Frontend
blogging-frontend/
├── src/
│   ├── components/        # Navbar, Footer, PostCard, etc.
│   ├── pages/             # Home, Login, Register, PostDetail, Dashboard
│   ├── context/           # AuthContext or State management
│   ├── services/          # Axios API calls
│   ├── App.js
│   └── index.js
└── package.json

Backend
blogging-backend/
├── config/
│   └── db.js              # MongoDB connection
├── controllers/
│   ├── authController.js
│   ├── postController.js
│   └── userController.js
├── models/
│   ├── User.js
│   └── Post.js
├── routes/
│   ├── authRoutes.js
│   ├── postRoutes.js
│   └── userRoutes.js
├── middleware/
│   └── authMiddleware.js
├── server.js
└── package.json

🧭 API Overview
Auth Routes
Method	Endpoint	Description
POST	/api/auth/register	Register a new user
POST	/api/auth/login	Login user
GET	/api/auth/me	Get logged-in user details
Blog Routes
Method	Endpoint	Description
GET	/api/posts	Get all blog posts
GET	/api/posts/:id	Get a single post
POST	/api/posts	Create a new post
PUT	/api/posts/:id	Update a post
DELETE	/api/posts/:id	Delete a post
✅ Usage Walk-through

Sign Up / Log In to access your dashboard.

Create a Blog: Add title, description, tags, and optional image.

View & Interact: Explore blogs from other users, leave comments or likes.

Edit/Delete: Manage your own posts easily from dashboard.

Logout securely to end the session.

🛠️ Future Enhancements

🖼️ Rich-text editor (Quill.js / TinyMCE)

🗂️ Categories & tags for better filtering

💬 Comment system with replies

🧵 Follow/unfollow authors

📊 Analytics dashboard for writers

🌙 Dark/Light mode toggle

📱 Progressive Web App (PWA) support




Commit and push your changes

Open a Pull Request
