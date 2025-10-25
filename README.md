# ERP Linkanawi

Starter monorepo: Backend (Node.js + Prisma/Postgres) + Frontend (React + Vite + Tailwind) + Docker

## Levantar local (Docker)
1. Copiar `.env.example` a `.env` y editar si necesario.
2. `docker-compose up --build`
3. Ejecutar migraciones y seed (si no quieres usar Docker para esto, instala node y prisma localmente):
   - `cd backend`
   - `npx prisma migrate dev --name init`
   - `node prisma/seed.js`
4. Frontend en `http://localhost:5173` y backend en `http://localhost:4000`
