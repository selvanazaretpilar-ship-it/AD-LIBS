# AD-LIBS Admin CPanel — Real-Time First Starter

This repo is optimized for real-time fleet telemetry and live maps.

Quick start (Docker):
1. Copy `.env.example` to `.env` and fill secrets.
2. `docker-compose up --build`
3. Frontend: http://localhost:3000
4. Backend API: http://localhost:4000/api
5. Socket.IO: ws://localhost:4000

Services included:
- backend (Express + Socket.IO + Mongoose)
- worker (BullMQ consumer for telemetry)
- mongo
- redis
- frontend (Vite + React)

Telemetry emulator: `node tools/telemetry-emulator.js --count 50 --rate 2`
