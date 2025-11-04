# Music Website (Full-stack)

This zip contains a simple full-stack music website example:
- backend: Node.js + Express (folder: backend)
- frontend: React + Vite (folder: frontend)

Quick steps:
1. Import database schema (see db-schema.sql) into MySQL (create DB `music_db`).
2. Backend: `cd backend` -> `npm install` -> copy `.env.example` to `.env` and fill values -> `npm run dev`
3. Frontend: `cd frontend` -> `npm install` -> `npm run dev`

Sample curl to upload a track (backend must be running):
curl -F "audio=@/path/to/file.mp3" -F "title=Test Track" -F "artist_id=1" http://localhost:4000/api/tracks
