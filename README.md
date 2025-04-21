
# Airbnb

This project is a web application that replicates the core functionalities of Airbnb, allowing users to book accommodations, manage listings, and handle bookings seamlessly. Built with a modern tech stack, this application aims to provide a user-friendly experience similar to Airbnb.
## Features

- User Registration and Authentication
- Profile Management
- Property Listings with detailed descriptions
- Image Upload and Management
- Booking System for reservations
- User Dashboards to manage properties and bookings
- Responsive design for mobile and desktop users
## Tech Stack

- **Frontend:**
  - React
  - Redux
  - MUI (Material-UI)
  - SASS
  - React Router

- **Backend:**
  - Node.js
  - Express.js
  - MongoDB (Mongoose for ORM)
  - JWT for authentication
  - Multer for image uploads

- **Development Tools:**
  - Nodemon for automatic server restarts
  - ESLint for code quality# API Routes

## Authentication

- `POST /register`
  - Registers a new user.
  - **Request Body**: `{ "name": String, "email": String, "password": String }`
  
- `POST /login`
  - Authenticates a user and returns a JWT token.
  - **Request Body**: `{ "email": String, "password": String }`
  
- `POST /logout`
  - Logs out the user by clearing the JWT token.
  
- `GET /profile`
  - Retrieves the logged-in user's profile information.

## Image Uploads

- `POST /upload-by-link`
  - Downloads an image from a provided link.
  - **Request Body**: `{ "link": String }`
  
- `POST /upload`
  - Uploads images sent from a form.
  - **Form Data**: `photos` (multiple files)

## Places

- `POST /places`
  - Creates a new place entry.
  - **Request Body**: 
    ```json
    {
      "title": String,
      "address": String,
      "addedPhotos": Array,
      "description": String,
      "price": Number,
      "perks": Array,
      "extraInfo": String,
      "checkIn": String,
      "checkOut": String,
      "maxGuests": Number
    }
    ```
  
- `GET /user-places`
  - Retrieves all places owned by the logged-in user.
  
- `GET /places/:id`
  - Retrieves a place by its ID.
  
- `PUT /places`
  - Updates an existing place.
  - **Request Body**: 
    ```json
    {
      "id": String,
      "title": String,
      "address": String,
      "addedPhotos": Array,
      "description": String,
      "perks": Array,
      "extraInfo": String,
      "checkIn
## Run Locally

Clone the project

```bash
  git clone https://github.com/Geetansh431/Airbnb-1.0
```
Go to the backend directory

```bash
  cd server
```

Install dependencies

```bash
  npm install
```

create **.env file** 

Start the server

```bash
  npm run start
```

Go to the frontend directory using Other Terminal

```bash
  cd ../
```

Install dependencies

```bash
  npm install
```

Start the server

```bash
  npm run start
```


# .env.example

- MongoDB Connection String: YOUR_MONGO_URL

## Demo

Live Link Coming Soon
## Contributing to Airbnb 🤝

We welcome and appreciate contributions from the community to enhance and improve Airbnb. Whether you're a developer, designer, tester, or someone with valuable feedback, your input is valuable to us.

## Thank You!❤️

Thank you for considering contributing to the Airbnb. Your efforts help make this project better for everyone. If you have any questions or need assistance, feel free to reach out through the issue tracker or discussions. Happy coding🤩!
