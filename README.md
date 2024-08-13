## Reach Studios - Developer Test


### Overview

The goal of this test is to assess the developer’s ability to work with Laravel, consume an external API, interact with a database, and use Blade templates to display data.

### Scenario

You are tasked with building a simple Laravel application that consumes a public API that provides book and author data.
The application should save this data into a database and display the books and authors using Blade templates.

> [!NOTE]
> Either MySQL or SQLite, your choice!


### Instructions

+ Create a new Laravel project.
+ Set up the project to use your chosen database.
+ Set up a `.env` file with the appropriate database configuration.

> [!IMPORTANT]
> We would like you to use `https://openlibrary.org/developers/api`


### API Consumption

+ Write a service class in Laravel to consume the API. This service should:
  + Fetch a list of books along with their associated authors.
  + Handle possible API errors (e.g., network issues, non-200 responses).

### Database Interaction

+ Create the necessary database migrations:
  + A books table with columns like id, title, description, author_id, published_date, etc.
  + An authors table with columns like id, name, bio, etc.

+ Create Eloquent models for Book and Author, defining the appropriate relationships


### Data Storage

Write a command, job or a controller action to:

+ Call the API service.
+ Parse the API response.
+ Store the data in the database tables.


### Display

Whilst we are looking at Laravel specific skills we are not really interested on the UI side of things, therefore a simple blade file to display this info would be sufficient.

Create a Blade view to display the list of books. Each book should display:
+ The title of the book.
+ The name of the author.
+ The publication date.
+ A brief description of the book.


### Testing (TDD)

Whilst we understand the time constraint, it would be good to see any tests you can write whether it be unit or feature tests.


### Documentation

Provide clear instructions on how to set up and run the application.
Include any assumptions or decisions you made while completing the task.


### Submission

The completed project, either as a GitHub repository or a zipped file, along with any additional documentation should be provided to `lee.stables@reachstudios.co.uk`
