# CI/CD Demo Project

A simple project demonstrating CI/CD pipeline with Python Flask backend and Angular frontend.

## Project Structure
```
CICD/
├── backend/          # Python Flask API
├── frontend/         # Angular application
├── .github/workflows # CI/CD pipeline
└── docker-compose.yml
```

## Quick Start

### Backend (Python Flask)
```bash
cd backend
pip install -r requirements.txt
python app.py
```
API will be available at http://localhost:5000

### Frontend (Angular)
```bash
cd frontend
npm install
npm start
```
App will be available at http://localhost:4200

### Docker
```bash
docker-compose up --build
```

## API Endpoints
- `GET /api/health` - Health check
- `GET /api/users` - Get users list

## CI/CD Pipeline
The GitHub Actions pipeline:
1. **Test Backend** - Runs Python tests
2. **Test Frontend** - Builds Angular app
3. **Deploy** - Deploys on main branch

## Testing
```bash
# Backend tests
cd backend && pytest

# Frontend build test
cd frontend && npm run build
```