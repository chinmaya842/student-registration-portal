# Student Registration Portal

A full-stack MERN application for managing student registrations, built as part of the TechnGlobal Full Stack Development capstone project.

## Live Demo
https://student-registration-portal-mw0z.onrender.com

## Features
- Student registration with name, email, student ID, course, and password
- Secure login with JWT stored in HTTP-only cookies
- Profile viewing and editing (update name, email, student ID, course, password)
- Delete student record
- Input validation (duplicate email check, password confirmation, required fields)

## Tech Stack
- **Frontend:** React, Redux Toolkit, React Bootstrap
- **Backend:** Node.js, Express
- **Database:** MongoDB (Mongoose)
- **Authentication:** JWT (JSON Web Tokens), bcrypt for password hashing

## API Endpoints
| Method | Endpoint | Access | Description |
|--------|----------|--------|-------------|
| POST | /api/users | Public | Register a new student |
| POST | /api/users/auth | Public | Login |
| POST | /api/users/logout | Public | Logout |
| GET | /api/users/profile | Private | Get logged-in student's profile |
| PUT | /api/users/profile | Private | Update student profile |
| DELETE | /api/users/profile | Private | Delete student record |

## Running Locally
1. Clone the repo
2. Run `npm install` in the root, then `npm install` inside `/frontend`
3. Create a `.env` file in the root with `MONGO_URI`, `JWT_SECRET`, `NODE_ENV=development`, `PORT=5000`
4. Run `npm run dev`