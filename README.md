## Reach Studios - Developer Test


### Overview

The goal of this test is to assess the developer’s ability to work with Laravel, consume an external API, interact with a database, and use Blade templates to display data.

### Scenario

You are tasked with building a simple Laravel application that consumes a public API that looks up a products API and there respective categories.
We would like the use of Laravel Breeze and creation of an admin account to login with.

> [!NOTE]
> Either MySQL or SQLite, your choice!


### Instructions

+ Create a new Laravel project.
+ Set up the project to use your chosen database.
+ Set up a `.env` file with the appropriate database configuration.

> [!IMPORTANT]
> Dummy API `https://dummyjson.com/products`


### API Consumption

+ Write a service class to consume the API, that includes:
  + Fetch all products from the above link.
  + Handle possible API errors (e.g., network issues, non-200 responses).

### Database Interaction

+ Create the necessary database migrations:
  + A products table with relevant columns.
  + A category table with relevant columns.

+ Create Eloquent models for both, defining the appropriate relationships


### Data Storage

Write a command, job or a controller action to:

+ Call the API service.
+ Parse the API response.
+ Store the data in the database tables.


### Display

We are not looking for anything flashy in terms of UI, simply use what comes from Breeze to display the list of products with a blade file.


### Testing

+ Write unit tests or feature tests to ensure:
  + The API service works correctly and handles errors gracefully.
  + The data is correctly saved in the database.
  + The Blade view renders correctly and displays the data as expected.


> [!NOTE]
> Whilst we understand the time constraint, it would be good to see any tests you can write whether it be unit or feature tests.


### Documentation

+ Provide clear instructions on how to set up and run the application.
+ Include any assumptions or decisions you made while completing the task.


### Evaluation Criteria

+ Code Quality: Clear, readable, and maintainable code.
+ Laravel Best Practices: Use of Laravel features (e.g., Eloquent, Blade, Artisan commands) appropriately.
+ API Integration: Ability to consume and handle API data effectively.
+ Database Management: Proper database schema design and interaction using Eloquent.
