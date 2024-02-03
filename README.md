# Quiz Battle App

## Overview

The Quiz Battle App is a web application built with React, Express, Redux, and MongoDB, providing users with a platform to create and participate in quizzes. The app integrates with the Open Trivia Database API to fetch quiz questions, enabling users to enjoy a diverse range of trivia challenges.

## Features

1. **Home Page**

   - **Title and Slogan**: Displays the app title and a catchy slogan.
   - **Navigation Links**: Allows users to navigate to different sections, including the profile, quiz creation, and homepage.

2. **Login Page**

   - **User Authentication**: Enables users to log in using their email or username.
   - **Error Handling**: Displays error messages for unsuccessful login attempts.

3. **Profile Page**

   - **User Information**: Shows user profile details, including the profile picture, username, and past quiz scores.
   - **Quiz History**: Displays a list of past quizzes with corresponding scores.

4. **Quiz Creator Page**

   - **Create a Quiz**: Lets users specify the number of questions, category, difficulty, and type of questions.
   - **Generate Game Code**: Generates a unique game code for the created quiz.

5. **Quiz Page**

   - **Quiz Gameplay**: Manages the quiz by displaying questions, handling user answers, and showing the leaderboard after completing the quiz.
   - **Timer**: Implements a countdown timer for each question, creating a time-sensitive quiz experience.

## Getting Started

Follow these steps to set up and run the Quiz Battle App:

### Prerequisites

- Node.js installed on your machine.
- MongoDB running locally or a valid MongoDB Atlas connection string.
- Open Trivia Database API key.

### Installation

1. Install dependencies for both the server and client:

   ```bash
   cd backend
   npm install
   cd ../frontend
   npm install
   ```

2. Set up environment variables:

   - Create a `.env` file in the `backend` directory with the following content:

     ```
     MONGO_URI=your-mongodb-connection-string
     OPENTDB_API_KEY=your-opentdb-api-key
     ```

### Running the App

1. Start the Express server:

   ```bash
   cd backend
   npm start
   ```

   The server will run on http://localhost:5000.

2. In a separate terminal, start the React client:

   ```bash
   cd frontend
   npm start
   ```

   The React app will run on http://localhost:3000.

3. Open your web browser and go to http://localhost:3000 to access the Quiz Battle App.

## Usage

- Navigate through the app using the provided links in the navigation bar.
- Create quizzes using the Quiz Creator page.
- Join quizzes using the generated game code.
- Enjoy the quiz gameplay and compete with others on the leaderboard.

## Credits

- React: A JavaScript library for building user interfaces. [React Documentation](https://reactjs.org/docs/getting-started.html)
- Express: A fast, unopinionated, minimalist web framework for Node.js. [Express Documentation](https://expressjs.com/)
- Open Trivia Database: A free-to-use database of trivia questions. [Open Trivia Database](https://opentdb.com/)
