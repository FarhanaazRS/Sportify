# 🏆 Sportify – Corporate Sports Tournament Manager

**Sportify** is a robust full-stack web platform tailored for managing corporate sports tournaments. It streamlines event creation, team registrations, live scoring, and leaderboard tracking – all from a user-friendly interface.

---

## 🚀 Key Features

### 🔐 Authentication & Authorization
- Secure authentication using **JWT**
- **Role-based access**: Admin, Judge, Participant
- Centralized auth management via `AuthContext.js`

### 🏟️ Event Management
- Admins can create & categorize events: Indoor, Outdoor, Fun
- Define participant limits and capacity
- Add event descriptions and multimedia

### 🧑‍🤝‍🧑 Team Registration
- Seamless registration experience
- Real-time team status tracking
- Team dashboard with updates

### 🧮 Live Scoring System
- Judges input scores in real-time
- **Socket.io** enables instant updates
- Dynamic leaderboard refresh

### 📊 Leaderboard & Visual Insights
- Per-event leaderboards
- Live data visualization using **Chart.js**

### 🤖 AI-Powered Event Assistant
- Integrated with **Gemini AI**
- Generates event ideas and descriptions intelligently

---

## 🧱 Tech Stack

### ⚙️ Backend
- Node.js with Express.js
- MongoDB (NoSQL)
- JWT for authentication
- **Socket.io** for real-time events
- PDFKit for downloadable content

### 💻 Frontend
- React.js
- Tailwind CSS for UI
- Framer Motion for animations
- Socket.io Client
- Chart.js for data visualization
- Gemini API for AI suggestions

---

## 🛠 Setup & Installation

### 📦 Requirements
- Node.js (v14 or newer)
- MongoDB
- npm or yarn package manager


---

## 🌐 Environment Variables Setup

Create `.env` files in both the `frontend/` and `backend/` directories.

### frontend/.env
```env
REACT_APP_API_URL=http://localhost:5000
REACT_APP_SOCKET_URL=http://localhost:5000
REACT_APP_GEMINI_API_KEY=your_gemini_api_key
```

### backend/.env
```env
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
PORT=5000
```

---

## ▶️ Running the App

### Start the Backend Server
```bash
cd backend
npm start
```

### Start the Frontend Server
```bash
cd frontend
npm start
```

---

## 📚 API Endpoints

### 🔑 Authentication
- `POST /api/auth/register` – User registration  
- `POST /api/auth/login` – User login

### 🏆 Event Management
- `GET /api/events` – Fetch all events  
- `POST /api/events` – Create event (Admin only)  
- `GET /api/events/:id` – Get specific event  
- `PUT /api/events/:id` – Update event (Admin)  
- `DELETE /api/events/:id` – Delete event (Admin)

### 👥 Team Management
- `POST /api/teams` – Register a team  
- `GET /api/teams` – Get all registered teams

### 🧮 Scoring System
- `POST /api/scores` – Submit score (Judge only)  
- `GET /api/scores/:eventId` – Get event scores  
- `GET /api/scores/leaderboard/:eventId` – Fetch leaderboard

---

> 🎉 Ready to host your own sports tournament? Fork this project and get started!



