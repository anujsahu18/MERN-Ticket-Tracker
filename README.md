# MERN Ticket Tracker

A simple ticket management web application built using the MERN stack. I worked on setting up the project locally, connecting it with MongoDB, and getting the frontend and backend running together.

## About the Project

This project is designed to manage support tickets in one place. Users can create an account, log in, and manage tickets through a simple web interface.

The project helped me understand how a React frontend communicates with an Express/Node.js backend and how MongoDB is used to store application data.

## Features

* User registration and login
* JWT based authentication
* Create and manage tickets
* Ticket status management
* MongoDB database integration
* REST API using Express.js
* React based frontend
* Responsive and simple interface

## Tech Stack

**Frontend**

* React.js
* Axios
* CSS

**Backend**

* Node.js
* Express.js
* JWT
* bcryptjs

**Database**

* MongoDB
* Mongoose

## Project Structure

```text
MERN-Ticket-Tracker/
│
├── client/          # React frontend
├── middleware/      # Authentication middleware
├── models/          # MongoDB models
├── routes/          # API routes
├── config/          # Local configuration
├── server.js        # Backend entry point
├── package.json
└── README.md
```

## Running the Project Locally

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
cd MERN-Ticket-Tracker
```

### 2. Install backend dependencies

```bash
npm install
```

### 3. Install frontend dependencies

```bash
npm install --prefix client
```

### 4. Configure MongoDB

Make sure MongoDB is running locally.

Create:

```text
config/default.json
```

Add:

```json
{
  "MONGO_URI": "mongodb://127.0.0.1:27017/ticket-tracker",
  "JWT_SECRET": "your_secret_key"
}
```

> Keep `config/default.json` private. It is ignored by Git.

### 5. Start the application

For the backend:

```bash
npm start
```

The backend runs on:

```text
http://localhost:5000
```

For the frontend, open another terminal and run:

```bash
set NODE_OPTIONS=--openssl-legacy-provider
npm start --prefix client
```

The frontend runs on:

```text
http://localhost:3000
```

## Database

The application uses MongoDB locally with the database name:

```text
ticket-tracker
```

Mongoose is used to connect the Node.js backend with MongoDB.

## What I Learned

While working on this project, I got practical experience with:

* MERN stack project structure
* REST APIs
* React and Express integration
* MongoDB and Mongoose
* User authentication with JWT
* Password hashing with bcrypt
* Running frontend and backend together
* Git and GitHub workflow

## Future Improvements

Some things I would like to improve in the future:

* Add better ticket filtering and search
* Add user roles such as admin and support staff
* Improve the UI
* Add ticket priority and due dates
* Deploy the application online

