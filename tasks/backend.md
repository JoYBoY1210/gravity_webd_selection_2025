# Backend Tasks ⚙️

Complete all three backend tasks to demonstrate your server-side development skills.

---

## Task 1: Simple User API (15 points)

### Objective
Build a basic REST API for user management.

### Requirements
- **Endpoints**:
  - `POST /users` - Create a new user
  - `GET /users` - Get all users
  - `GET /users/:id` - Get user by ID (bonus)
- **Data Storage**: In-memory storage is acceptable
- **Data Format**:
  ```json
  {
    "id": 1,
    "name": "John Doe",
    "email": "john@example.com",
    "createdAt": "2025-01-01T00:00:00Z"
  }
  ```
- **Validation**: Basic input validation for required fields

### Evaluation Criteria
- API design and functionality (8 pts)
- Error handling and validation (4 pts)
- Code structure and documentation (3 pts)

### Technologies
- Node.js with Express.js, Python with Flask/FastAPI, or any preferred framework

---

## Task 2: Todo API (CRUD) (25 points)

### Objective
Create a complete CRUD API for managing todo items.

### Requirements
- **Endpoints**:
  - `POST /todos` - Create new todo
  - `GET /todos` - Get all todos
  - `GET /todos/:id` - Get specific todo
  - `PUT /todos/:id` - Update todo
  - `DELETE /todos/:id` - Delete todo
  - `PATCH /todos/:id/complete` - Mark todo as complete
- **Data Model**:
  ```json
  {
    "id": 1,
    "title": "Complete backend task",
    "description": "Build a CRUD API for todos",
    "completed": false,
    "priority": "medium",
    "createdAt": "2025-01-01T00:00:00Z",
    "updatedAt": "2025-01-01T00:00:00Z"
  }
  ```
- **Features**:
  - Filter todos by completion status
  - Search todos by title
  - Proper HTTP status codes

### Bonus Features (+5 pts)
- Data persistence (file-based, SQLite, or MongoDB)
- Pagination for large todo lists
- Todo categories/tags

### Evaluation Criteria
- RESTful API design (10 pts)
- CRUD operations implementation (8 pts)
- Error handling and validation (4 pts)
- Code quality and documentation (3 pts)

### Technologies
- Any backend framework of choice
- Optional: Database (SQLite/MongoDB/PostgreSQL)

---

## Task 3: Mini Authentication System (35 points)

### Objective
Implement a secure authentication system with user registration and login.

### Requirements
- **Endpoints**:
  - `POST /auth/register` - User registration
  - `POST /auth/login` - User login
  - `POST /auth/logout` - User logout
  - `GET /auth/profile` - Get authenticated user profile
- **Security Features**:
  - Password hashing (bcrypt or similar)
  - Input validation and sanitization
  - Rate limiting for auth endpoints
- **Data Model**:
  ```json
  {
    "id": 1,
    "username": "johndoe",
    "email": "john@example.com",
    "password": "$2b$10$...", // hashed
    "createdAt": "2025-01-01T00:00:00Z"
  }
  ```

### Bonus Features (+10 pts)
- JWT token implementation
- Password reset functionality
- Email verification
- Role-based access control

### Evaluation Criteria
- Security implementation (15 pts)
- API functionality and design (10 pts)
- Error handling and validation (5 pts)
- Code quality and best practices (5 pts)

### Technologies
- Backend framework of choice
- Password hashing library (bcrypt, argon2)
- Optional: JWT library, database

---

## General Requirements

### Code Quality Standards
- **Clean Code**: Well-organized, readable code with meaningful variable names
- **Error Handling**: Proper error responses with appropriate HTTP status codes
- **Documentation**: API documentation (README or inline comments)
- **Environment Variables**: Use environment variables for configuration

### API Response Format
```json
{
  "success": true,
  "data": { /* response data */ },
  "message": "Operation completed successfully"
}
```

### Error Response Format
```json
{
  "success": false,
  "error": {
    "code": 400,
    "message": "Validation failed",
    "details": ["Email is required", "Password must be at least 8 characters"]
  }
}
```

---

## Submission Guidelines

1. Create a folder: `backend/` in your submission directory
2. Organize tasks in subfolders:
   ```
   backend/
   ├── task1-user-api/
   │   ├── app.js (or main file)
   │   ├── package.json
   │   ├── README.md
   │   └── routes/
   ├── task2-todo-api/
   │   ├── app.js
   │   ├── package.json
   │   ├── README.md
   │   ├── models/
   │   └── routes/
   └── task3-auth/
       ├── app.js
       ├── package.json
       ├── README.md
       ├── middleware/
       ├── models/
       └── routes/
   ```
3. Include README.md for each task with:
   - Setup instructions
   - API documentation
   - Testing guidelines
   - Dependencies list

## Testing Your APIs 🧪

### Recommended Tools
- **Postman** - API testing and documentation
- **Thunder Client** - VS Code extension
- **curl** - Command line testing
- **Insomnia** - API client

### Example Test Cases
Include test cases in your README:
```bash
# Create user
curl -X POST http://localhost:3000/users \
  -H "Content-Type: application/json" \
  -d '{"name": "John Doe", "email": "john@example.com"}'

# Get all users
curl http://localhost:3000/users
```

## Tips for Success 💡

- **Start Simple**: Get basic functionality working first
- **Error First**: Implement error handling early
- **Test Frequently**: Test each endpoint as you build
- **Documentation**: Write clear, concise API documentation
- **Security**: Never store plain text passwords
- **Validation**: Validate all input data
- **Status Codes**: Use appropriate HTTP status codes

**Good luck! 🚀**
