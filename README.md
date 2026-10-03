# Movie Database CLI

A Python command-line application for managing and querying a MySQL movie database.

The project models movies and their relationships with actors, characters, technicians, production houses, genres, awards, trailers, and other movie information.

## Features

The command-line application supports:

- Adding and updating movies
- Adding and updating production houses
- Adding and updating trailers
- Adding technicians, actors, characters, and awards
- Deleting trailers
- Updating technician departments
- Searching for movies and technicians
- Finding actors and characters based on movie information
- Querying technicians by department
- Running analytical SQL queries on movie data
- Counting movies by genre
- Finding maximum profit for each production house
- Analyzing awards by genre and category

## Technology Used

- Python
- MySQL
- PyMySQL
- SQL

## Database Design

The database uses a relational schema with tables including:

- `Movie`
- `Actor`
- `Technician`
- `Production_House`
- `Genre_Movie`
- `ACTED_IN`
- `Char_acter`
- `Award`
- `Category_Award`
- `Trailer`
- `WORKS_FOR`
- `Released_Languages_Movie`
- `Animated_Movie`
- `Feature_Film`
- `Documentary`
- `Short_Film`
- `COLLABORATION`

The schema uses primary keys and foreign keys to represent relationships between entities.

## SQL Query Operations

The application includes several types of database queries.

### Search

Search movies by name and technicians by name.

### Selection

Examples include:

- Find characters played by a given actor
- Find actors associated with a specified genre

### Projection

Examples include:

- Find actors who have appeared in at least a specified number of movies
- Find technicians belonging to a specified department

### Analysis

Examples include:

- Find production houses associated with movies whose collections exceed the recent average
- Count awards by genre and award category

### Aggregation

Examples include:

- Find the maximum profit for each production house
- Count the total number of movies in each genre

## Command-Line Interface

After connecting to the database, the application provides a menu with options for database operations and queries.

```text
1.  Add Movie
2.  Delete Trailer
3.  Production house analysis
4.  Award analysis
5.  Actor character lookup
6.  Actor genre lookup
7.  Actor movie-count query
8.  Technician department query
9.  Search technicians
10. Search movies
11. Maximum profit by production house
12. Movie count by genre
13. Update Movie
14. Update Production House
15. Update Trailer
16. Update Technician Department
17. Add Trailer
18. Add Award
19. Add Technician
20. Add Production House
21. Add Actor
22. Add Character
0.  Exit
