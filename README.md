📦 AI Inventory Demand Predictor
🚀 Overview

This project is a full-stack inventory management system that allows users to:

Add and manage products
Track inventory levels
Predict future demand using a simple Machine Learning model

The goal was to build a clean, modular, and reliable system using a modern tech stack while keeping the design simple and maintainable.

🏗️ Architecture

The system follows a layered client-server architecture:

React Frontend → Flask API → SQLite Database
                             → ML Prediction Service
Components:
Frontend (React):
Handles UI and user interactions
Displays products and predictions
Sends API requests to backend
Backend (Flask):
Exposes REST APIs
Handles business logic
Validates input data
Database (SQLite):
Stores product information
ML Service:
Predicts demand using Linear Regression
🧠 Tech Stack
Layer	Technology
Frontend	React
Backend	Flask (Python)
Database	SQLite (SQLAlchemy)
ML Model	Scikit-learn
Validation	Marshmallow
📂 Project Structure
inventory-ai-app/

backend/
  app/
    routes/        # API endpoints
    models/        # Database models
    services/      # ML logic
    schemas/       # Validation schemas
    __init__.py
  run.py

frontend/
  src/
    App.js

README.md
agents.md
⚙️ Setup Instructions
🔹 Backend Setup
cd backend
pip install -r requirements.txt
python run.py
🔹 Frontend Setup
cd frontend
npm install
npm start
✅ Features
Add new products
View all products
Delete products
Predict demand using ML model
Clean UI dashboard
Real-time updates (no page reload)
🧠 Key Technical Decisions
1. Flask for Backend
Chosen for simplicity, flexibility, and quick API development
2. SQLite Database
Lightweight and easy to set up for a small-scale application
3. Modular Architecture

Separated into:

Routes (API layer)
Models (data layer)
Services (business logic)
Schemas (validation)

Benefits:

Maintainability
Scalability
Easy debugging
4. Simple ML Model
Used Linear Regression to:
Keep system lightweight
Ensure interpretability
Avoid over-engineering
🛡️ Interface Safety & Validation
Input validation implemented using Marshmallow schemas
Prevents invalid or missing data
Ensures consistent API structure
Avoids runtime errors
🔍 Observability
Error handling implemented in frontend and backend
Clear API error messages
Loading and error states handled in UI
🔁 Change Resilience
Modular code design ensures new features can be added easily
Changes in one layer do not affect others
Clear separation of concerns
🧪 Verification
APIs tested manually using browser/Postman
Edge cases handled:
Missing product
Invalid inputs
Frontend reflects real-time updates
🤖 AI Usage

AI tools were used for:

Generating initial boilerplate code
Structuring backend architecture
Debugging errors
Improving UI design

Important Note:

All AI-generated code was:

Carefully reviewed
Manually tested
Refactored for clarity and correctness
⚖️ Tradeoffs
Used simple Linear Regression instead of advanced time-series models
No authentication system implemented
No pagination for large datasets
Minimal UI styling to prioritize functionality
🔮 Future Improvements
Add authentication (JWT-based login)
Use advanced ML models (ARIMA, LSTM)
Add analytics dashboard with charts
Implement pagination and filtering
Deploy on cloud (AWS / Render)
