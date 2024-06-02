# SwiftChat Web-App Backend

Welcome to the backend of SwiftChat, a MERN stack application that empowers real-time connections. With SwiftChat, users can chat instantly and hold video calls using Socket.io and WebRTC. The backend is designed to ensure a seamless user experience and scalability, leveraging technologies such as Node.js, Express.js, and MongoDB.

[Link to the Frontend Repository](https://github.com/swarshah09/SwiftChat-Frontend.git)
## Table of Contents

- [Features](#features)
- [Technologies](#technologies)
- [Installation](#installation)
- [Configuration](#configuration)
- [API Endpoints](#api-endpoints)
- [Usage](#usage)
  
## Features

- **Real-Time Chat:** Instant messaging using Socket.io.
- **Video Calls:** High-quality video calls using WebRTC.
- **Contact Management:** Manage contacts effortlessly.
- **Google OAuth:** Easy login with Google OAuth.
- **Scalable Backend:** Built with Node.js, Express.js, and MongoDB.

## Technologies

- **Node.js**
- **Express.js**
- **MongoDB**
- **Mongoose**
- **Socket.io** for real-time communication
- **WebRTC** for video calls
- **Passport.js** for Google OAuth authentication

## Installation

### Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/)

### Clone the Repository

```bash
git clone https://github.com/your-username/swiftchat-backend.git
cd swiftchat-backend
```

### Install Dependencies

```bash
npm install
```

## Configuration

Create a `.env` file in the root of the project with the following environment variables:

```plaintext
PORT=5000
MONGODB_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
```

## API Endpoints

### User Authentication

- **POST /api/auth/google**: Authenticate a user with Google OAuth

### Chat

- **GET /api/chats**: Get all chat rooms for the authenticated user
- **POST /api/chats**: Create a new chat room
- **GET /api/chats/:id**: Get a specific chat room
- **DELETE /api/chats/:id**: Delete a chat room

### Messages

- **GET /api/messages/:chatId**: Get all messages for a specific chat room
- **POST /api/messages/:chatId**: Send a new message to a chat room
- **DELETE /api/messages/:id**: Delete a message

## Usage

To start the server, run:

```bash
npm start
```

The backend will be running on the port specified in the `.env` file (default is 5000).

---

Thank you for using SwiftChat! We hope this app enhances your real-time communication experience. If you have any questions or feedback, feel free to contact us.
