# Building REST API with Express & TypeScript

This project is a RESTful API built with Express, TypeScript, and MongoDB.

## Features
- User Authentication (Login/Register)
- User Management (CRUD operations)
- Middleware for authentication and authorization

## Prerequisites
- Node.js (v16+)
- MongoDB Atlas account (or local MongoDB)

## Setup

1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file based on `.env.example` and add your `MONGO_URL`.
4. Start the development server:
   ```bash
   npm start
   ```

## API Documentation

### Authentication
- `POST /auth/register` - Create a new user.
- `POST /auth/login` - Authenticate a user.

### Users
- `GET /users` - Get all users (requires authentication).
- `DELETE /users/:id` - Delete a user (requires authentication and owner authorization).
- `PATCH /users/:id` - Update a user (requires authentication and owner authorization).
