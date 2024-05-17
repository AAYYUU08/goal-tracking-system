# goal-tracking-system

basic goal tracking system, where particular goal can be defined and goal will have multiple task where min and max timeline can be defined and logs will be maintained

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
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

1. Clone the repository: `git clone <repository-url>`
2. Navigate to the project directory: `cd project-directory`
3. Install dependencies: `npm install`

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



## Contributing

If you'd like to contribute to this project, please follow these guidelines:

1. Fork the repository
2. Create your feature branch: `git checkout -b feature-name`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request

## License

This project is licensed under the [MIT License](LICENSE).
