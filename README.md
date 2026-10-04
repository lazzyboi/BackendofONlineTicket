# Online Movie Ticket Booking System

This project is a Python-based Database Management System mini-project that provides a graphical interface for managing movie information.

The application uses **Tkinter** for the graphical user interface and **SQLite** for database operations.

## Features

The system provides a desktop GUI for managing movie records.

Main operations include:

- Add new movie records
- Display stored movie records
- Search movie records
- Delete movie records
- Update movie information
- Clear input fields
- Exit the application

## Movie Information

Each movie record contains:

- Movie ID
- Movie Name
- Release Date
- Director
- Cast
- Budget
- Duration
- Rating

## Technologies Used

- **Python 3**
- **Tkinter** — Graphical User Interface
- **SQLite3** — Database management
- **SQL** — Database queries

No third-party Python packages are required.

## Project Structure

```text
DBMS/
│
├── dbms/
│   ├── frontend.py
│   └── MiniProject_Backend.py
│
├── png.jpg
└── README.md
```

## Architecture

The application follows a simple frontend/backend structure.

```text
              +----------------------+
              |     Tkinter GUI      |
              |     frontend.py      |
              +----------+-----------+
                         |
                         v
              +----------------------+
              |     Backend Layer    |
              | MiniProject_Backend  |
              +----------+-----------+
                         |
                         v
              +----------------------+
              |       SQLite         |
              |      movie1.db       |
              +----------------------+
```

### `frontend.py`

Responsible for:

- Creating the graphical interface
- Receiving user input
- Displaying movie records
- Handling button actions
- Calling backend database functions

### `MiniProject_Backend.py`

Responsible for:

- SQLite database connection
- Creating the movie table
- Inserting records
- Retrieving records
- Searching records
- Deleting records
- Updating records

## Database

The application uses SQLite and stores movie data in:

```text
movie1.db
```

The movie table contains fields for:

```text
id
Movie_ID
Movie_Name
Release_Date
Director
Cast
Budget
Duration
Rating
```

## Requirements

Install Python 3.x.

Tkinter and SQLite3 are part of the standard Python distribution.

To verify Python:

```bash
python --version
```

## Running the Project

Open a terminal inside the `dbms` directory:

```bash
cd dbms
```

Run:

```bash
python frontend.py
```

The graphical interface will launch.

## Using the Application

### Add Movie

Enter the movie information and select:

```text
Add New
```

### Display Movies

Select:

```text
Display
```

to retrieve movie records from the database.

### Search Movies

Enter the required movie information and select:

```text
Search
```

### Update Movie

Select an existing movie record, modify the information, and use:

```text
Update
```

### Delete Movie

Select a record and choose:

```text
Delete
```

### Clear

Use:

```text
Clear
```

to reset the input fields.

## Database Operations

The backend implements functions for:

```text
MovieData()
AddMovieRec()
ViewMovieData()
DeleteMovieRec()
SearchMovieData()
UpdateMovieData()
```

These functions provide the database CRUD layer:

```text
Create
Read
Update
Delete
```

## Project Objective

The purpose of this project is to demonstrate practical Database Management System concepts using Python, including:

- Database connectivity
- SQL operations
- CRUD operations
- GUI-based database applications
- SQLite database management
- Frontend/backend separation

## Current Limitations

The current source contains SQL syntax issues in the database initialization and update queries that should be corrected before relying on those operations in a fresh database.

The project is intended as an academic DBMS mini-project and can be extended with:

- User authentication
- Seat selection
- Theatre management
- Show timings
- Ticket booking
- Payment integration
- Booking history
- Movie recommendations
- Improved database normalization
- Better validation and error handling

## Future Enhancements

A future version can evolve the current movie-management system into a complete movie ticket booking platform with separate entities for:

```text
Users
Movies
Theatres
Screens
Shows
Seats
Bookings
Payments
```

## Academic Project

This project was developed as a DBMS mini-project to demonstrate database operations using Python, Tkinter, and SQLite.
