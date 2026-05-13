# Azure Translator (Simran)

The **Azure-translator-Simran-** project ("The Linguistic Atelier") is a small web app that translates text into multiple languages using selectable translation engines (e.g., Google Translate or Azure Translator API) and provides history + user-scoped saved data.

## Features

- Multi-language translation workspace (simultaneous outputs)
- Supports multiple translation engines (configurable via UI)
- User-specific persisted data stored under `data/users/<email>/`
- History, settings, and palette endpoints served by the Node/Express backend

## Tech Stack

- Frontend: HTML/CSS/Vanilla JS, Tailwind CDN
- Backend: Node.js + Express
- Data storage: JSON files under `data/users/`

## Run locally

1. Install dependencies:
   ```bash
   npm install
   ```
2. Start the server:
   ```bash
   npm start
   ```
3. Open:
   - http://localhost:3000

## Scripts

- `npm start` - runs `node server.js`
- `npm run dev` - runs `node --watch server.js`

## Project Structure

- `server.js` - Express server + file-based persistence
- `*.html` - Frontend pages
- `*.js` - Frontend scripts
- `data/users/` - Per-user JSON data

## Note

If you plan to deploy publicly, replace file-based auth/storage with a proper authentication/database solution.

