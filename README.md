# Azure Task Manager ☁️✅

![CI/CD](https://github.com/krishna2198-dotcom/azure-task-manager/actions/workflows/deploy.yml/badge.svg?branch=main)

A Full Stack Task Manager app built with React.js frontend
and Flask REST API backend, connected to Azure CosmosDB (NoSQL).
Demonstrates OOP design patterns and automated CI/CD pipeline.

## Project Structure
azure-task-manager/
├── backend/         # Flask REST API (OOP Architecture)
│   ├── app.py       # Model + Repository + Service + Controller
│   └── requirements.txt
├── frontend/        # React.js UI
│   └── src/
└── .github/
    └── workflows/   # CI/CD Pipeline

## Architecture (OOP + MVC)
| Layer | Class | Responsibility |
|-------|-------|----------------|
| Model | Task | Data structure |
| Repository | TaskRepository | Database access |
| Service | TaskService | Business logic |
| Controller | Flask Routes | HTTP handling |

## Tech Stack
| Layer | Technology |
|-------|-----------|
| Frontend | React.js, JavaScript |
| Backend | Python, Flask |
| Database | Azure CosmosDB (NoSQL) |
| Hosting | Microsoft Azure App Service |
| CI/CD | GitHub Actions |
| Version Control | Git & GitHub |

## Features
- ✅ View all tasks
- ✅ Add new tasks
- ✅ Mark tasks as done/pending
- ✅ Delete tasks
- ✅ OOP architecture (Model, Repository, Service, Controller)
- ✅ Automated CI/CD with GitHub Actions

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
Create backend/.env:
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


<img width="1013" height="681" alt="project4-task-manager drawio" src="https://github.com/user-attachments/assets/33b04f84-2dc8-45a4-b586-4ee565f4d7ae" />




