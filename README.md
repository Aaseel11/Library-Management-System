# Library Management System

A relational database system built with Microsoft Access to manage a library's core operations: book registration, borrower records, and borrowing/return transactions — replacing manual, error-prone paper tracking with an accurate, searchable digital system.

> **Note:** This project is a Microsoft Access database (`.accdb`). It requires Microsoft Access (2007 or later) installed to open and run.

## Features

✓ Adjustable book catalog with author, publisher, and category information  
✓ Complete borrower management — store names, phone numbers, emails, and addresses  
✓ Automatic transaction tracking with due dates and return dates  
✓ One-to-Many relational database design for data integrity  
✓ Linked tables connecting books, borrowers, categories, and transactions  
✓ Easy-to-use forms for data entry and editing  
✓ Ready-made queries for fast data retrieval  
✓ Search by category, borrower, or book title  
✓ Overdue transaction alerts  
✓ Track borrowing and return history  

## Database Design

The system is built around 4 linked tables with One-to-Many relationships:

| Table | Fields |
|-------|--------|
| **BOOK** | ID • Title • Author • Publisher • YearPublisher • Category |
| **BORROWER** | ID • FirstName • LastName • PhoneNumber • Email • Address |
| **Borrowing** | ID • BookID • BorrowerID • BorrowerDate • DueDate • ReturnDate |
| **Category** | CategoryID • CategoryName • Description |

### Entity Relationship Diagram

The **Borrowing** table acts as a junction table connecting **BOOK** and **BORROWER**, while **BOOK** references **Category** for flexible categorization.

## Data Entry Forms

- **Book Form** — Add and edit book records with all metadata
- **Borrowing Form** — Log borrowing and return transactions
- **Category Form** — Manage and expand book categories
- **Borrower Form** — Register and update borrower information

## Tools and Technologies

- **Microsoft Access 2016** — Database design, forms, queries
- **Relational Database Concepts** — Primary/Foreign Keys, One-to-Many relationships
- **SQL Queries** — Data retrieval and reporting

## How to Use

1. Open the `.accdb` file in Microsoft Access (2007 or later)
2. Navigate to the Forms tab to access data entry interfaces
3. Add books, borrowers, and categories using their respective forms
4. Log borrowing transactions with due dates
5. Record return dates when books are returned
6. Run queries to retrieve specific information (overdue books, books by category, etc.)
7. Generate reports for library management

## Project Documentation

A full project presentation (objectives, design rationale, and walkthrough) is included:
- `Library_System.pptx`

## Author

**Aseel Alanzi**

Department of Computer Science · University of Hail

[GitHub](https://github.com/Aaseel11) • [LinkedIn](https://www.linkedin.com/in/aseel-alanazi410)

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
