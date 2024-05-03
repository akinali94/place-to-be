# Place-To-Be

## Shared Locations Application

This full-stack web application built with MERN allows users to share their locations along with images. Other users can view these shared locations, and the application provides functionalities for image upload and input validation.

## Features

- **User Authentication**: Users can sign up, log in, and log out securely using JWT tokens.
- **Authorization**: Certain routes and actions are restricted to authenticated users.
- **Location Sharing**: Users can add their locations along with images to share with others. Google Maps API is integrated to facilitate finding and displaying locations accurately.
- **View Shared Locations**: Other users can browse through the shared locations and images.
- **Image Upload**: The application supports uploading images along with location information.
- **Input Validation**: Robust validation ensures data integrity and security.
- **CRUD Operations**: Full CRUD functionality for managing shared locations.

## Tech Stack

- **Frontend**: React
- **Backend**: Node.js, Express
- **Database**: MongoDB
- **Authentication**: JSON Web Tokens (JWT)

## API Reference

#### Retrieve list of all users

```http
  GET /api/users/
```

#### Create new user + log user in

```http
  POST /api/users/signup
```

#### Create new user + log user in

```http
  POST /api/users/login
```

#### Retrieve list of all places for a given user id (uid)

```http
  GET /api/places/user/:uid
```

#### Get a specific place by place id (pid)

```http
  POST /api/places/:pid
```

#### Create a new place

```http
  POST /api/places/
```

#### Update a place by id (:pid)

```http
  PATCH /api/places/:pid
```

#### Delete a place by id (pid)

```http
  DELETE /api/places/:pid
```
