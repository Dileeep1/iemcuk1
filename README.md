# IEMCUK Global Platform

Production-ready multi-country education and migration consultancy platform for IEMCUK and regional entities.

## Apps

- `apps/web`: Next.js App Router marketing site and lead capture frontend
- `apps/api`: Node.js + Express + TypeScript API for leads, admin-ready workflow, and integrations

## Stack

- Next.js 15 + React 19 + TypeScript + Tailwind CSS
- Express + TypeScript + PostgreSQL
- AWS-ready deployment architecture

## Quick start

1. Install dependencies:

```bash
npm install
```

2. Copy environment files:

```bash
copy apps\\web\\.env.example apps\\web\\.env.local
copy apps\\api\\.env.example apps\\api\\.env
```

3. Run the frontend:

```bash
npm run dev:web
```

4. Run the backend:

```bash
npm run dev:api
```

## Architecture

- Frontend calls `NEXT_PUBLIC_API_BASE_URL`
- Backend persists leads into PostgreSQL
- SMTP notifications fire on lead creation
- WhatsApp CTA deep-link is generated from the submitted lead
- Country content is config-driven for global expansion

See [docs/architecture.md](/C:/Users/dileep/Downloads/AE%20Vibe/docs/architecture.md) for deployment and scaling notes.
