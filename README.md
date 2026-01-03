## About the Project

**Brev.ly** is a URL shortener that transforms long links into short, easy-to-share URLs.

This project was developed as a **practical challenge** for the **Technical and Strategic Foundations** module, part of the **Pós Tech Developer 360** postgraduate program at **Faculdade de Tecnologia Rocketseat (FTR)**.

## Technologies Used

- **Node.js** — backend
- **TypeScript**
- **Fastify** — HTTP API
- **Drizzle ORM** — migrations and database access
- **PostgreSQL** — database
- **React + Vite** — frontend
- **Tailwind CSS** — styling
- **Cloudflare R2** — file storage
- **Vitest** — testing
- **Docker & Docker Compose** — containerization
- **pnpm** — package manager

## Deployment / Execution Flow

1. Install dependencies for both **backend** and **frontend**.
2. Configure the `.env` file with database, Cloudflare, and other required environment variables.
3. Start the containers using **Docker Compose**.
4. Run the migrations to create the database tables.
5. Access the API at `http://localhost:3333` and the frontend at `http://localhost:5173` (or the configured port).

## Tests

To run backend tests, navigate to the `backend` directory and execute:

```bash
pnpm test
```

## Cloudflare R2 Integration

The project supports exporting CSV reports to **Cloudflare R2**.  
To enable this feature, configure the related environment variables in the `.env` file.

> If Cloudflare R2 is not configured, downloading the CSV report will not be available.

## Notes

- Migrations must be applied manually after starting the containers using:

  ```bash
  pnpm db:migrate
  ```
- The project uses Drizzle ORM for migration versioning and execution.
