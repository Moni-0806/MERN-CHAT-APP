# Chatify App

<p align="center">
  <img src="./frontend/public/Gemini_Generated_Image_2561wk2561wk2561.png" alt="Chatify app preview" width="900" />
</p>

A full-stack real-time chat application built with the MERN stack, designed to provide secure authentication, instant messaging, and engaging user experiences. The app includes custom JWT-based authentication, live presence indicators, email notifications, image uploads, and a modern responsive UI.

## Highlights

- 🔐 Custom JWT Authentication (no 3rd-party auth)
- ⚡ Real-time Messaging via Socket.io
- 🟢 Online/Offline Presence Indicators
- 🔔 Notification & Typing Sounds (with toggle)
- 📨 Welcome Emails on Signup (Resend)
- 🗂️ Image Uploads (Cloudinary)
- 🧰 REST API with Node.js & Express
- 🧱 MongoDB for Data Persistence
- 🚦 API Rate-Limiting powered by Arcjet
- 🎨 Beautiful UI with React, Tailwind CSS & DaisyUI
- 🧠 Zustand for State Management
- 🧑‍💻 Git & GitHub Workflow (branches, PRs, merges)
- 🚀 Easy Deployment (free-tier friendly with Sevalla)

## Tech Stack

### Frontend
- React
- Vite
- Tailwind CSS
- DaisyUI
- Zustand
- Socket.io Client

### Backend
- Node.js
- Express.js
- MongoDB with Mongoose
- Socket.io
- JWT
- Resend
- Cloudinary
- Arcjet

## Project Structure

```bash
chatify-app/
├── backend/
│   ├── src/
│   ├── .env
│   ├── package.json
│   └── server.js
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
├── README.MD
├── package.json
└── .gitignore
```

## Prerequisites

Before running the app, make sure you have the following installed:

- Node.js v20 or later
- MongoDB instance or MongoDB Atlas connection string
- Cloudinary account
- Resend API key
- Arcjet API key

## Environment Setup

Create a `.env` file inside the `backend` directory with the following variables:

```bash
PORT=3000
MONGO_URI=your_mongo_uri_here

NODE_ENV=development

JWT_SECRET=your_jwt_secret

RESEND_API_KEY=your_resend_api_key
EMAIL_FROM=your_email_from_address
EMAIL_FROM_NAME=your_email_from_name

CLIENT_URL=http://localhost:5173

CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret

ARCJET_KEY=your_arcjet_key
ARCJET_ENV=development
```

## Run the Application

### 1) Start the backend

```bash
cd backend
npm install
npm run dev
```

### 2) Start the frontend

```bash
cd frontend
npm install
npm run dev
```

The frontend should run on a local development URL such as `http://localhost:5173`, while the backend listens on the port defined in your `.env` file.

## Features Overview

- Secure authentication flow with JWT
- Instant message delivery in real time
- User online/offline state updates
- Typing indicator and notification events
- Signup email workflows for onboarding
- Profile picture and media upload support
- Fast and responsive UI for modern browsing experiences

## Notes

This project is built as a practical full-stack application for learning and showcasing modern web development patterns. It combines backend API design, database management, real-time communication, and frontend state management in a single workflow.

## License

This project is available for learning and personal development use.
