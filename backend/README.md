# Backend — Brev.ly

Brev.ly backend is a Node.js/TypeScript API for shortening URLs, managing links, and exporting reports. It is part of the practical challenge for the Technical and Strategic Foundations module (Pós Tech Developer 360, FTR).

## Technologies Used

- Node.js
- TypeScript
- Fastify (HTTP API)
- Drizzle ORM (migrations, DB access)
- PostgreSQL
- Cloudflare R2 (file storage)
- Vitest (testing)
- Docker & Docker Compose
- pnpm (package manager)

## Setup & Usage

1. Install dependencies:
   ```bash
   pnpm install
   ```
2. Configure the `.env` file with database, Cloudflare, and other required environment variables.
3. Start the backend (standalone):
   ```bash
   pnpm dev
   ```
   Or with Docker Compose (from project root):
   ```bash
   docker compose up --build
   ```
4. Run database migrations:
   ```bash
   pnpm drizzle:push
   ```
5. The API will be available at `http://localhost:3333` (default).

## Tests

To run backend tests:
```bash
pnpm test
```

## Cloudflare R2 Integration

To enable CSV report export to Cloudflare R2, configure the related environment variables in `.env`.
If not configured, CSV report download will be unavailable.
