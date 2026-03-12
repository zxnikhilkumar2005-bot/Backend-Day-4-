# Day-4 Backend (Express)

A simple Express.js backend project with a basic notes API.

## Features

- Express server setup
- JSON request body parsing
- Health/basic route: `GET /`
- Notes creation route: `POST /notes`

## Project Structure

```text
Day-4/
|-- server.js
|-- package.json
|-- src/
|   `-- app.js
```

## Requirements

- Node.js (recommended: v18+)
- npm

## Installation

```bash
npm install
```

## Run the Project

### Development mode (with nodemon)

```bash
npm run dev
```

Server runs at:

```text
http://localhost:3000
```

## API Endpoints

### 1. GET `/`

Returns a simple message.

Response:

```text
Hello world
```

### 2. POST `/notes`

Creates a note by pushing request body into an in-memory `notes` array.

Request body example:

```json
{
  "title": "My note",
  "description": "This is my first note"
}
```

Response:

```text
note created
```

## Important Notes

- Notes are stored in memory only.
- Data will be lost when the server restarts.
- There is no validation for request body fields yet.

## Future Improvements

- Add note validation
- Add `GET /notes` endpoint
- Persist data in a database
- Add error handling middleware
