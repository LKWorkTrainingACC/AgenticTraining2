# OctoFit Tracker

A modern multi-tier application for activity tracking, team management, and competitive leaderboards.

## Project Structure

```
octofit-tracker/
├── frontend/          # React 19 + Vite (Port: 5173)
│   ├── src/
│   ├── public/
│   ├── package.json
│   ├── vite.config.js
│   └── .env
├── backend/           # Node.js + Express + TypeScript (Port: 8000)
│   ├── src/
│   ├── package.json
│   ├── tsconfig.json
│   └── .env
└── .gitignore
```

## Stack

- **Frontend**: React 19, Vite, React Router, Bootstrap
- **Backend**: Node.js, Express, TypeScript
- **Database**: MongoDB with Mongoose ODM
- **Ports**: Frontend (5173), Backend (8000), MongoDB (27017)

## Setup Instructions

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd octofit-tracker/backend
   ```

2. Dependencies are already installed. To install again:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

   Or compile to JavaScript and run:
   ```bash
   npm run build
   npm start
   ```

The backend will run on `http://localhost:8000`

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd octofit-tracker/frontend
   ```

2. Dependencies are already installed. To install again:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

The frontend will run on `http://localhost:5173`

### Database Setup

Ensure MongoDB is running on `localhost:27017`. The backend will automatically connect to the `octofit-tracker` database.

To check if MongoDB is running:
```bash
ps aux | grep mongod
```

## Features (To Be Implemented)

- [ ] User authentication and profiles
- [ ] Activity logging and tracking
- [ ] Team creation and management
- [ ] Competitive leaderboard
- [ ] Personalized workout suggestions

## API Endpoints (To Be Implemented)

- `GET /` - API root
- `GET /health` - Health check

## Development Workflow

1. Start MongoDB
2. Start the backend server (`npm run dev` in backend directory)
3. Start the frontend server (`npm run dev` in frontend directory)
4. Access the app at `http://localhost:5173`

## Build for Production

### Backend
```bash
cd octofit-tracker/backend
npm run build
npm start
```

### Frontend
```bash
cd octofit-tracker/frontend
npm run build
```

The built frontend will be in `dist/` directory.
