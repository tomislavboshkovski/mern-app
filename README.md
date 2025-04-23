# 🏋️ Workout Tracker MERN App

This is a full-stack MERN (MongoDB, Express, React, Node.js) application that allows users to register, log in, and track their workouts. Users can submit workouts via a form and delete them at any time.

## 🚀 Features

- JWT-based authentication (signup and login)  
- Create, read, and delete workouts  
- MongoDB Atlas for database storage  
- Environment variables managed with `dotenv`  
- RESTful API backend with Express.js  
- Frontend built with React and deployed with Netlify  
- CORS enabled for development and deployment  

## 🛠 Tech Stack

- **Frontend:** React, Vite  
- **Backend:** Node.js, Express  
- **Database:** MongoDB Atlas  
- **Authentication:** JSON Web Tokens (JWT)  
- **Environment Variables:** dotenv  
- **CORS:** Configured for frontend-backend communication  

## 📂 Project Structure

```
mern_app/
├── client/          # React frontend (Vite)
└── server/          # Node.js backend (Express)
    └── .env         # Environment variables
```

## 🔐 .env Configuration (Server)

⚠️ This project includes a .env file in the repository for demonstration purposes only. Normally, sensitive environment variables like database connection strings or API keys should never be committed to version control. However, to make it easier for recruiters and reviewers to run the app locally without additional setup, a test database connection string is included. Please use this responsibly and understand that in a real-world or production environment, secrets should be stored securely and excluded from the repo via .gitignore.


## 💡 Getting Started (Local Development)

1. Clone the repo

```
git clone https://github.com/tomislavboshkovski/mern-app
cd MERN_APP
```

2. Start the Backend

```
cd server
npm install
npm run dev
```

3. Start the Frontend

```
cd client
npm install
npm run dev
```

Make sure both the client and server are running.  
The frontend will run on: `http://localhost:5173`  
The backend will run on: `http://localhost:4000`


## 🔄 API Endpoints (Protected with JWT)

| Method | Endpoint            | Description                |
|--------|---------------------|----------------------------|
| POST   | `/api/user/signup`  | Register a new user        |
| POST   | `/api/user/login`   | Login with credentials     |
| GET    | `/api/workouts`     | Get all workouts (auth)    |
| POST   | `/api/workouts`     | Create a new workout (auth)|
| DELETE | `/api/workouts/:id` | Delete a workout (auth)    |


Created by **Tomislav** — this project was built for learning and portfolio purposes.

