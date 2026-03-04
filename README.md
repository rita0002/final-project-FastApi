# FastAPI Task Management System

A simple backend REST API built using **FastAPI** that allows users to manage tasks.
The application stores task data in a text file using **JSON Lines format**, ensuring persistence even after server restarts.

## Features

* Create tasks
* View all tasks
* View a task by ID
* Update tasks
* Delete a task
* Delete all tasks
* Filter tasks by completion status
* View task statistics

## Project Structure

```
fastapi-tasks
│
├── main.py           # FastAPI application and API endpoints
├── helpers.py        # file handling functions for loading/saving tasks
├── models.py         # Pydantic models for task validation
├── tasks.txt         # storage file for tasks (JSON lines format)
├── requirements.txt  # project dependencies
└── README.md
```

## Installation

Clone the repository

```
git clone https://github.com/YOUR_USERNAME/fastapi-tasks.git
cd fastapi-tasks
```

Create virtual environment

```
python -m venv venv
```

Activate environment

Windows

```
venv\Scripts\activate
```

Install dependencies

```
pip install -r requirements.txt
```

## Run the Application

```
uvicorn main:app --reload
```

Open the API documentation in your browser

```
http://127.0.0.1:8000/docs
```

## Example Task Format

Tasks are stored in `tasks.txt` in JSON Lines format:

```
{"id":1,"title":"Learn FastAPI","description":"Watch tutorial","completed":false}
{"id":2,"title":"Buy groceries","description":"Milk","completed":true}
```

## Author

Suman Das
