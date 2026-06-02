# Repository Guidelines

## Project Structure & Module Organization
This repository defines the Lohbeng hackathon prototype: a Next.js frontend and a FastAPI backend. Follow the structure in `SPEC.md`: `frontend/src` for app code, `frontend/public` for static assets, and `backend/app` for routers, services, models, and utilities. Keep `backend/videos`, `backend/outputs`, and `backend/weights` for local AI pipeline assets. Root docs such as `SPEC.md`, `CONTEXT.md`, and `TASKS.md` are the current source of truth for architecture, scope, and priorities.

## Build, Test, and Development Commands
Frontend:
- `cd frontend && npm install` installs dependencies.
- `cd frontend && npm run dev` starts the Next.js 16 dev server.
- `cd frontend && npm run build` creates a production build.
- `cd frontend && npm run lint` checks ESLint issues.

Backend:
- `cd backend && python -m venv .venv` creates a local virtual environment.
- `cd backend && pip install -r requirements.txt` installs FastAPI and AI dependencies.
- `cd backend && uvicorn app.main:app --reload` runs the API locally.

## Coding Style & Naming Conventions
Use TypeScript on the frontend and Python 3.11+ on the backend. Prefer modular, feature-based organization and stateless REST handlers. Keep components small, readable, and reusable. Use `PascalCase` for React components, `camelCase` for functions and hooks, and lowercase descriptive filenames for API/router modules. Match the project's futuristic, Stitch-aligned UI direction; do not introduce drastic redesigns without approval.

## Testing Guidelines
Before opening a PR, ensure the frontend builds cleanly, has no TypeScript errors, and passes linting. Add frontend tests as `*.test.ts` or `*.test.tsx` when logic is introduced. Add backend tests as `test_*.py`, focusing on endpoint behavior and analytics calculations. At minimum, smoke-test `/api/metrics`, `/api/detections`, `/api/pollution-risk`, and `/api/cctv`.

## Commit & Pull Request Guidelines
Use short, imperative commit messages, preferably Conventional Commit style such as `feat: add PM2.5 trend card` or `fix: correct risk badge colors`. PRs should include a concise summary, affected area (`frontend`, `backend`, or `docs`), linked task from `TASKS.md`, and screenshots or GIFs for UI changes.

## Security & Configuration Tips
Keep APIs stateless and use polling every 3000ms; do not introduce WebSockets or `socket.io`. Do not add Prisma, PostgreSQL, Redis, Docker, Kubernetes, Redux, or microservices. Use mock or simulated datasets unless a task explicitly expands the data strategy. Preserve the lightweight hackathon architecture and presentation-first priorities documented in `CONTEXT.md`.
