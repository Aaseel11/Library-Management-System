# Library Management System

A relational database system built with Microsoft Access to manage a library's core operations: book registration, borrower records, and borrowing/return transactions — replacing manual, error-prone paper tracking with an accurate, searchable digital system.

> **Note:** This project is a Microsoft Access database (`.accdb`). It requires Microsoft Access (2007 or later) installed to open and run. There is no live browser demo — see the screenshots below for a full walkthrough of the system, and the accompanying presentation for a complete project overview.

## Project Objectives

- **Organize Book Data** — Register every book with its author, publisher, publication year, and subject category
- **Manage Borrowers** — Store complete borrower records: name, phone number, email, and address
- **Track Borrowing & Returns** — Link every transaction to its due date and actual return date automatically
- **Reduce Manual Errors** — Replace paper records with an accurate database that's easy to search and update

## Database Design

The system is built around 4 linked tables, connected through One-to-Many relationships via primary and foreign keys — the **Borrowing** table connects to both **BOOK** and **BORROWER**, while **BOOK** connects to **Category**.

### Tables Structure

| Table | Fields |
|-------|--------|
| **BOOK** | ID • Title • Author • Publisher • YearPublisher • Category |
| **BORROWER** | ID • FirstName • LastName • PhoneNumber • Email • Address |
| **Borrowing** | ID • BookID • BorrowerID • BorrowerDate • DueDate • ReturnDate |
| **Category** | CategoryID • CategoryName • Description |

### Entity Relationship Diagram

[ER Diagram included in project files]

## Screenshots

### Data Entry Forms

- **Book Form** — Add and edit book records
- **Borrowing Form** — Log borrowing and return transactions
- **Category Form** — Manage book categories
- **Borrower Form** — Register and update borrower information

### Sample Data & Queries

- **Books Table** — Searchable book inventory
- **Borrowers Table** — Complete borrower directory
- **Queries** — Retrieve specific information such as books in a given category or overdue borrowing transactions

## Key Features

✓ Automatic linking between books and borrowers through the Borrowing table  
✓ Precise tracking of due dates and actual return dates for every transaction  
✓ Flexible book categorization (science, history, literature…) that can grow  
✓ Easy-to-use forms for entering and editing data  
✓ Ready-made queries for fast, accurate data retrieval  

## Technologies Used

- **Microsoft Access 2016** — Database design, forms, queries
- **Relational Database Concepts** — Primary/Foreign Keys, One-to-Many relationships

## Project Documentation

A full project presentation (objectives, design rationale, and walkthrough) is included:
- `Library_System.pptx`

## Author

**Aseel Alanzi**  
Department of Computer Science  
University of Hail  
[GitHub](https://github.com/Aaseel11) • [LinkedIn](https://linkedin.com/in/aaseel-alanzi)

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
