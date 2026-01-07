
# Frontend — Brev.ly

Brev.ly frontend is a React + Vite application for interacting with the Brev.ly URL shortener API. It is part of the practical challenge for the Technical and Strategic Foundations module (Pós Tech Developer 360, FTR).

## Technologies Used

- React
- Vite
- TypeScript
- Tailwind CSS (styling)
- pnpm (package manager)

## Setup & Usage

1. Install dependencies:
	```bash
	pnpm install
	```
2. Configure the environment variables if needed (see `.env.example` or project documentation).
3. Start the frontend:
	```bash
	pnpm dev
	```
4. The app will be available at `http://localhost:5173` (default).

## Project Structure

- `src/` — React components, pages, and HTTP utilities
- `public/` — Static assets

## Features

- Create, list, and delete shortened URLs
- Redirect to original URLs
- Download CSV reports (if backend and Cloudflare R2 are configured)


