# Misinformation Detective

An interactive web application designed to improve critical thinking skills and help users detect misinformation through engaging educational games. This project aims to educate users about media literacy in a fun and interactive way.

## Table of Contents
- Overview
- Features
- Demo
- Technology Stack
- Installation
  - Prerequisites
  - Setup Instructions
- Game Descriptions
- Project Structure
- API Endpoints
- Contributing
- License

## Overview
In today's digital age, being able to identify misinformation is a crucial skill. **Misinformation Detective** provides a series of interactive games that challenge users to distinguish between real and fake content, identify reliable sources, and recognize misleading headlines—all while learning valuable media literacy skills.

## Features
- **Real or Fake Game**: Determine whether news article snippets are from legitimate sources or fabricated  
- **Guess the Headline Game**: Identify the correct headline for a given article excerpt  
- **Guess the Source Game**: Determine which publication an article excerpt came from  
- Score tracking and timing mechanics  
- Progressive difficulty levels  
- Immediate feedback with educational explanations  

## Demo
**Live Demo:** [Video Demo](https://www.youtube.com/watch?v=sU_tLRtoJYg)

## Technology Stack

**Frontend**
- React 19.0.0
- React Router 7.3.0
- TailwindCSS 4.0.15
- Node.js 23.9.0

**Backend**
- Django 5.1.7
- Django REST Framework
- SQLite3

## Installation

### Prerequisites
- Node.js (v23.9.0)  
- Python (v3.8+)  
- pip  
- nvm  

### Setup Instructions

#### Backend Setup
1. Clone the repo  
2. Navigate to `app/backend`  
3. Create and activate a virtual environment:  
   ```bash
   python -m venv venv
   source venv/bin/activate  # macOS/Linux
   venv\Scripts\activate     # Windows

Install dependencies: 
pip install -r requirements.txt

Run the server: 

python manage.py runserver
Open http://localhost:8000

Run the React app:
npm start
Open http://localhost:3000

## Game Descriptions

### Real or Fake Game
Users are presented with article snippets and must decide if they come from legitimate sources or are fabricated. Points are awarded for correct answers, with time bonuses for quick responses. The game provides educational feedback after each answer.

### Guess the Headline Game
Players are shown an article excerpt and must select the correct headline from multiple options. This game helps users recognize sensationalism and misleading headlines while developing critical reading skills.

### Guess the Source Game
Users are challenged to identify which publication an article excerpt originated from. This game teaches players to recognize the distinctive styles, biases, and content patterns of different news sources.

## Project Structure

```text
misinformation-detective/
├── app/
│   ├── backend/            Django API server
│   │   ├── game/           Game logic and models
│   │   ├── misinformation/ Project settings
│   │   └── manage.py       Django management script
│   └── frontend/           React application
│       ├── public/         Static files
│       ├── src/            React components and logic
│       │   ├── components/ Game components
│       │   └── App.js      Main application component
│       └── package.json    Frontend dependencies
└── README.md               Project documentation
```

## API Endpoints 

```text
GET    /api/real_or_fake_question/      # Get a random Real or Fake game question
POST   /api/real_or_fake_answer/        # Submit an answer for Real or Fake game

GET    /api/guess_headline_question/    # Get a random Guess the Headline game question
POST   /api/guess_headline_answer/      # Submit an answer for Guess the Headline game

GET    /api/guess_source_question/      # Get a random Guess the Source game question
POST   /api/guess_source_answer/        # Submit an answer for Guess the Source game
```

## Contributing

Fork the repository

Create your feature branch:
git checkout -b feature/amazing-feature

Commit your changes:
git commit -m "Add some amazing feature"

Push to the branch:
git push origin feature/amazing-feature
