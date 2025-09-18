# TeamSync - B2B Project Management Platform

## Project Overview

TeamSync is a powerful and scalable multi-tenancy project management system built with the MERN stack (MongoDB, Express.js, React, Node.js). It's designed for modern B2B collaboration needs, featuring comprehensive workspace management, project tracking, and team collaboration tools.

## Key Features

- 🔐 **Authentication**
  - Google OAuth Integration
  - Email & Password Authentication
  - Secure Session Management

- 🏢 **Workspace Management**
  - Create and Manage Multiple Workspaces
  - Member Invitations
  - Role-Based Access Control (Owner, Admin, Member)

- 📊 **Project Management**
  - Projects & Epics Organization
  - Task Management (CRUD operations)
  - Priority & Status Tracking
  - Assignee Management

- 🔍 **Advanced Features**
  - Comprehensive Search & Filters
  - Analytics Dashboard
  - Pagination Support
  - Data Integrity with Mongoose Transactions

## Tech Stack

### Backend
- Node.js
- MongoDB with Mongoose
- TypeScript
- Express.js
- Google OAuth2

### Frontend
- React.js
- TypeScript
- TailwindCSS
- Shadcn UI
- Vite.js

## Getting Started

### Prerequisites
- Node.js (LTS version)
- MongoDB instance
- Google OAuth credentials

### Environment Setup

1. Create a `.env` file in the backend directory:

```plaintext
PORT=8000
NODE_ENV=development
MONGO_URI=your_mongodb_connection_string
SESSION_SECRET=your_session_secret
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
GOOGLE_CALLBACK_URL=http://localhost:8000/api/auth/google/callback
FRONTEND_ORIGIN=http://localhost:3000
FRONTEND_GOOGLE_CALLBACK_URL=http://localhost:3000/google/callback
```

### Installation & Running

1. Backend Setup:
```bash
cd backend
npm install
npm run dev
```

2. Frontend Setup:
```bash
cd client
npm install
npm run dev
```

The application will be available at:
- Frontend: http://localhost:3000
- Backend: http://localhost:8000

## Project Structure

```
├── backend/
│   ├── src/
│   ├── package.json
│   └── tsconfig.json
└── client/
    ├── src/
    ├── public/
    └── package.json
```

## Features Documentation

### Authentication Flow
- Implements secure OAuth 2.0 with Google
- Session-based authentication
- Secure cookie management

### Workspace Management
- Multi-tenancy support
- Hierarchical team structure
- Granular permission system

### Project & Task Management
- Hierarchical project organization
- Real-time task updates
- Priority and status tracking
- Assignment and tracking system

## Development

### Code Style
- TypeScript for type safety
- ESLint configuration
- Prettier formatting

### Database Design
- MongoDB with Mongoose schemas
- Transaction support
- Optimized queries

## Deployment

1. Configure production environment variables
2. Build the frontend: `npm run build`
3. Start the production server: `npm start`

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a pull request

## License

This project is licensed under the MIT License.

