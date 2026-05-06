# 🛠️ Debug Battle — 6 May Edition

A full-stack **Product Management** web application built as part of a timed debug battle challenge. The goal: receive a broken codebase, find the bugs, fix them, and ship a working app.

---

## 📁 Project Structure

```
6-May-Battle/
├── backend/          # Node.js + Express REST API
├── frontend/         # React + Vite client
└── .sixth/           # Challenge skill files
```

---

## 🚀 Tech Stack

| Layer     | Technology                              |
|-----------|-----------------------------------------|
| Frontend  | React 19, Vite, Tailwind CSS v4, Radix UI |
| Backend   | Node.js, Express 4, Mongoose 8          |
| Database  | MongoDB                                 |
| HTTP      | Axios                                   |

---

## ⚙️ Getting Started

### Prerequisites
- Node.js ≥ 18
- MongoDB (local or Atlas)

---

### 1. Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file (copy from `.env.example`):

```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/product-management
NODE_ENV=development
```

Start the server:

```bash
# Development (with auto-reload)
npm run dev

# Production
npm start
```

Seed the database with sample data:

```bash
npm run seed
```

The API will be available at `http://localhost:5000`.

---

### 2. Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

The client will be available at `http://localhost:5173`.

---

## 🔌 API Endpoints

Base URL: `/api/products`

| Method   | Endpoint          | Description              |
|----------|-------------------|--------------------------|
| `GET`    | `/api/products`   | Get all products         |
| `POST`   | `/api/products`   | Create a new product     |
| `GET`    | `/api/products/:id` | Get a product by ID    |
| `PUT`    | `/api/products/:id` | Update a product by ID |
| `DELETE` | `/api/products/:id` | Delete a product by ID |

A health-check is also available at `GET /`.

---

## 🧩 Frontend Components

| Component       | Description                              |
|-----------------|------------------------------------------|
| `Dashboard`     | Main view — lists products with filters  |
| `ProductCard`   | Displays individual product details      |
| `ProductForm`   | Form for creating / editing products     |
| `Pagination`    | Handles page navigation                  |

---

## 🐛 Challenge Context

This repo is part of a **Debug Battle** — a competitive challenge where participants receive a intentionally broken codebase and must identify and fix all bugs within a time limit.
