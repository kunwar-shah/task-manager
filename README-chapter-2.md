# Task Manager Application - Chapter 2: Application Architecture and Folder Structure

This chapter focuses on setting up the application architecture and folder structure for our Task Manager application. We'll implement the MVC pattern for both frontend and backend, set up our testing environment, and begin with our first tests.

## Key Points

- MVC architecture implementation for backend and frontend
- Feature-based folder structure
- Setting up testing environment
- Writing our first tests

## Folder Structure

We'll be using the following folder structure:

```
task-manager/
│
├── backend/
│   ├── src/
│   │   ├── config/
│   │   ├── models/
│   │   ├── views/
│   │   ├── controllers/
│   │   ├── routes/
│   │   ├── middlewares/
│   │   ├── utils/
│   │   └── app.js
│   │
│   ├── tests/
│   │   ├── unit/
│   │   ├── integration/
│   │   └── e2e/
│   │
│   └── package.json
│
├── frontend/
│   ├── src/
│   │   ├── models/
│   │   ├── views/
│   │   ├── controllers/
│   │   ├── utils/
│   │   └── app.js
│   │
│   ├── public/
│   │   ├── index.html
│   │   ├── css/
│   │   └── js/
│   │
│   ├── tests/
│   │   ├── unit/
│   │   └── integration/
│   │
│   └── package.json
│
├── .gitignore
├── .eslintrc.js
├── .prettierrc
└── README.md
```

## Setup Instructions

1. Create the folder structure:
   ```bash
   mkdir -p backend/src/{config,models,views,controllers,routes,middlewares,utils}
   mkdir -p backend/tests/{unit,integration,e2e}
   mkdir -p frontend/src/{models,views,controllers,utils}
   mkdir -p frontend/public/{css,js}
   mkdir -p frontend/tests/{unit,integration}
   ```

2. Initialize npm for backend and frontend:
   ```bash
   cd backend && npm init -y && cd ..
   cd frontend && npm init -y && cd ..
   ```

3. Install necessary dependencies (we'll do this in detail in the chapter)

4. Set up ESLint and Prettier (we'll cover this in the chapter)

## MVC Implementation

### Backend MVC
- Models: Database schemas and business logic
- Views: API endpoints (RESTful API)
- Controllers: Request handling and response formation

### Frontend MVC
- Models: Data management and business logic
- Views: HTML templates and rendering logic
- Controllers: User input handling and view updates

## Testing Setup

We'll be using Jest for both backend and frontend testing. We'll cover:
- Unit testing
- Integration testing
- End-to-end testing (for backend)

## Next Steps

In this chapter, we'll:
1. Set up the folder structure
2. Implement a basic MVC structure for both backend and frontend
3. Set up the testing environment
4. Write our first tests

The next chapter will focus on implementing user authentication and authorization.