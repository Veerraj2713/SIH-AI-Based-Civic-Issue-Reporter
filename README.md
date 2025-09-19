# Civic Issue Reporter (MERN)

Quickstart:

1) Backend

```
cd backend
copy .env.example .env  (create if missing)
npm install
npm run dev
```

2) Frontend

```
cd frontend
echo VITE_API_BASE=http://localhost:4000 > .env.local
npm install
npm run dev
```

Features:

- Client: upload image, AI checks if civic issue, auto short complaint, categorize, submit
- Admin: view all complaints, update status (in progress / resolved / rejected)
- Image AI-gen heuristic filter; rejects AI images from submission
- Stored in MongoDB; images saved to `backend/uploads`

API:

- POST `/api/complaints/analyze` -> analyze image only
- POST `/api/complaints` -> create complaint (multipart: `image`, optional `category`, `description`)
- GET `/api/complaints` -> list
- PATCH `/api/complaints/:id/status` -> { status }


