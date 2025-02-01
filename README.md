# WorkoutBuddy - MERN Stack Exercise Tracker

A full-stack web application built using the MERN (MongoDB, Express.js, React.js, Node.js) stack that allows users to track their workouts. This project demonstrates core concepts of full-stack development including REST API creation, database operations, state management, and user authentication.

## Features

- Create, read, update, and delete workout records
- User authentication system
- Protected routes for authenticated users
- Personal workout dashboard for each user
- Responsive design

## Tech Stack

- **Frontend**: React.js
  - React Router for navigation
  - Context API for state management
  - Custom hooks for data fetching
  - Modern React practices (Hooks, Functional Components)

- **Backend**: Node.js & Express.js
  - RESTful API architecture
  - JWT (JSON Web Token) authentication
  - MongoDB database integration
  - MVC pattern

- **Database**: MongoDB
  - Mongoose ODM
  - Timestamp tracking
  - Data validation

## Project Structure

```
workout-buddy/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── context/
│   │   ├── hooks/
│   │   ├── pages/
│   │   └── App.js
│   └── package.json
│
└── backend/
    ├── controllers/
    ├── models/
    ├── routes/
    ├── server.js
    └── package.json
```

## Installation

1. Clone the repository
```bash
git clone https://github.com/your-username/workout-buddy.git
cd workout-buddy
```

2. Install backend dependencies
```bash
cd backend
npm install
```

3. Install frontend dependencies
```bash
cd ../frontend
npm install
```

4. Set up environment variables
Create a `.env` file in the backend directory:
```
PORT=4000
MONGO_URI=your_mongodb_connection_string
```

## Running the Application

1. Start the backend server (from the backend directory)
```bash
npm run dev
```

2. Start the frontend development server (from the frontend directory)
```bash
npm start
```

The application will be available at `http://localhost:4000`

## API Endpoints

### Workouts
- `GET /api/workouts` - Get all workouts
- `GET /api/workouts/:id` - Get single workout
- `POST /api/workouts` - Create new workout
- `DELETE /api/workouts/:id` - Delete a workout
- `PATCH /api/workouts/:id` - Update a workout

### Authentication
- `POST /api/user/signup` - Register a new user
- `POST /api/user/login` - Login user

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request
