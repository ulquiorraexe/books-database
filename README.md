# Books Database with Flask and SQLAlchemy

## Overview
This project demonstrates how to use **Flask** in combination with **SQLAlchemy** to build a simple database application for managing books. It allows you to create, read, update, and delete records for books, including their title, author, and rating.

The project is set up to use an **SQLite** database, which stores information about books in a local database file (`new-books-collection.db`).

## Features
- **Create** new book records.
- **Read** all or specific book records.
- **Update** existing book records by title or primary key.
- **Delete** book records by primary key.
  
## Requirements
- Python 3.x
- Flask
- Flask-SQLAlchemy
- SQLAlchemy

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ulquiorraexe/books-database.git
2. Navigate to the project directory:
   ```bash
   cd books-database
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
   This will install:
     - Flask
     - Flask-SQLAlchemy
     - SQLAlchemy
5. Run the application:
   ```bash
   python main.py

## Usage

### Database Setup

The project is set up with SQLite. The database URI is configured as:
```python
app.config['SQLALCHEMY_DATABASE_URI'] = "sqlite:///new-books-collection.db"
```
When you run the application, SQLAlchemy automatically creates the required database file if it doesn't already exist.

## Code Explanation

This project uses **Flask** to build a simple web app with a SQLite database, managed by **Flask-SQLAlchemy**.
  - `app.py` sets up the application, connects to the database, and handles the routes for creating, reading, updating, and deleting book records.
  - The `Book` class is the SQLAlchemy model representing a book in the database.
  - The database URI is configured as `sqlite:///new-books-collection.db`, which creates a local SQLite database file.

## License

This project does not have a license.
