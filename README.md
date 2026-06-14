# Peblo Neural Workspace

AI-powered note-taking workspace built using React, Node.js, Express, MongoDB Atlas, and OpenAI/Groq.

Repository: https://github.com/Aadiii07/Peblo-Neural-Workspace

## Features

- JWT Authentication
- AI Summaries
- AI Action Items
- AI Title Suggestions
- Voice Notes
- Public Sharing
- Analytics Dashboard
- Responsive Design

## Tech Stack

### Frontend
- React
- Vite
- Tailwind CSS
- Framer Motion
- Zustand

### Backend
- Node.js
- Express
- JWT

### Database
- MongoDB Atlas
- Mongoose

### AI
- OpenAI / Groq

## Getting Started

1. Install dependencies for both apps:
   - Backend: cd server && npm install
   - Frontend: cd client && npm install
2. Create a local environment file in the server folder using the template in server/.env.example.
3. Start the backend and frontend in separate terminals.

## Environment Variables

Create server/.env from the example below:

PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
OPENAI_API_KEY=your_api_key
CLIENT_URL=http://localhost:5173
USE_IN_MEMORY_DB=0

## Project Structure

- server/ — Express API, auth, notes, AI integration
- client/ — React/Vite frontend
- docs/ — screenshots and preview assets

## Preview

Screenshots will be added in the docs folder for the workspace, dashboard, AI summary, and login views.

Built by Aditya for the Peblo Full Stack Developer Challenge.
