# Auth API (TypeScript + Express + Postgres)

Endpoints (all under `/api/auth`):

| Method | Path     | Body                        | Returns                  |
|--------|----------|-----------------------------|--------------------------|
| POST   | /signup  | `{ name, email, password }` | `{ user, token }` (201)  |
| POST   | /login   | `{ email, password }`       | `{ user, token }`        |
| GET    | /me      | header `Authorization: Bearer <token>` | `{ user }`    |

The login/signup page is served at `/`. Health check: `GET /health`.

