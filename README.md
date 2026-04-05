🤖 AI Choose Your Own Adventure Game
A dynamic, interactive storytelling application where the narrative evolves based on player choices. This project utilizes an 
AI-driven backend and a Tree Data Structure to manage complex branching paths, ensuring every playthrough is unique.

🚀 Key Features
AI-Generated Narratives: Leverages Large Language Models to generate immersive story segments on the fly.

Branching Logic (Tree DS): Implemented a custom Tree data structure in the backend to map user decisions to story nodes, preventing "logical loops" and managing state efficiently.

React-Powered Frontend: A modern, responsive UI built with React and Vite for seamless transitions between story segments.

State Persistence: Tracks player progress and allows for "Game Over" or "Victory" conditions based on the path taken.

🏗️ Technical Architecture
Backend (Python/Flask)
The core of the game is the Story Tree. Each node in the tree represents a specific "state" of the story.

Tree Implementation: Each Node contains the story text, a set of child nodes (options), and the AI-generated context.

API Integration: Communicates with AI APIs to fetch creative text based on the parent node's context.

Frontend (React/Vite)
Axios: Used for robust communication with the Python backend.

React Router: Manages navigation between the home screen and the active game session.

🛠️ Installation & Setup

Prerequisites

Python 3.10+
Node.js & npm

Backend Setup

cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
"Add your API Key to a .env file"

Frontend Setup

cd frontend
npm install
npm run dev
