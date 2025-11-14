# Real-Time Chat Application — Week 7: Deployment & Real-Time Communication.

This is a real-time chat application built using Node.js, Express, Socket.io, and a React + Vite frontend.
It supports live messaging, private chat, typing indicators, online-user tracking, and room-based communication.

---
## Live Demo

- Frontend (Vercel): https://real-time-communication-with-socket-rose.vercel.app/

- Backend (Render): https://week5-chat-backend-61ui.onrender.com


## Features
# Real-Time Communication
- Live chat (public)
- Private messaging (1-to-1)
- Typing indicator
- Online users list
- System notifications (join/leave)
- Chat rooms

# Backend (Node.js + Socket.io)
- Express server
- In-memory users + messages
- CORS configured for frontend deployment
- Real-time socket events

# Frontend (React + Vite)

- Clean UI for chat
- Socket.io client integration
- Displays online users
- Supports rooms + private chat
---

## **Screenshots**

![Login](./screenshots/login.png)
![Home Page](./screenshots/HOMEPAGE.png)
![Chat](./screenshots/chat.png)
![Chat Rooms](./screenshots/chatroom.png)
![Chat Rooms](./screenshots/chatroom2.png)

---
project-root/
│── server/
│     ├── server.js
│     ├── package.json
│     ├── .env.example
│
│── client/
│     ├── src/
│     ├── package.json
│     ├── vite.config.js
│     ├── .env.example
│
│── README.md
---
# How to Run Locally
1️⃣ Clone the repository
```bash
git clone https://github.com/PLP-MERN-Stack-Development/deployment-and-devops-essentials-naomitesfe
cd deployment-and-devops-essentials-naomitesfe
```

2️⃣ Run the Backend (Node.js + Socket.io)
```bash
cd backend
npm install
npm run dev
```
Backend runs on:
👉 http://localhost:5000

3️⃣ Run the Frontend (React + Vite)
```bash
cd frontend
npm install
npm run dev
```
Frontend runs on:
👉 http://localhost:5173

# 🔧 Environment Variables
Backend .env
```bash
CLIENT_URL=http://localhost:5173
PORT=5000
```
```bash
Frontend .env
VITE_SOCKET_URL=http://localhost:5000
```
When deployed, replace with your Render + Vercel URLs.

## Usage
- Enter your username and log in.
- Select or create a chat room.
- Send messages in the room or privately to other users.
- Toggle notifications to view unread messages.
- Click Sign Out to end your session.

## Deployment
# Backend: Render
- Created a new Web Service
- Set the build command: npm install
- Start command: node server.js
- Added environment variables under “Environment”
- Added CORS whitelist to allow Vercel frontend

# Frontend: Vercel
- Connected GitHub repo
- Vercel automatically built Vite project
- Added environment variable: VITE_SOCKET_URL
- Deployment runs automatically on every push

# CI/CD 
- GitHub → Vercel auto deployment
- GitHub → Render auto redeploy 

# Contributing
- Fork the repo.
- Create a feature branch: git checkout -b feature/my-feature
- Commit changes: git commit -m "Add my feature"
- Push branch: git push origin feature/my-feature
- Open a Pull Request



