# Task Manager API

A **Node.js** CRUD API with a **MongoDB** Database. You can check the API [here](https://tasks-management-api.herokuapp.com/)

- Users can create their account
- Can generate JWT tokens
- Users can upload their avatars
- Users can add tasks to their account

## Requirements

- NodeJS
- MongoDB
- SendGrid API Keys

## How to use?

- Clone the repository.
- Navigate to the repository and run `npm install`.
- Add your **SendGrid API keys**, **Database route** and **JWT Secret** to the `config/dev.env` file.
- Type `npm run dev` to start the dev server.

## Endpoints

- `/users` to create account
- `/users/login` to login
- `/users/logout` to logout of the current device
- `/users/logoutAll` to logout of all devices
- `/users/me` to read authenticated profile
- `/users/me` to read, update and delete authenticated user
- `/users/me/avatar` to upload avatar
- `/tasks` to read all the tasks
  - `?completed=<true/false>` to get tasks based on whether they are completed or not
  - `?limit=__&skip=__` for pagination
  - `?sort:<asc/desc>` to sort tasks based on their date
- `/tasks/<ID>` to get, update and delete a task by its ID

## License

> MIT
