# Peblo Neural Workspace

Peblo is an AI-powered note workspace for capturing ideas, generating summaries, creating action items, and sharing notes with collaborators. The repository now includes a Vercel-compatible API entry, a React/Vite frontend, and a Node/Express backend that work together to power the experience.

## What is in this repo

- api/ — Vercel serverless wrapper that exposes the same Express app used in local development
- client/ — React + Vite front end with Tailwind, Framer Motion, Zustand, and the note/voice/AI UI
- server/ — Express API, authentication, note management, AI integration, and MongoDB connection logic
- docs/ — portfolio screenshots and visual previews used in this project

## Quick start

1. Install dependencies for both apps:
   - npm install --prefix server
   - npm install --prefix client
2. Start the backend:
   - npm run dev:server
3. Start the frontend in a second terminal:
   - npm run dev:client
4. If you want a production build for the frontend:
   - npm run build

## Project structure

- api/index.js — Vercel entry point that loads the Express app
- server/app.js — main server setup and route wiring
- server/controllers/ — auth, notes, AI, and note-sharing logic
- server/models/ — Mongoose models for users and notes
- server/routes/ — API endpoints for auth, notes, and sharing
- client/src/ — React pages, components, services, hooks, and store logic

## Tech stack

### Frontend
- React
- Vite
- Tailwind CSS
- Framer Motion
- Zustand
- Axios

### Backend
- Node.js
- Express
- JWT
- bcryptjs

### Data and AI
- MongoDB Atlas / Mongoose
- OpenAI / Groq integration

## Features

- JWT authentication
- Auto-save note workspace
- AI summaries and action items
- AI tags and title suggestions
- Voice note interaction
- Public sharing links
- Analytics-style dashboard
- Responsive interface

## Environment setup

Create a local environment file in the server folder before running the backend.

Example variables:

PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
OPENAI_API_KEY=your_api_key
CLIENT_URL=http://localhost:5173
USE_IN_MEMORY_DB=0

## Preview gallery

The screenshot files in the docs folder have been renamed and are now organized as follows:

- docs/ai-assistant-panel.png
- docs/action-items-tags.png
- docs/analytics-dashboard.png
- docs/public-share-page.png
- docs/voice-note-modal.png
- docs/workspace-editor.png

Use the images in this folder for the portfolio, documentation, and visual walkthroughs.

Built for the Peblo Full Stack Developer Challenge.
