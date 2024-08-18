# Bookstore CRUD Application

## Overview

This is a simple CRUD (Create, Read, Update, Delete) application for managing books. It is built using Symfony, a PHP framework, and it allows users to:

- List all books
- View details of a specific book
- Add a new book
- Edit an existing book
- Delete a book

## Project requirements

Idea of this task is to refactor the previous book site using Symfony 7

- Create a new “web” folder, rename previous “web” to something else
- Use the Symfony console to generate a new entity e.g.

```bash
php bin/console make:entity Book
```

- Add properties to the Book entity such as tile, author, publishingYear, genre and description
- Set up the database
- Configure the .env file with correct database connection details
- Create the database and schema

```bash
php bin/console doctrine:database:create
```

- Do necessary database migration command
- Add twig template

### Specs

1. Create a “web” folder inside of src of Symfony-MAMP
2. Feel free to use any CSS styling, HTML/Twig syntax
3. Keep it simple

## Features

- **Book Management**: Manage books with fields `title`, `author`, and `description`.
- **Form Handling**: Create and update books using Symfony forms.
- **Database Integration**: Uses Doctrine ORM to interact with a MySQL or MariaDB database.

## Prerequisites

- PHP 8.0 or higher
- Composer
- MySQL or MariaDB database server

## Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/the-sankari/symfony-bookstore.git
   ```

2. Install Dependencies

3. Ensure you have Composer installed. Run the following command to install project dependencies:

```bash
composer install
```

4. Configure the Environment
5. Copy the .env file to .env.local and configure your database connection:
   DATABASE_URL=mysql://username:password@localhost:3306/bookstore
6. Replace username, password, localhost, and 3306 with your actual database credentials.

7. Create the Database

8. Create the database (if it doesn’t already exist):

```bash
php bin/console doctrine:database:create
Run Migrations
```

9. Apply the migrations to create the necessary database schema:

```bash
php bin/console doctrine:migrations:migrate
```

10. Running the Application
11. Start the Symfony Server

You can use the Symfony CLI tool or PHP's built-in server. For Symfony CLI:

```bash
symfony server:start
```

For PHP built-in server:

```bash
php bin/console server:run
```

12. Access the Application

13. Open your web browser and go to http://127.0.0.1:8000 to access the application.

### Usage

List Books: Visit /books to view a list of all books.
View Book Details: Visit /book/{id} to see details of a specific book.
Add New Book: Visit /book/new to add a new book.
Edit Book: Visit /book/{id}/edit to edit an existing book.
Delete Book: Use the delete button in the book list or detail view to remove a book.
Troubleshooting
Database Connection Errors: Ensure that your database server is running and that your .env.local file has the correct database credentials.

14. Cache Issues: If you encounter any issues, try clearing the Symfony cache:

```bash
php bin/console cache:clear
```

### Error Logs:

Check var/log/dev.log or var/log/prod.log for detailed error messages if something is not working as expected.

### Contributing

Feel free to fork this repository and submit pull requests. For major changes or features, please open an issue to discuss before making changes.

### License

This project is licensed under the MIT License. See the LICENSE file for details.

### Contact

For any questions or issues, you can reach out to me or open an issue in the GitHub repository.

### Summary

- **Overview**: Provides a brief description of the project.
- **Features**: Lists the key functionalities.
- **Prerequisites**: Details the software needed to run the project.
- **Installation**: Step-by-step instructions to set up the project.
- **Running the Application**: Instructions to start the server and access the app.
- **Usage**: How to interact with the application.
- **Troubleshooting**: Common issues and solutions.
- **Contributing**: Guidelines for contributing to the project.
- **License**: Information about the project's license.
- **Contact**: How to get in touch or report issues.
### Assigned by
- [Santosh Kalwar](https://github.com/kalwar)
### Author

- [kajol](https://github.com/the-sankari)
