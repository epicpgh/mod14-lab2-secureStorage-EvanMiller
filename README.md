# mod14-lab2-secureStorage-EvanMiller
# mod14SBAsecure-web-portal-EvanMiller


# 🚀 Innovate Inc. User Portal API

This is a secure Express.js backend application that provides user authentication via GitHub OAuth and a protected API for managing personal notes. We were introduced to Passport.js, bcrypt, and continued refining our practice of building routes and using jsonwebtokens for verification of data.

---

Software Used

    Node.js + Express.js

    MongoDB + Mongoose

    Passport.js (Local + GitHub OAuth2.0)

    JWT for authentication

    bcrypt for password hashing

    dotenv for configuration


| Method | Endpoint                         | Description                          |
|--------|----------------------------------|--------------------------------------|
| POST   | `/api/users/register`            | Register with email and password     |
| POST   | `/api/users/login`               | Login and receive JWT                |
| GET    | `/api/users/auth/github`         | Start GitHub OAuth flow              |
| GET    | `/api/users/auth/github/callback`| Handle GitHub OAuth callback         |


All endpoints require a Bearer JWT in the `Authorization` header.

| Method | Endpoint                       | Description                         |
|--------|--------------------------------|-------------------------------------|
| GET    | `/api/bookmarks`              | Get all bookmarks (user-specific)   |
| GET    | `/api/bookmarks/:id`          | Get a single bookmark               |
| POST   | `/api/bookmarks`              | Create a new bookmark               |
| PUT    | `/api/bookmarks/:id`          | Update an existing bookmark         |
| DELETE | `/api/bookmarks/:id`          | Delete a bookmark 


