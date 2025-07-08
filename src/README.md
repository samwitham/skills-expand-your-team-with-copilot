# Mergington High School Activities

A full-stack web application that enables teachers to manage student extracurricular activities at Mergington High School. Built with FastAPI backend and modern responsive frontend.

## Features

### For Students and Teachers
- View all available extracurricular activities with detailed information
- Advanced filtering and search capabilities:
  - Search activities by keyword
  - Filter by category (Sports, Arts, Academic, Community, Technology)
  - Filter by day of the week
  - Filter by time (Before School, After School, Weekend)
- Responsive design that works on desktop and mobile devices

### For Teachers (Authentication Required)
- Secure login system for teachers
- Register students for activities
- Remove students from activities
- Manage student participation

### Technical Features
- FastAPI-based REST API with automatic documentation
- MongoDB database integration
- Professional responsive UI with modern styling
- Real-time activity updates and filtering

## API Endpoints

The application provides a REST API with the following key endpoints:

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/activities` | Get all activities with optional filtering by day and time |
| GET | `/activities/days` | Get list of all days that have activities scheduled |
| POST | `/activities/{activity_name}/signup` | Register a student for an activity (teacher authentication required) |
| POST | `/activities/{activity_name}/unregister` | Remove a student from an activity (teacher authentication required) |
| POST | `/auth/login` | Teacher login authentication |
| GET | `/auth/check-session` | Validate teacher session |

> **Note**: Interactive API documentation is available at `/docs` when running the application.

## Technology Stack

- **Backend**: FastAPI with Python
- **Database**: MongoDB
- **Frontend**: Vanilla JavaScript, HTML5, CSS3
- **Authentication**: Session-based with password hashing
- **Deployment**: ASGI server (Uvicorn)

## Development Guide

For detailed setup and development instructions, please refer to our [Development Guide](../docs/how-to-develop.md).
