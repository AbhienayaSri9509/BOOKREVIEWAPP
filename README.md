# BOOKREVIEWAPP
  Book Review Platform

A MERN Stack application where users can sign up, log in, add books, and write reviews.
This project demonstrates authentication, CRUD operations, protected routes, and frontend-backend integration.

## 🚀 Features

User Authentication

Sign up with secure password hashing (bcrypt)

Login with JWT token authentication

Protected routes with middleware

Book Management

Add, Edit, Delete books (only by creator)

View all books with pagination (5 per page)

Review System

Add ratings (1–5 stars) and text reviews

Edit/Delete own reviews

Average rating calculation for each book

Frontend (React)

Signup & Login pages

Book List with pagination

Book Details with reviews

Add/Edit Book form

Profile page (bonus)

Database (MongoDB Atlas)

User ↔ Book ↔ Review schema relationships

Efficient queries for ratings and reviews

## 🛠️ Tech Stack

Frontend: React, React Router, Context API, Axios, Tailwind CSS

Backend: Node.js, Express.js

Database: MongoDB Atlas, Mongoose

Authentication: JWT, bcrypt

Deployment: (Optional) Render/Heroku (backend) + Vercel/Netlify (frontend)

## 📂 Project Structure
/backend
  ├── config/
  ├── controllers/
  ├── middleware/
  ├── models/
  ├── routes/
  ├── server.js
/frontend
  ├── src/
      ├── api/
      ├── contexts/
      ├── pages/
      ├── components/
      ├── App.jsx
      ├── index.js

## ⚙️ Setup Instructions
1. Clone the Repository
git clone https://github.com/your-username/book-review-platform.git
cd book-review-platform

2. Backend Setup
cd backend
npm install


## Create a .env file:

PORT=5000
MONGO_URI=your_mongodb_atlas_connection_string
JWT_SECRET=your_jwt_secret
JWT_EXPIRES_IN=7d
SALT_ROUNDS=10


Run server:

npm run dev

3. Frontend Setup
cd frontend
npm install


Create .env:

REACT_APP_API_URL=http://localhost:5000/api


## Run frontend:

npm start

📌 API Endpoints
Auth

POST /api/auth/signup → Register new user

POST /api/auth/login → Login user and return JWT

Books

GET /api/books?page=1 → Get paginated books

POST /api/books → Add book (protected)

GET /api/books/:id → Get book details + reviews

PUT /api/books/:id → Update book (only creator)

DELETE /api/books/:id → Delete book (only creator)

Reviews

POST /api/reviews/:bookId → Add/Update review

GET /api/reviews/:bookId → Get all reviews

PUT /api/reviews/:id → Edit review (only creator)

DELETE /api/reviews/:id → Delete review (only creator)



## ✅ Conclusion

This Book Review Platform integrates authentication, CRUD operations, reviews, and ratings into a functional MERN application.
It demonstrates full-stack development skills and can be expanded into a real-world community platform for book lovers.
