# Library Management System (LMS)

## Overview
The Library Management System (LMS) is a SQL-based application designed to streamline the operations of a library. It allows for efficient management of book lending, user tracking, and overdue monitoring. This system provides a user-friendly interface for library staff and students to manage books and transactions effectively.

## Features
- **Book Management:** Add, update, and delete books in the library database.
- **Loan Tracking:** Track the issue and return dates of borrowed books.
- **Overdue Monitoring:** Automatically identify and report overdue books.
- **User Management:** Manage user information and borrowing history.

## Technologies Used
- **Database Management System:** MySQL or Oracle Database
- **Programming Language:** SQL
- **Development Tools:** MySQL Workbench or Oracle SQL Developer
- **Version Control:** GitHub

## Database Schema
The LMS consists of three main tables:
1. **Books**
   - ISBN (Primary Key)
   - Title
   - Author
   - Genre
   - AvailabilityStatus

2. **Users**
   - UserID (Primary Key)
   - Name
   - Email (Unique)

3. **Transactions**
   - TransactionID (Primary Key)
   - UserID (Foreign Key)
   - ISBN (Foreign Key)
   - IssueDate
   - ReturnDate

## SQL Scripts
The SQL scripts for setting up the database and populating it with sample data are located in the `lms_setup.sql` file. This file includes:
- Table creation scripts
- Sample data insertion
- Common queries for managing the library

## How to Use
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/repository-name.git
   cd repository-name
