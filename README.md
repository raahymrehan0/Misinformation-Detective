# Misinformation Detective

An interactive web application designed to improve critical thinking skills and help users detect misinformation through engaging educational games.

## Features

- **Real or Fake Game**: Determine whether news article snippets are from legitimate sources or fabricated
- **Guess the Headline Game**: Identify the correct headline for given article
- **Guess the Source Game**: Determine which publication an article excerpt came from

## Technology Stack

### Frontend
- React 19.0.0
- React Router 7.3.0
- TailwindCSS 4.0.15
- Node.js 23.9.0

### Backend
- Django 5.1.7
- Django REST Framework
- SQLite3

## Setup Instructions

### Backend Setup

#### Windows
```
cd app/backend
venv\Scripts\activate
python manage.py runserver
```

#### macOS/Linux
```
cd app/backend
source venv/bin/activate
python3 manage.py runserver
```

The Django server will run on http://localhost:8000

### Frontend Setup

#### Windows/macOS/Linux
```
cd app/frontend
nvm use 23.9
npm start
```

The React app will run on http://localhost:3000