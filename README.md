# 📝 Full-Stack Task Manager

A modern, full-stack task management application built with a **Go (Golang)** backend and a **React + TypeScript** frontend. This project features a robust RESTful API for all core task operations and a clean, responsive user interface built with Chakra UI.

---

## 📖 About The Project

This application provides a simple yet powerful interface for managing to-do items. It's designed with a clean separation between the frontend and backend, making it a great example of a modern, full-stack web application architecture. The backend is built in Go for performance and concurrency, while the frontend uses a modern React stack for a fast and interactive user experience.

## 🚀 Key Features

-   **Full CRUD Functionality**: Create, read, update, and delete tasks.
-   **Mark Tasks Complete/Incomplete**: Easily toggle the status of any task.
-   **Bulk Delete**: Clear all tasks with a single action.
-   **RESTful API**: A well-defined API for seamless communication between the client and server.
-   **Modern Frontend**: A responsive and accessible user interface built with React and Chakra UI.
-   **Efficient Data Fetching**: Utilizes TanStack Query for optimized data fetching and state management.

## 🛠️ Tech Stack

| Area      | Technology                                                                          |
| :-------- | :---------------------------------------------------------------------------------- |
| **Backend** | **Go (Golang)** with **Gorilla Mux** for routing |
| **Database**| **MongoDB** (with the official Go driver) |
| **Frontend**| **React 18** (with Vite), **TypeScript** |
| **UI Library**| **Chakra UI** |
| **Data Fetching**| **TanStack (React) Query**|

## 📊 API Endpoints

All API endpoints are prefixed with `/api`.

| Method   | Endpoint              | Description                    |
| :------- | :-------------------- | :----------------------------- |
| `GET`    | `/task`               | Get all tasks |
| `POST`   | `/tasks`              | Create a new task |
| `PUT`    | `/tasks/{id}`         | Mark a task as complete |
| `PUT`    | `/undoTask/{id}`      | Mark a task as not complete |
| `DELETE` | `/deleteTask/{id}`    | Delete a single task |
| `DELETE` | `/deleteAllTasks`    | Delete all tasks |

## ⚙️ Setup and Installation

### Prerequisites

-   Go (version 1.18 or higher)
-   Node.js (version 18 or higher)
-   A running MongoDB instance

### Backend Setup

1.  **Navigate to the server directory:**
    ```bash
    cd server
    ```
2.  **Install dependencies:**
    ```bash
    go mod tidy
    ```
3.  **Set up your environment variables:**
    Create a `.env` file in the `server` directory with your MongoDB connection string:
    ```
    MONGO_URI=mongodb://localhost:27017
    ```
4.  **Run the server:**
    ```bash
    go run main.go
    ```
    The server will start on `http://localhost:9000`.

### Frontend Setup

1.  **Navigate to the client directory:**
    ```bash
    cd client
    ```
2.  **Install dependencies:**
    ```bash
    npm install
    ```
3.  **Run the development server:**
    ```bash
    npm run dev
    ```
    The application will be available at `http://localhost:5173`.
