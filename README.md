# Social Network API

This is a RESTful API for a social network web application where users can share their thoughts, react to friends' thoughts, and create a friend list. The API is built using Express.js for routing, MongoDB for the database, and Mongoose ODM for interacting with MongoDB.

## Getting Started

To get started with the project, follow these steps:

1. Clone this repository to your local machine.
2. Install dependencies using `npm install`.
3. Ensure you have MongoDB installed and running locally on your machine.
4. Start the server using `npm start`.

## Walkthrough Video

[Link to Walkthrough Video](#) - (Include the link to your actual video here)

The walkthrough video demonstrates the functionality of the API and how to test it using Insomnia.

### Functionality Demonstrated in the Video:

- Starting the application's server.
- Testing GET routes for all users and all thoughts.
- Testing GET routes for a single user and a single thought.
- Testing POST, PUT, and DELETE routes for users and thoughts.
- Testing POST and DELETE routes for a user's friend list.
- Testing POST and DELETE routes for reactions to thoughts.

## API Routes

### Users

- `GET /api/users`: Get all users.
- `GET /api/users/:userId`: Get a single user by ID.
- `POST /api/users`: Create a new user.
- `PUT /api/users/:userId`: Update a user by ID.
- `DELETE /api/users/:userId`: Delete a user by ID.

### Friends

- `POST /api/users/:userId/friends/:friendId`: Add a friend to a user's friend list.
- `DELETE /api/users/:userId/friends/:friendId`: Remove a friend from a user's friend list.

### Thoughts

- `GET /api/thoughts`: Get all thoughts.
- `GET /api/thoughts/:thoughtId`: Get a single thought by ID.
- `POST /api/thoughts`: Create a new thought.
- `PUT /api/thoughts/:thoughtId`: Update a thought by ID.
- `DELETE /api/thoughts/:thoughtId`: Delete a thought by ID.

### Reactions

- `POST /api/thoughts/:thoughtId/reactions`: Create a reaction for a thought.
- `DELETE /api/thoughts/:thoughtId/reactions/:reactionId`: Delete a reaction for a thought.

## Repository Structure

- `controllers/`: Contains controller files for handling business logic.
- `models/`: Contains Mongoose model definitions for users, thoughts, and reactions.
- `routes/`: Contains Express.js route files.
- `server.js`: Main entry point of the application.
- `README.md`: This file.

## Technologies Used

- Express.js
- MongoDB
- Mongoose
- JavaScript

## Credits

This project was created as part of a challenge for [Your Course/Instructor Name]. Special thanks to [Instructor/Teaching Assistant Name] for guidance and support.

