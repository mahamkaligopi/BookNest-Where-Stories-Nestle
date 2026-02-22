# BookNest - MERN Stack Project

BookNest is a MERN-based book marketplace application with 3 roles:
- User
- Seller
- Admin

It includes authentication, product/book listing, cart, wishlist, and order management.

## Project Structure

```text
Backend/   -> Express + MongoDB API
frontend/  -> React + Vite client
```

## Tech Stack

- **Frontend:** React, Vite, Axios, React Router
- **Backend:** Node.js, Express, MongoDB, Mongoose
- **Other:** Multer (image upload), CORS, dotenv

## Prerequisites

- Node.js (v18+ recommended)
- npm
- MongoDB (local or Atlas)

## Environment Variables

Create a file: `Backend/.env`

```env
PORT=4000
MONGO_URI=mongodb://127.0.0.1:27017/BookStore
FRONTEND_URL=http://localhost:5173
```

> `MONGO_URI` can be your MongoDB Atlas URI if you are not using local MongoDB.

## Installation

From project root, install dependencies for both apps:

```bash
npm install
cd Backend && npm install
cd ../frontend && npm install
```

## Run the Project

### 1) Start Backend

```bash
cd Backend
npm run dev
```

Backend runs on: `http://localhost:4000`

### 2) Start Frontend

Open a second terminal:

```bash
cd frontend
npm run dev
```

Frontend usually runs on: `http://localhost:5173`

## Git Setup and Push

Run from project root:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin <your-repo-url>
git push -u origin main
```

Example remote URL:

```bash
git remote add origin https://github.com/<username>/<repo-name>.git
```

## Notes

- Uploaded images are stored in `Backend/uploads/`.
- Keep `.env` private (already ignored in `.gitignore`).
