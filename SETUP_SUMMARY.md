# Repository Setup Summary

This repository has been successfully set up as a GitHub Copilot Coding Agent learning exercise, based on the official GitHub Skills course "Expand your team with Copilot coding agent".

## What Was Created

### Application Files

1. **Python Backend (FastAPI)**
   - `src/app.py` - Main FastAPI application
   - `src/backend/database.py` - MongoDB database configuration with sample data
   - `src/backend/routers/activities.py` - API endpoints for managing activities
   - `src/backend/routers/auth.py` - Authentication endpoints
   - `src/requirements.txt` - Python dependencies

2. **Frontend (HTML/CSS/JavaScript)**
   - `src/static/index.html` - Main HTML page
   - `src/static/app.js` - JavaScript application logic
   - `src/static/styles.css` - Styling

### Development Environment

3. **DevContainer Configuration**
   - `.devcontainer/devcontainer.json` - VS Code devcontainer configuration
   - `.devcontainer/installMongoDB.sh` - MongoDB installation script
   - `.devcontainer/postCreate.sh` - Post-creation setup
   - `.devcontainer/postStart.sh` - Container start script
   - `.devcontainer/startMongoDB.sh` - MongoDB startup script

4. **VS Code Configuration**
   - `.vscode/launch.json` - Debug configuration for FastAPI

### Documentation

5. **Project Documentation**
   - `README.md` - Main project README with exercise instructions
   - `docs/how-to-develop.md` - Development guide
   - `LICENSE` - MIT License
   - `src/README.md` - Application-specific README

6. **GitHub Configuration**
   - `.github/copilot-instructions.md` - Copilot customization file

## The Application

This is a **Mergington High School Extracurricular Activities Management System** that allows:
- Students to view available extracurricular activities
- Teachers to register students for activities (requires authentication)
- Filtering activities by day, time, and category
- Viewing participant lists and availability

### Sample Teacher Accounts
- Username: `mrodriguez`, Password: `art123` (Teacher)
- Username: `mchen`, Password: `chess456` (Teacher)
- Username: `principal`, Password: `admin789` (Admin)

## How to Use This Repository

1. **Open in Codespaces**: Click the "Code" button and select "Create codespace on copilot/setup-copilot-coding-agent"
2. **Wait for Setup**: The devcontainer will automatically install MongoDB and Python dependencies
3. **Run the Application**: Use VS Code's debugger or run `python -m uvicorn src.app:app --host 0.0.0.0 --port 8000`
4. **Access the App**: Open http://localhost:8000 in your browser

## Learning with Copilot Coding Agent

This repository is designed for learning how to:
- Enable GitHub Copilot coding agent on repositories
- Assign issues to Copilot
- Review and provide feedback on Copilot's work
- Work with Copilot on multiple parallel tasks
- Customize Copilot's workspace and instructions

## Security Note

The codebase intentionally contains a security issue for educational purposes:
- `src/backend/routers/auth.py` uses SHA-256 for password hashing (weak)
- `src/backend/database.py` uses Argon2 for password hashing (strong)

This demonstrates the difference between secure and insecure password hashing for learning purposes.

## Technology Stack

- **Backend**: Python 3.12, FastAPI, Uvicorn
- **Database**: MongoDB
- **Frontend**: Vanilla JavaScript, HTML5, CSS3
- **Development**: VS Code, Devcontainers, GitHub Codespaces

## Source

This repository structure is based on the official GitHub Skills course:
https://github.com/skills/expand-your-team-with-copilot
