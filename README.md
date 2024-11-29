# Node.js Authentication System with MySQL
This project is a Node.js authentication system that uses MySQL for storing user data. 
It provides a secure, scalable way to manage user registration and login functionality with features like password hashing, session management, and input validation. 
This project is based on the [tutorial by Nuel Obeto](https://dev.to/nuelobeto/building-a-nodejs-authentication-system-with-mysql-a-step-by-step-guide-19l9?fbclid=IwY2xjawG2fVJleHRuA2FlbQIxMAABHQataZeWT-ZmKh2fNkqDdAuecPhRutQpA2s-mFQlq1ReqyDBPQVe6odKIQ_aem_WinSBH4wHYnNj01UaqHtMA)
, which guides you through building an authentication system from scratch. My aim is to use ths as a spike and apply it to my Diabetic Assistant App. 

## Features
- User Registration: Securely stores user information in a MySQL database.
- Login System: Authenticates users with their email and password.
- Password Hashing: Uses bcrypt for hashing passwords.
- Session Management: Implements session handling using express-session.
- Input Validation: Validates user inputs to ensure data integrity.
- Environment Configuration: Uses dotenv to manage environment variables.
  
Tech Stack
Node.js - Backend framework
- express: A popular web framework for building APIs and web applications.
- cors: Middleware for handling Cross-Origin Resource Sharing (CORS).
- dotenv: A package for managing environment variables.
- nodemon: A tool for automatically restarting the server during development.
- mysql: A MySQL database driver for Node.js.
- uuid: A package for generating universally unique identifiers (UUIDs).
- jsonwebtoken: A library for generating and verifying JSON Web Tokens (JWTs).
- bcryptjs: A library for hashing and verifying passwords securely.

## Setup
Prerequisites
Make sure you have the following installed:

Node.js (v14+)
MySQL (v8+)
Git (optional, for cloning the repository)

## Installation
1) Clone the repo
2) Install dependencies
   ```bash
   npm install
   ```
3) Set Up Environment Variables:
Create a .env file in the root directory with the following contents:
```bash
PORT=your-chosen-port
JWT_SECRET=your-jwt-secret
HOST=your-database-host
USER=your-database-user
PASSWORD=your-database password
DATABASE=your-database-name
```
## Start the Server
```bash
npm start
```
## Access the application
You can open your browser and navigate to http://localhost:your-chosen-port

## Try out the application in Postman
POST to http://localhost:your-chosen-port/register, add body -> select x-www-form-urlencoded -> add user email and user password 
POST to http://localhost:your-chosen-port/login, add body -> select x-www-form-urlencoded -> add user email and user password 

