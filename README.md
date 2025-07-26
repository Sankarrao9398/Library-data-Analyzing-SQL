# Library-data-Analyzing-SQL
Project Title
Digital Library Management System Using SQLite and Pandas

🎯 Aim
The goal of this project is to create a Library Database using SQLite and perform basic and advanced SQL queries to extract meaningful insights, such as:
Listing books
Filtering by authors
Ranking and rating books
Analyzing borrow history
🗃️ Database Schema
Three tables are created:
Authors
id: Unique identifier (Primary Key)
name: Author’s name
Books
id: Unique identifier (Primary Key)
title: Book title
author_id: Foreign key referencing Authors.id
year: Year of publication
rating: Rating of the book (float)
Borrowers
id: Unique identifier (Primary Key)
book_id: Foreign key referencing Books.id
borrowers_name: Name of the person borrowing
borrow_date: Date of borrowing
🧱 Data Inserted
Authors: J.K. Rowling, George R.R. Martin, J.R.R. Tolkien
Books: Multiple Harry Potter books, Game of Thrones, The Silmarillion
Borrowers: Six borrow entries with different names and dates

🔍 Basic SQL Queries
List All Books
Retrieves all book records from the database.
Books by J.K. Rowling
Filters books where author_id = 1.
Books with Author Names
Uses JOIN to display each book along with its author's name.
Number of Books Per Author
Uses GROUP BY and COUNT() to show how many books each author has written. The top author is returned using ORDER BY and LIMIT.

📈 Advanced SQL Queries
Books by J.R.R. Tolkien
Subquery to find all books written by Tolkien.
Ranking Books by Author by Year
Uses RANK() window function to order books per author chronologically.

Top 3 Highest Rated Books
Uses a CTE (WITH) to fetch the top 3 books sorted by rating.

🧪 SQL Assignments
Top 3 Most Borrowed Books
Subquery with JOIN, GROUP BY, and COUNT() to find most borrowed titles.

Rank Books by Author Based on Rating
Uses RANK() window function to rank books by author and descending rating.

Recent Borrowers (Last 6 Months)
Uses Python datetime to calculate a 6-month window and returns distinct recent borrowers.

Most Borrowed Book by Unique Members
Counts unique borrowers per book and returns the book with the highest count.

💻 Technologies Used
Language: Python 3
Database: SQLite (In-Memory)
Libraries: sqlite3, pandas, datetime

📊 Outputs
DataFrames printed for:
Books list
Filtered and joined queries
Rankings and top-rated books
Most borrowed books and unique borrowers
Borrowers in the last 6 months

📝 Conclusion
This project demonstrates the design and querying of a relational database using SQLite in-memory with real-world use cases such as:
Tracking borrow history
Ranking books and authors
Identifying top-performing books
It serves as a solid base for building a library management system or enhancing SQL query skills.

🚀 Future Enhancements
Add user interface (CLI or GUI)
Add return dates, overdue fines, etc.
Expand dataset for real-world testing
Integrate with a Flask web app or Streamlit dashboard

👨‍💻 Author
Developed by: [Your Name]
Purpose: Educational / Learning Project

