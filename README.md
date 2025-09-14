# Rune Quest — Full Project

This archive contains a full-stack demo of the Rune Quest prototype with:
- A* pathfinding and smooth movement
- Pixel-art sprites (simple placeholders included)
- Functional combat messages over WebSocket
- Express + WebSocket + SQLite backend with save/load
- Stripe checkout endpoint and webhook handler (placeholders)
- Dockerfiles and docker-compose for easy deployment

## Quick start (local)
1. Ensure Docker is installed.
2. From repo root: `docker-compose up --build`.
3. Open http://localhost:5173 to access the client. Server API is at http://localhost:8080.

## Stripe
Set `STRIPE_SECRET_KEY` and `STRIPE_WEBHOOK_SECRET` in the server environment for payments to work. Create Stripe products/prices and use their price IDs.

## Notes
- The webhook code requires the raw request body and signature header; configure Stripe accordingly.
- The included sprites are simple programmatic placeholders. Replace `client/public/spritesheet.png` with your art for better visuals.
