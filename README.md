CRUD App
Overview
This is a simple CRUD (Create, Read, Update, Delete) application built with React, Express, and MySQL. The application allows users to manage a list of contacts, including their name, phone number, and email. The front end is built with React, and the back end uses Express.js to interact with a MySQL database.

Features
Create: Add a new user with a name, phone number, and email.
Read: View a list of all users.
Update: Modify existing user information.
Delete: Remove a user from the list.
Tech Stack
Frontend: React.js, Bootstrap
Backend: Node.js, Express.js
Database: MySQL
HTTP Client: Axios
Getting Started
Prerequisites
Make sure you have the following installed on your system:

Node.js
MySQL
npm or yarn
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/crud-app.git
cd crud-app
Install the dependencies:

bash
Copy code
npm install
or

bash
Copy code
yarn install
Set up the MySQL database:

Create a database named crud.
Use the following SQL command to create the users table:
sql
Copy code
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255),
    phone VARCHAR(15),
    email VARCHAR(255)
);
Start the server:

bash
Copy code
node server.js
Run the React application:

bash
Copy code
npm start
or

bash
Copy code
yarn start
Open your browser and navigate to http://localhost:3000 to view the app.

Project Structure
server.js: The main server file where the API endpoints are defined.
client/: The React frontend source code.
src/: Contains the main components (Home.js, Create.js, Update.js) and configuration files.
database/: Contains SQL scripts and database configuration.
API Endpoints
GET /: Fetches all users from the database.
POST /create: Adds a new user to the database.
PUT /update/:id: Updates the details of a user specified by id.
DELETE /delete/:id: Deletes a user specified by id.
Troubleshooting
Common Issues:
Ensure your MySQL server is running and the database is properly configured.
Check that the API server is running on port 8081 and the React app on port 3000.

