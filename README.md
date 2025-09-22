# SQL-Internship

# SQL-Internship
**Overview**
This project demonstrates the database design of a Library Management System using Entity-Relationship (ER) modeling. The system manages library members, books, loans, and fines efficiently with proper relationships and constraints.

 **Entities and Attributes**
**1. Members**
member_id (Primary Key)
member_name
member_email
member_contactno

**2. Books**
book_id (Primary Key)
book_author
book_title
published_year

**3. Loans**
loan_id (Primary Key)
loan_date
return_date
member_id (Foreign Key → Members)
book_id (Foreign Key → Books)

**4. Fine**
fine_id (Primary Key)
loan_id (Foreign Key → Loans)
fine_amount
status

**Relationships**
A Member can borrow many Books (via Loans).
A Book can be borrowed multiple times.
A Loan may generate a Fine if the book is returned late

**Database Link**

http://localhost/phpmyadmin/index.php?route=/database/structure&db=librarymanagement
