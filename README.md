# Task Management Dashboard with Kanban Board

## Overview

This project is a **Task Management Dashboard** built with **Next.js**, which allows users to manage tasks through both a list view and a Kanban board view. Users can authenticate, create, edit, delete, and manage tasks with features like status updates, filtering, and sorting. The app is fully integrated with **MongoDB** for data storage, uses **JWT** for authentication.

The app is deployed on **Vercel** and includes the following main features:
- User authentication (signup/login/logout)
- Task management with CRUD operations
- Task filtering and sorting
- Responsive and user-friendly UI

## Features

### 1. **User Authentication**
- Users can sign up, log in, and log out.
- JWT-based authentication is implemented to protect routes.
- Only authenticated users can access task management features.

### 2. **Task Management**
- Users can create, edit, delete, and view tasks.
- Each task has:
  - **Title** (required)
  - **Description** (optional)
  - **Status**: "To Do", "In Progress", "Completed"
  - **Priority**: "Low", "Medium", "High"
  - **Due Date**
- Tasks can be filtered and sorted by status, priority, and due date.

### 3. **Task List Screen**
- Displays tasks in a list view.
- Users can filter and sort tasks directly from the list.
- Perform CRUD operations (create, edit, delete) from the list.

### 4. **Kanban Board Screen**
- Displays tasks in a Kanban board format with columns for each status ("To Do", "In Progress", "Completed").

### 5. **Backend API**
- Backend API built using **Node.js** and **Express**.
- CRUD operations for tasks.
- JWT authentication for user sign-up and login.
- Uses **MongoDB** as the database for storing user and task data.


## Deployed Application

You can access the deployed application [here](https://taskify-eta-ten.vercel.app/).

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/Tejaspatil06/Kanban_TaskManager.git
    cd Kanban_TaskManager
    ```

2. Install dependencies for the client:

    ```bash
    cd client
    npm install
    ```

3. Install dependencies for the server:

    ```bash
    cd backend
    npm install
    ```

## Environment Variables

Create a `.env` file in the root of the `server` directory and add the following environment variables:

```env
# .env file for the server

# Port number for the server
PORT=8000

# MongoDB connection string
MONGODB_URI=mongodb://localhost:27017/

# JWT secret key
JWT_SECRET=your_jwt_secret_key

# Frontend URL
CLIENT_URL=your_fronted_url
```

## Starting the Application

1. Start the server:

    ```bash
    cd backend
    npm start
    ```

2. Start the client:

    ```bash
    cd client
    npm run dev
    ```

## Tech Stack

- **Frontend**: NextJs, React.js, CSS, HTML, JavaScript
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JWT (JSON Web Tokens)
- **Deployment**: Render (for backend), Vercel (for frontend)

