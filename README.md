# MFC-Tech

MFC-Tech is a full-stack web application with a Vite frontend and a Node.js backend.

## Repository layout

- `frontend/` — browser client
- `backend/` — API server

## Run locally

Install dependencies in each application directory:

```bash
cd backend
npm install
npm start
```

In a second terminal:

```bash
cd frontend
npm install
npm run dev
```

The frontend's development server and API base URL may need to be aligned with the backend configuration for local requests.

## Architecture

```mermaid
flowchart LR
    User[Browser] --> Frontend[React/Vite frontend]
    Frontend --> API[Node.js/Express backend]
    API --> Services[API routes and business logic]
    Services --> Data[(Configured data store)]
```
