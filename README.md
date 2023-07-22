# User Authentication System Setup Guide

This guide will walk you through the installation process for setting up a user authentication system. The system uses React for the frontend and Node.js with Express for the backend. Additionally, it utilizes MongoDB as the database. Make sure you have Node.js and Git as well as mongoDB installed on your machine before proceeding.

## Tools Used
### Frontend:
- React
- react-router-dom
- Axios

### Backend:
- Node.js
- Express
- nodemon
- cors
- email-validator
- bcrypt
- cookie-parser
- dotenv
- mongoose

### Database:
- MongoDB

## Installation Process:

1. Clone the repository:
   Open your terminal or command prompt and run the following command to clone the repository:

   ```bash
   git clone git@github.com:omkeshborse/user-authentication-system.git
   cd user-authentication-system
   ```

2. Install backend dependencies:
   Change to the backend directory and install the required Node.js dependencies:

   ```bash
   cd backend
   npm install
   ```

3. Install frontend dependencies:
   Now, navigate to the client directory and install the frontend dependencies:

   ```bash
   cd ../client
   npm install
   ```

4. Create environment files:
   After installing the dependencies in both frontend and backend, you need to create environment files to store configuration settings.

   In the backend folder, create a `.env` file and add the following contents:

   ```plaintext
   PORT=8081
   MONGODB_URL=mongoDB_connection_string (without quotes) / mongodb_atlas_connection_string
   SECRET=SECRET
   CLIENT_URL=http://localhost:3000
   ```

   Replace `mongoDB_connection_string` with your MongoDB connection string. This will be used to connect the backend to the MongoDB database. Also, set a secret key for the JWT token generation by replacing `SECRET` with your desired secret key.

   In the frontend folder, create another `.env` file and add the following:

   ```plaintext
   REACT_APP_URL=http://localhost:8081
   ```

5. Start the application:
   Now that everything is set up and configured, you can run the user authentication system. Open two terminal or command prompt windows, one for the backend and the other for the frontend.

   In the backend terminal, run the following command:

   ```bash
   cd ../backend
   npm start
   ```

   This will start the backend server using nodemon, which will automatically restart the server whenever you make changes to the backend code.

   In the frontend terminal, run the following command:

   ```bash
   cd ../client
   npm start
   ```

   This will start the development server for the React frontend.

6. Access the application:
   The user authentication system should now be up and running. You can access it by navigating to http://localhost:3000 in your web browser.

That's it! You have successfully installed and set up the user authentication system using React for the frontend and Node.js with Express for the backend. Enjoy building secure user authentication features for your application!
