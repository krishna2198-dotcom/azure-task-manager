# Azure Task Manager ☁️✅

A Full Stack Task Manager app built with React.js frontend 
and Flask REST API backend, connected to Azure CosmosDB (NoSQL).

## Project Structure
azure-task-manager/
├── backend/ # Flask REST API
├── frontend/ # React.js UI

## Tech Stack
| Layer | Technology |
|-------|-----------|
| Frontend | React.js, JavaScript |
| Backend | Python, Flask |
| Database | Azure CosmosDB (NoSQL) |
| Hosting | Microsoft Azure App Service |
| Version Control | Git & GitHub |

## Features
- ✅ View all tasks
- ✅ Add new tasks
- ✅ Mark tasks as done/pending
- ✅ Delete tasks
- ✅ Real-time updates from CosmosDB

## How to Run Locally

### Backend
cd backend
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python app.py

### Frontend
cd frontend
npm install
npm start

## Environment Variables
Create `backend/.env` with:
COSMOS_ENDPOINT=your_cosmos_endpoint
COSMOS_KEY=your_cosmos_key
COSMOS_DATABASE=taskdb
COSMOS_CONTAINER=tasks

## API Endpoints
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | / | Health check |
| GET | /tasks | Get all tasks |
| POST | /tasks | Add a new task |
| PUT | /tasks/<id> | Update a task |
| DELETE | /tasks/<id> | Delete a task |
