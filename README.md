# 📚 Book Store — Product Management App

## 📌 Project Overview
A full-stack web application to manage a personal book collection. Users can add books with a name, price, and cover image, view all added books, and delete them. Built to practice full-stack development with a React frontend and Node.js/Express backend.

## 🛠 Tech Stack

**Frontend**
* React (Vite)
* React Router
* CSS

**Backend**
* Node.js
* Express.js
* MongoDB (Mongoose)

## 📁 Project Structure
```
book-store/
├── backend/
│   ├── config/
│   │   └── db.js              # MongoDB connection
│   ├── controllers/
│   │   └── product.controller.js   # Add & delete logic
│   ├── models/
│   │   └── product.model.js   # Book schema
│   ├── routes/
│   │   └── product.route.js   # API routes
│   └── server.js              # Express server entry point
│
└── frontend/
    ├── src/
    │   ├── components/
    │   │   ├── Navbar.jsx
    │   │   └── ProductCard.jsx
    │   ├── pages/
    │   │   ├── HomePage.jsx
    │   │   └── CreatePage.jsx
    │   ├── store/
    │   │   └── product.js     # State management
    │   └── App.jsx
    └── index.html
```

## ✨ Features
* Add a book with name, price, and cover image
* View all books on the home page
* Delete a book from the collection
* Responsive card-based UI
* Frontend and backend fully separated

## 🚀 Run Locally

### Prerequisites
* Node.js installed
* MongoDB running locally or a MongoDB Atlas connection string

### Backend Setup
```bash
cd backend
npm install

# Create a .env file in the root with:
# MONGO_URI=your_mongodb_connection_string
# PORT=5000

node server.js
```

### Frontend Setup
```bash
cd frontend
npm install
npm run dev
```

Frontend runs on `http://localhost:5173`  
Backend runs on `http://localhost:5000`

## 📌 API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/api/products` | Get all books |
| POST | `/api/products` | Add a new book |
| DELETE | `/api/products/:id` | Delete a book by ID |

## 💡 What I Learned
* Building a REST API with Node.js and Express
* Connecting MongoDB using Mongoose and defining schemas
* Consuming APIs from a React frontend
* Managing state across components
* Structuring a full-stack project cleanly
