# CRUD App

## Overview

This is a simple CRUD (Create, Read, Update, Delete) application built with React, Express, and MySQL. The application allows users to manage a list of contacts, including their name, phone number, and email. The front end is built with React, and the back end uses Express.js to interact with a MySQL database.

## Features

- **Create**: Add a new user with a name, phone number, and email.
- **Read**: View a list of all users.
- **Update**: Modify existing user information.
- **Delete**: Remove a user from the list.

## Tech Stack

- **Frontend**: React.js, Bootstrap
- **Backend**: Node.js, Express.js
- **Database**: MySQL
- **HTTP Client**: Axios

## Getting Started

### Prerequisites

Make sure you have the following installed on your system:

- Node.js
- MySQL
- npm or yarn

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/crud-app.git
   cd crud-app
   
2. Install the dependencies:
    npm install
   
4. Set up the MySQL database:
Create a database named crud.
Use the following SQL command to create the users table:
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255),
    phone VARCHAR(15),
    email VARCHAR(255)
);

5. Start the server:
node server.js

6. Open your browser and navigate to http://localhost:3000 to view the app.

Project Structure
server.js: The main server file where the API endpoints are defined.
client/: The React frontend source code.
src/: Contains the main components (Home.js, Create.js, Update.js) and configuration files.
database/: Contains SQL scripts and database configuration.
API Endpoints
GET /: Fetches all users from the database.
POST /create: Adds a new user to the database.
PUT /update/:id: Updates the details of a user specified by id.
DELETE /delete/:id: Deletes a user specified by id
