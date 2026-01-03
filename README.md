# AI Agent Framework 

Overview:
This project is a custom AI Agent Framework built from scratch without using
existing agent libraries like CrewAI or AutoGen.

features:
A Flask-based AI Agent framework that accepts user tasks and processes them using
a **Planner → Executor → Reviewer** architecture.

The project provides a clean web UI with a galaxy-themed background and displays:
- Task Plan
- Execution (Final Answer)
- Review Summary
- Chat history & new chat
- REST-based orchestration
- Logs and state handling

## Project Structure

backup ai framework/
│
├── agents/
│ ├── planner.py
│ ├── executor.py
│ ├── reviewer.py
│ └── init.py
│
├── orchestrator/
│ ├── dag.py
│ └── init.py
│
├── llm/
│ ├── openai_client.py
│ └── init.py
│
├── templates/
│ ├── index.html
│ └── task.html
│
├── static/
│ └── galaxy.jpg
│
├── app.py
├── main.py
├── requirements.txt
└── README.md

## Technologies Used
- Python
- Flask
- HTML, CSS, JavaScript

## How It Works

1. User enters a task from the web interface
2. The **Planner** breaks the task into steps
3. The **Executor** generates the final answer
4. The **Reviewer** validates and summarizes the result
5. The response is shown on the UI

## How to Run Locally
1. Install Python
2. pip install -r requirements.txt
3. python app.py
4. Open http://localhost:5000

## Deployment
Deployed globally using Render cloud platform.

## Author
Second Year Engineering Student
