# goal-tracking-system

basic goal tracking system, where particular goal can be defined and goal will have multiple task where min and max timeline can be defined and logs will be maintained

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [License](#license)

## Features

- Some key features.
1. Create a user collection
2. Create a goal collection with each user can signup / set upto 2 goals - each goal has a
min and max timeline to achieve and user can set as per his/ her timeline between it
3. Each goal has a set of tasks they need to do
4. Each task will have quantity, frequency ( one a day, twice a day, no of days days - days of
week to select from, or one a week ) and option to set reminders and there can be auto time
suggestions for the reminders also.
5. Collection to save the logs of users

## Installation

1. Clone the repository:

    ```bash
(https://github.com/AAYYUU08/goal-tracking-system)    ```

2. Navigate to the backend directory:

    ```bash
    cd goal-tracking-system/backend
    ```

3. Install dependencies:

    ```bash
    npm install
    ```

4. Set up environment variables:
   - Create a `.env` file in the `backend` directory.
   - Define the following variables:
     - `MONGO_URI`: MongoDB connection URI.
     - `JWT_SECRET`: Secret key for JWT authentication.
     - `PORT`: Port for the backend server (default is 3000).

5. Start the backend server:

    ```bash
    npm run start
    ```

6. Navigate to the frontend directory:

    ```bash
    cd ../frontend
    ```

7. Install dependencies:

    ```bash
    npm install
    ```

8. Set up environment variables:
   - Create a `.env` file in the `frontend` directory.
   - Define the following variable:
     - `REACT_APP_API_URL`: Backend API URL (e.g., `http://localhost:3000/api`).

9. Start the frontend development server:

    ```bash
    npm run dev
    ```

10. Access the application in your browser at `http://localhost:5172`.


## Usage

1. Start the development server: `npm start`
2. Open your browser and visit `http://localhost:3000`

## API Endpoints
### Authentication Endpoints (/api/auth)
- POST /register: Register a new user.
- POST /login: Login an existing user.

### Goal Endpoints (/api/goals)
- POST /: Create a new goal.
- GET /: Retrieve all goals belonging to the authenticated user.
- PUT /:goalId: Update an existing goal.
- DELETE /:goalId: Delete an existing goal.

### Task Endpoints (/api/tasks)
- POST /: Create a new task.
- GET /:goalId: Retrieve all tasks belonging to a specific goal.
- PUT /:taskId: Update the status of an existing task.
- DELETE /:taskId: Delete an existing task.

### Log Endpoints (/api/logs)
- POST /: Create a new log entry for a task.
- GET /: Retrieve all log entries belonging to the authenticated user.




## License

This project is licensed under the [MIT License](LICENSE).
