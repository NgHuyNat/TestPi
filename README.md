# TestHostPi Node.js Server

A simple Node.js web server built with Express.js for the TestHostPi project.

## Features

- 🚀 Express.js web server
- 🌐 RESTful API endpoints
- 🛡️ CORS enabled
- 📁 Static file serving
- 🔧 Environment variable configuration
- 🔄 Auto-restart with nodemon (development)
- ✅ Health check endpoint
- 📝 JSON request/response handling

## Prerequisites

- Node.js (version 14 or higher)
- npm (Node Package Manager)

## Installation

1. Clone or download this project
2. Navigate to the project directory:
   ```bash
   cd TestHostPi
   ```
3. Install dependencies:
   ```bash
   npm install
   ```

## Usage

### Development Mode (with auto-restart)

```bash
npm run dev
```

### Production Mode

```bash
npm start
```

The server will start on port 3000 by default. You can change this by setting the `PORT` environment variable in the `.env` file.

## API Endpoints

### Base URL

- `GET /` - Welcome message and server status

### Health Check

- `GET /api/health` - Server health and system information

### Users (Example API)

- `GET /api/users` - Get all users
- `POST /api/users` - Create a new user
  - Body: `{ "name": "string", "email": "string" }`

## Environment Variables

Create a `.env` file in the root directory with the following variables:

```env
NODE_ENV=development
PORT=3000
```

## Project Structure

```
TestHostPi/
├── index.js          # Main application file
├── package.json      # Project dependencies and scripts
├── .env             # Environment variables
├── .gitignore       # Git ignore rules
├── README.md        # Project documentation
└── public/          # Static files (will be created when needed)
```

## Available Scripts

- `npm start` - Run the server in production mode
- `npm run dev` - Run the server in development mode with nodemon
- `npm test` - Run tests (not implemented yet)

## Technologies Used

- **Express.js** - Web application framework
- **CORS** - Cross-Origin Resource Sharing middleware
- **dotenv** - Environment variable loader
- **nodemon** - Development auto-restart tool

## Contributing

1. Fork the project
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## License

This project is licensed under the ISC License.
