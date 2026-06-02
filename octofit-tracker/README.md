# OctoFit Tracker

A modern multi-tier application with a React frontend and Node.js/Express backend.

## Project Structure

```
octofit-tracker/
├── frontend/      # React 19 + Vite (Port 5173)
└── backend/       # Node.js + Express + TypeScript (Port 8000)
```

## Frontend Setup

- **Framework**: React 19
- **Build Tool**: Vite
- **Port**: 5173
- **Language**: JavaScript/JSX

### Frontend Commands

```bash
cd frontend
npm install  # Already done
npm run dev  # Start development server
npm run build  # Build for production
```

## Backend Setup

- **Runtime**: Node.js
- **Framework**: Express
- **Language**: TypeScript
- **Port**: 8000
- **Database**: MongoDB (Port 27017)
- **ODM**: Mongoose

### Backend Commands

```bash
cd backend
npm install  # Already done
npm run dev  # Start development server with ts-node
npm run build  # Compile TypeScript to JavaScript
npm start  # Run compiled JavaScript
```

## Environment Variables

### Backend (.env)

```
PORT=8000
MONGODB_URI=mongodb://localhost:27017/octofit
NODE_ENV=development
```

## Dependencies Installed

### Frontend
- react (19.2.6)
- react-dom (19.2.6)
- vite
- eslint

### Backend
- express
- mongoose
- typescript
- ts-node
- cors
- dotenv
- @types/node
- @types/express
- @types/cors

## Getting Started

1. **Start MongoDB** (if running locally):
   ```bash
   mongod
   ```

2. **Start Backend**:
   ```bash
   cd octofit-tracker/backend
   npm run dev
   ```

3. **Start Frontend** (in a new terminal):
   ```bash
   cd octofit-tracker/frontend
   npm run dev
   ```

4. Open http://localhost:5173 in your browser

## API Endpoints

- `GET /` - API welcome message
- `GET /health` - Health check endpoint

## Notes

- Frontend runs on port 5173 (Vite default)
- Backend runs on port 8000
- MongoDB should run on port 27017
- CORS is enabled for cross-origin requests from frontend to backend
- TypeScript configuration uses "bundler" for module resolution
