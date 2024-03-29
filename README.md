# Task API with Django Authentication

This is a Django REST Framework (DRF) API for managing tasks with authentication features including login, sign-up, and sign-out functionalities.

## Features

### User authentication (login, sign-up, sign-out) using Django authentication system.
### CRUD operations for tasks (Create, Read, Update, Delete).
### Ability to mark tasks as completed.

## Technologies Used

Django
Django REST Framework
Python
SQLite

## Installation

### Clone the repository:

git clone https://github.com/david5465/Django-crud-api

### Install dependencies:

pip install -r requirements.txt

### Apply migrations:

python manage.py migrate

### Run the development server:

python manage.py runserver

## Endpoints

POST /signup/: Sign up a new user.

POST /login/: Login and obtain an authentication token.

POST /logout/: Logout and invalidate the authentication token.

GET /tasks/: Retrieve all tasks.

POST /tasks/create/: Create a new task.

GET /tasks/<task_id>/: Retrieve a specific task.

PUT /tasks/<task_id>/: Update a task.

DELETE /tasks/<task_id>/: Delete a task.

## Authentication

For accessing protected endpoints, include the authentication token in the Authorization header of your requests.

Obtain the token by making a POST request to /login/ with valid credentials.

## Usage

Sign up for an account using the /api/signup/ endpoint.

Log in using the /login/ endpoint to obtain an authentication token.

Use the obtained token to access protected endpoints.

Perform CRUD operations on tasks using the provided endpoints.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.