# Product App — Full Stack

## Stack
- **Frontend**: React + Vite + TypeScript + Tailwind CSS
- **Backend**: Node.js + Express + TypeScript + MongoDB

## Setup

### Prerequisites
- Node.js >= 18
- MongoDB running locally (or MongoDB Atlas URI)

### Backend
cd backend

cp .env.example .env   # Fill MongoDB URI and JWT secret

npm install

npm run seed           # Seed sample data

npm run dev            # Run at http://localhost:5000

### Frontend
cd frontend

npm install

npm run dev            # Run at http://localhost:5173

## API Endpoints
| Method | Endpoint          | Auth Required |
|--------|-------------------|---------------|
| GET    | /api/products     | No            |
| GET    | /api/products/:id | No            |
| POST   | /api/products     | Yes (JWT)     |
| PUT    | /api/products/:id | Yes (JWT)     |
| DELETE | /api/products/:id | Yes (JWT)     |
| POST   | /api/auth/register| No            |
| POST   | /api/auth/login   | No            |