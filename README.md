# DayTrack Backend

A REST API backend for the DayTrack daily task and mood tracker application.

## Tech Stack

- Node.js
- Express.js
- MongoDB Atlas
- Mongoose

## Features

- Task management (create, read, delete)
- Mood tracking
- Notes with secret/password protection
- Security middleware (helmet, cors, rate limiting, xss protection)

## Getting Started

### Prerequisites

- Node.js installed
- MongoDB Atlas account

### Installation

1. Clone the repo
```bash
   git clone https://github.com/chika-12/dayTrack-backend.git
   cd daytrack-backend
```

2. Install dependencies
```bash
   npm install
```

3. Create a `.env` file in the root folder

4. Start the server
```bash
   npm run dev
```

## API Endpoints

### Tasks
| Method | Route | Description |
|---|---|---|
| GET | `/api/v1/tasks` | Get all tasks |
| POST | `/api/v1/tasks` | Create a task |
| DELETE | `/api/v1/tasks/:id` | Delete a task |

### Moods
| Method | Route | Description |
|---|---|---|
| GET | `/api/v1/moods` | Get mood |
| POST | `/api/v1/moods` | Save a mood |

### Notes
| Method | Route | Description |
|---|---|---|
| GET | `/api/v1/notes` | Get all notes |
| POST | `/api/v1/notes` | Create a note |
| DELETE | `/api/v1/notes/:id` | Delete a note |

## Security

- Helmet for HTTP headers
- CORS configured for Vercel frontend
- Rate limiting on all API routes
- XSS protection
- NoSQL injection protection
- HTTP Parameter Pollution protection

## Deployment

- Frontend: [Vercel](https://day-track-pi.vercel.app)
- Backend: Render
- Database: MongoDB Atlas

## Author

Chika Ndukwe Mark