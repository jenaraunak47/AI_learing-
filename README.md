# LearnSphere — starter application

A responsive React + Vite MVP for a global learning platform concept. It includes interactive dashboard navigation, room creation and discovery, a room workspace with local demo chat and notes, a rule-based tutor demo, practice quiz, flashcards, focus timer, and progress views.

## Run locally

Requirements: Node.js 18+ and npm.

```bash
npm install
npm run dev
```

Open the local URL printed by Vite (usually `http://localhost:5173`). To make a production build:

```bash
npm run build
npm run preview
```

## Current implementation scope

This starter is a **frontend MVP**. Room data, flashcards, completed activities, and the tutor conversation are saved in the browser's `localStorage`. Demo room chat and notes are local to the current browser. The tutor uses a small rule-based response engine, not a live AI model. Room membership is not shared between devices yet. Sample analytics are clearly labelled as starter estimates.

## What needs a backend for a real global launch

- Authentication and authorization.
- Database-backed profiles, rooms, room membership, notes, resources, quizzes, and progress.
- Real-time shared chat and synchronized notes (e.g. Socket.IO + Node/Express + MongoDB).
- Secure server-side LLM API integration for the AI tutor.
- Moderation, rate limiting, account deletion, and privacy controls.
- Automated tests and deployment configuration.

Do not place private API keys in frontend code. Use server-side environment variables for any AI provider.
