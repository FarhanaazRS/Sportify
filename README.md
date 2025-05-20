# SportsFiesta 🏆

**SportsFiesta** is a full-stack web application designed for managing corporate sports tournaments and events. It provides powerful tools for organizing events, team registrations, real-time scoring, and dynamic l

---

## 🚀 Features

### 🔐 Authentication & Authorization
- Secure **JWT-based** authentication
- **Role-based access control** (Admin, Judge, Participant)
- Context-based auth handling in frontend (`AuthContext.js`)

### 🏁 Event Management
- Admin can create and manage events
- Events categorized as Indoor, Outdoor, or Fun
- Registration limits and event capacities
- Event details with descriptions and media

### 🧑‍🤝‍🧑 Team Registration
- Smooth registration flow
- Live status updates
- Dashboard for team tracking

### 🧮 Real-time Scoring
- Judges can input scores
- Live updates via **Socket.io**
- Automatic leaderboard updates

### 📊 Leaderboards & Visualization
- Event-specific leaderboards
- **Chart.js** for real-time data visualization

### 🤖 AI-Powered Event Suggestions
- Integrated with **Gemini AI**
- Suggests event ideas & auto-generates event details

---

## 🧱 Tech Stack

### ⚙️ Backend
- Node.js + Express.js
- MongoDB
- JWT Auth
- Socket.io
- PDFKit

### 💻 Frontend
- React.js
- Tailwind CSS
- Framer Motion
- Socket.io Client
- Chart.js
- Google Generative AI API

---

---

## 🛠 Getting Started

### 📦 Prerequisites
- Node.js (v14+)
- MongoDB
- npm or yarn

### 📥 Installation

#### 1. Clone the Repository
```bash
git clone https://github.com/RaafidAfraazG/SportsFiesta.git
```
### 2. Install Frontend Dependencies
```
cd SportsFiesta/frontend
npm install
```

### 3. Install Backend Dependencies
```
cd ../backend
npm install
```

## 🌍 Environment Variables

Create .env files in both frontend/ and backend/ folders.
---
frontend/.env
```
REACT_APP_API_URL=http://localhost:5000
REACT_APP_SOCKET_URL=http://localhost:5000
REACT_APP_GEMINI_API_KEY=your_gemini_api_key

```
backend/.env

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
PORT=5000

```

## ▶️ Running the Project

Start Backend Server
```
cd backend
npm start

```

Start Frontend Server
```
cd frontend
npm start

```

## 📚 API Documentation

### 🔑 Authentication
- `POST /api/auth/register` — Register a user  
- `POST /api/auth/login` — Login

### 🏆 Events
- `GET /api/events` — Get all events  
- `POST /api/events` — Create new event (Admin)  
- `GET /api/events/:id` — Get event by ID  
- `PUT /api/events/:id` — Update event (Admin)  
- `DELETE /api/events/:id` — Delete event (Admin)

### 👥 Teams
- `POST /api/teams` — Register a team  
- `GET /api/teams` — View registered teams

### 🧮 Scores
- `POST /api/scores` — Submit score (Judge)  
- `GET /api/scores/:eventId` — Get scores for event  
- `GET /api/scores/leaderboard/:eventId` — Get leaderboard

---

## 📸 Screenshots 


<img width="958" alt="image" src="https://github.com/user-attachments/assets/bd0f96a0-e8fd-490b-9f17-13868ab749fc" />


<img width="960" alt="image" src="https://github.com/user-attachments/assets/483e97a2-2d72-47c9-bc99-27f216492073" />


<img width="960" alt="image" src="https://github.com/user-attachments/assets/ea12eb4a-c3f3-44da-8b14-db410fde8919" />


<img width="959" alt="image" src="https://github.com/user-attachments/assets/c8f191a6-809e-426e-8a3c-422f816377fb" />


