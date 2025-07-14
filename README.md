# College Management API

A straightforward RESTful API designed to handle college student and course data, built using Node.js.

## Project Overview

This API facilitates the management of educational resources within a college environment. It features:

- User authentication with distinct roles: admin and staff
- Comprehensive course management (create, read, update, delete)
- Student management along with course enrollment capabilities
- Role-based access control to secure sensitive API routes

## Developer Information

**Name:** Pranav Bhandari
**Roll Number:** 221732
**Class:** BESE 'Day' - 6th Semester

## Technology Stack

- **Backend:** Node.js with Express framework
- **Database:** MongoDB, interfaced via Mongoose
- **Authentication:** JSON Web Tokens (JWT) and bcrypt for password hashing
- **Deployment:** Containerized using Docker

## API Endpoints

### Authentication Routes

- `POST /api/auth/register` - Register a new user account
- `POST /api/auth/login` - Authenticate user and receive a token
- `GET /api/auth/me` - Retrieve profile info of the logged-in user

### Course Routes

- `GET /api/courses` - Fetch all courses
- `GET /api/courses/:id` - Get details for a specific course
- `POST /api/courses` - Create a new course (admin access only)
- `PUT /api/courses/:id` - Modify course details (admin access only)
- `DELETE /api/courses/:id` - Delete a course (admin access only)

### Student Routes

- `GET /api/students` - Retrieve list of all students
- `GET /api/students/:id` - Get detailed information about a student
- `POST /api/students` - Add a new student record (admin only)
- `PUT /api/students/:id` - Update existing student information (admin only)
- `DELETE /api/students/:id` - Remove a student record (admin only)
- `POST /api/students/:id/enroll` - Assign a student to a course (admin only)

---

Feel free to reach out if you want me to add usage examples, setup instructions, or anything else!
