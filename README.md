# Todo App Backend with Node.js, Express, and TypeScript

This project is a small and simple Todo app backend built with Node.js, Express, and TypeScript. The backend supports CRUD operations for managing todo items.

## Table of Contents

- [Todo App Backend with Node.js, Express, and TypeScript](#todo-app-backend-with-nodejs-express-and-typescript)
  - [Table of Contents](#table-of-contents)
  - [Features](#features)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running the Application](#running-the-application)
  - [API Endpoints](#api-endpoints)
    - [Create a Todo](#create-a-todo)
    - [Get All Todos](#get-all-todos)
    - [Update a Todo](#update-a-todo)
    - [Delete a Todo](#delete-a-todo)
  - [Project Structure](#project-structure)
  - [Contributing](#contributing)
  - [License](#license)

## Features

- Built with Node.js and Express
- Utilizes the latest features of TypeScript
- Implements CRUD operations for todo items
- Provides a clear and maintainable code structure
- Includes comprehensive type safety

## Prerequisites

Make sure you have the following installed on your machine:

- Node.js
- npm (Node Package Manager)

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/todo-app-backend.git
   cd todo-app-backend
   ```

2. Install the dependencies:
   ```bash
   npm install
   ```

## Running the Application

To start the development server, run:

```bash
npm run dev
```

This will start the server with nodemon, which automatically restarts the server on file changes.

To build and run the production server, run:

```bash
npm run build
npm start
```

## API Endpoints

### Create a Todo

- **URL:** `api/v1/todos`
- **Method:** `POST`
- **Body:**
  ```json
  {
    "text": "Sample Todo"
  }
  ```
- **Response:**
  ```json
  {
    "text": "Sample Todo"
  }
  ```

### Get All Todos

- **URL:** `api/v1/todos`
- **Method:** `GET`
- **Response:**
  ```json
  [
    {
      "text": "Sample Todo"
    }
  ]
  ```

### Update a Todo

- **URL:** `api/v1/todos/:id`
- **Method:** `PATCH`
- **Body:**
  ```json
  {
    "text": "Updated Todo"
  }
  ```
- **Response:**
  ```json
  {
    "text": "Updated Todo"
  }
  ```

### Delete a Todo

- **URL:** `api/v1/todos/:id`
- **Method:** `DELETE`
- **Response:**
  ```json
  {
    "message": "Todo deleted successfully"
  }
  ```

## Project Structure

```
├── src
│   ├── controllers
│   │   └── todoController.ts
│   ├── models
│   │   └── todo.ts
│   ├── routes
│   │   └── todoRoutes.ts
│   ├── app.ts
│   └── server.ts
├── .env
├── .gitignore
├── package.json
├── README.md
├── tsconfig.json
└── nodemon.json
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any changes.

1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature-branch`)
5. Open a pull request

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---
