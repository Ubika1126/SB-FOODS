# Food Ordering App (MERN)

This is a full-stack food ordering application built using the MERN (MongoDB, Express, React, Node.js) stack. Users can browse menus, add items to their cart, and place orders. The application also features user authentication and an admin panel to manage menu items and orders.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

---

## Features

- **User Authentication**: Signup, login, and logout functionality.
- **Browse Menu**: Users can browse food items, categorized by type.
- **Cart Management**: Add items to the cart, update quantities, and calculate total price.
- **Order History**: Users can view their past orders.
- **Admin Panel**: Admin users can add, update, and delete food items and view orders.
- **Responsive Design**: Optimized for both mobile and desktop use.

## Technologies Used

- **Frontend**: React, Redux, Axios
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JSON Web Token (JWT)
- **Styling**: CSS, Bootstrap

## Installation

To set up and run this project locally, follow these steps:

### Prerequisites

- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/)

### Steps

1. **Clone the repository:**

   ```bash
   git clone https://github.com/AHBRIJESH/Food-Ordering-App-Mern-NM.git
   cd Food-Ordering-App-Mern-NM
   ```

2. **Install dependencies** for both client and server:

   ```bash
   cd client
   npm install
   cd ../server
   npm install
   ```

3. **Environment Variables**:
   Create a `.env` file in the `server` folder and add the following variables:

   ```plaintext
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret_key
   ```

4. **Run MongoDB** (if not hosted):

   ```bash
   mongod --port 27017
   ```

5. **Start the application:**

   - Start the server:
     ```bash
     cd server
     npm start
     ```

   - Start the client:
     ```bash
     cd ../client
     npm start
     ```

6. **Access the App**:
   Open your browser and navigate to `http://localhost:3000`.

## Usage

1. **Register and Login** to access the features.
2. Browse the **menu** and add items to your cart.
3. **Place orders** and view order history.
4. **Admin users** can manage the menu and orders from the Admin Panel.

## Project Structure

The project is divided into client and server directories:

```plaintext
Food-Ordering-App-MERN/
├── client/              # React frontend
│   ├── public/          # Public assets
│   ├── src/             # React components, Redux, utilities
│   └── package.json     # Client dependencies
├── server/              # Express backend
│   ├── config/          # MongoDB and JWT configuration
│   ├── controllers/     # Request handlers
│   ├── models/          # Mongoose models
│   ├── routes/          # API routes
│   ├── middleware/      # JWT authentication
│   └── server.js        # Server entry point
└── package.json         # Project dependencies
```

## Contributing

Feel free to submit issues or pull requests. Please ensure that your contributions align with the project's goals and structure.

