Following API Design in Node.js, v5 on Frontend Masters

- Install Node.js on your system. <= 23

- Install the required packages (node_modules) using npm:

  ```bash
  npm install
  ```

- Create a new file named **.env** in the root directory. Use **.env.example** as example.

# Project Structure

habit-habits-api/
├── env.ts # Environment configuration
├── src/
│ ├── index.ts # Application entry point
│ └── server.ts # Express app definition
├── .env # Development environment variables
├── .env.test # Test environment variables
├── .env.example # Environment template
└── package.json

# RESTful Route Patterns

// Resource: Users
GET /api/users // Get all users
GET /api/users/123 // Get specific user
POST /api/users // Create new user
PUT /api/users/123 // Update entire user
PATCH /api/users/123 // Update user fields
DELETE /api/users/123 // Delete user

// Nested resources
GET /api/users/123/habits // Get user's habits
POST /api/users/123/habits // Create habit for user
DELETE /api/users/123/habits/456 // Delete specific habit
