# Dummy API for Postman Tutorials

This is a simple REST API built with Express.js that you can use to practice Postman. It includes endpoints for managing users and posts.

## Setup

1. Install dependencies:
```bash
npm install
```

2. Start the server:
```bash
npm start
```

The server will run on `http://localhost:3000`

## Available Endpoints

### Users

- `GET /api/users` - Get all users
- `GET /api/users/:id` - Get a specific user
- `POST /api/users` - Create a new user
- `PUT /api/users/:id` - Update a user
- `DELETE /api/users/:id` - Delete a user

### Posts

- `GET /api/posts` - Get all posts
- `GET /api/posts/:id` - Get a specific post
- `POST /api/posts` - Create a new post

## Example Requests

### Create a new user
```http
POST /api/users
Content-Type: application/json

{
    "name": "Alice Johnson",
    "email": "alice@example.com"
}
```

### Create a new post
```http
POST /api/posts
Content-Type: application/json

{
    "title": "My First Post",
    "content": "This is the content of my first post",
    "userId": 1
}
```

## Notes

- This is a dummy API with in-memory storage. Data will be reset when the server restarts.
- All endpoints return JSON responses.
- The API includes basic error handling for common scenarios. 