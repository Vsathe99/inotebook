# Notebook Application

This is a full-stack web application for managing notes. Users can create, edit, delete, and search for notes. The application also supports user authentication and profile management.

## Features

- User authentication (Sign Up, Login)
- Create, edit, and delete notes
- Mark notes as important
- Search notes by title, description, or content
- User profile with note statistics
- Responsive design using Tailwind CSS

## Tech Stack

### Frontend
- React.js
- Tailwind CSS
- React Router DOM
- Jodit React (Rich Text Editor)
- HTML React Parser

### Backend
- Node.js
- Express.js
- MongoDB (Mongoose for ORM)
- JSON Web Tokens (JWT) for authentication
- Bcrypt.js for password hashing

## Installation

### Prerequisites
- Node.js and npm installed
- MongoDB installed and running locally

### Clone the Repository
```bash
git clone <repository-url>
cd notebook
```

### Install Dependencies

#### Frontend
```bash
cd frontend
npm install
```

#### Backend
```bash
cd backend
npm install
```

## Running the Application

### Start the Backend
```bash
cd backend
npx nodemon
```

The backend will run on `http://localhost:8000`.

### Start the Frontend
```bash
cd frontend
npm start
```

The frontend will run on `http://localhost:3000`.

## Folder Structure

### Frontend
- `src/components`: Reusable React components (e.g., Navbar, Note, Oops)
- `src/pages`: Pages for routing (e.g., Home, Login, Profile)
- `src/tools`: Utility components (e.g., CheckBox)
- `src/index.js`: Entry point for the React app
- `tailwind.config.js`: Tailwind CSS configuration

### Backend
- `models`: Mongoose models for MongoDB (e.g., User, Notes)
- `routes`: API routes (e.g., user authentication, note management)
- `app.js`: Main server file

## API Endpoints

### User Authentication
- `POST /signUp`: Register a new user
- `POST /login`: Login an existing user
- `POST /getUserDetails`: Fetch user details

### Notes Management
- `POST /getNotes`: Fetch all notes for a user
- `POST /addNote`: Add a new note
- `POST /updateNote`: Update an existing note
- `POST /deleteNote`: Delete a note
- `POST /getNote`: Fetch a single note by ID

## Environment Variables

The backend connects to MongoDB using the default local connection string. Update the connection string in `models/userModel.js` and `models/noteModel.js` if needed.

## Testing

### Frontend
Run the following command to execute tests:
```bash
cd frontend
npm test
```

### Backend
Use tools like Postman or cURL to test API endpoints.

## Deployment

1. Build the frontend:
   ```bash
   cd frontend
   npm run build
   ```
2. Deploy the `frontend/build` folder and the backend server to your hosting platform.

## License

This project is licensed under the MIT License.

## Acknowledgments

- [React](https://reactjs.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Express](https://expressjs.com/)
- [MongoDB](https://www.mongodb.com/)
