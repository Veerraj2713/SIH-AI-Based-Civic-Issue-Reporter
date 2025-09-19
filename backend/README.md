# Backend

Environment variables:

- `PORT` default 4000
- `MONGODB_URI` e.g. `mongodb://127.0.0.1:27017/sih_solutions`

Scripts:

- `npm run dev` - start with nodemon
- `npm start` - start server

Routes:

- `POST /api/complaints` multipart form-data: `image` file, optional `category`, `description`
- `GET /api/complaints` list complaints
- `PATCH /api/complaints/:id/status` body: `{ status }`

Uploads are served from `/uploads`.


