# SOFTWARE REQUIREMENTS SPECIFICATION

# LIBRARY MANAGEMENT APP

## 1. Introduction

### 1.1 Purpose

The purpose of the Library Management App is to automate and simplify library activities. The application allows students to search, borrow and return books. It also helps librarians manage books, students and borrowing records.

### 1.2 Scope

The Library Management App is a software application used to manage library operations digitally.

The system provides the following features:

- Student registration and login
- Book search
- Checking book availability
- Borrowing books
- Returning books
- Viewing borrowing history
- Adding and managing books
- Managing student records
- Tracking overdue books

### 1.3 Intended Users

The main users of the system are:

1. Students
2. Librarians
3. Administrators

---

## 2. Overall Description

### 2.1 Product Perspective

The Library Management App replaces manual library record management with a computerized system. It stores book, student and borrowing information and provides quick access to the required information.

### 2.2 Product Functions

The main functions of the system are:

- User registration
- User login
- Book search
- Book availability checking
- Book borrowing
- Book return
- Borrowing history
- Book management
- Student management
- Overdue book tracking

### 2.3 User Classes

| User | Responsibilities |
|---|---|
| Student | Search, borrow and return books |
| Librarian | Manage books and borrowing records |
| Administrator | Manage users and monitor the system |

### 2.4 Operating Environment

The application can run on:

- Windows or Linux
- Google Chrome
- Microsoft Edge
- Mozilla Firefox
- Web server
- Database server

---

## 3. Functional Requirements

### FR1 - User Registration

The system shall allow students to create an account by entering their required details.

### FR2 - User Login

The system shall allow registered users to log in using their username or email and password.

### FR3 - Book Search

The system shall allow students to search for books using:

- Book title
- Author
- Category
- ISBN

### FR4 - Book Availability

The system shall display whether a book is available or currently borrowed.

### FR5 - Borrow Book

The system shall allow students to borrow an available book.

### FR6 - Return Book

The system shall allow students to return a borrowed book.

### FR7 - Borrowing History

The system shall allow students to view their current and previous borrowing records.

### FR8 - Add Book

The librarian shall be able to add new books to the library.

### FR9 - Update Book

The librarian shall be able to update book information.

### FR10 - Delete Book

The librarian shall be able to remove books from the system.

### FR11 - Manage Users

The administrator shall be able to manage student and librarian accounts.

### FR12 - Overdue Tracking

The system shall identify books that are not returned before the due date.

### FR13 - Reports

The system shall provide basic reports such as:

- Available books
- Borrowed books
- Overdue books
- Borrowing history

---

## 4. Non-Functional Requirements

### 4.1 Performance

- The system should respond quickly to user requests.
- Book searches should provide results within a few seconds.
- The system should support multiple users.

### 4.2 Security

- User passwords must be protected.
- Only authorized users should access administrative features.
- Users should not be allowed to modify unauthorized information.

### 4.3 Usability

- The application should have a simple and user-friendly interface.
- Navigation should be easy to understand.
- Error messages should be clear.

### 4.4 Reliability

- The system should maintain accurate records.
- Data should not be lost during normal operation.
- The application should handle errors properly.

### 4.5 Availability

- The application should be available during library working hours.
- The system should recover properly after failures.

### 4.6 Maintainability

- The application should be easy to maintain and update.
- The software should be divided into manageable modules.

### 4.7 Scalability

The system should support an increasing number of students, books and borrowing transactions.

---

## 5. External Interface Requirements

### 5.1 User Interface

The application should contain:

- Login page
- Registration page
- Home page
- Book search page
- Book details page
- Borrow and return page
- User profile
- Librarian dashboard
- Administrator dashboard

### 5.2 Hardware Interface

The system requires:

- Computer or laptop
- Keyboard and mouse
- Internet connection

### 5.3 Software Interface

The application may use:

- HTML
- CSS
- JavaScript
- Python
- MySQL
- Web browser

---

## 6. Database Requirements

The system should maintain information about students, books and borrowing transactions.

### 6.1 Student Table

| Field | Description |
|---|---|
| Student ID | Unique student identification |
| Name | Student name |
| Email | Student email |
| Password | Login password |
| Phone | Student contact number |

### 6.2 Book Table

| Field | Description |
|---|---|
| Book ID | Unique book identification |
| Title | Book title |
| Author | Author name |
| Category | Book category |
| ISBN | Book ISBN |
| Status | Available or Borrowed |

### 6.3 Borrowing Table

| Field | Description |
|---|---|
| Transaction ID | Unique transaction identification |
| Student ID | Student who borrowed the book |
| Book ID | Borrowed book |
| Issue Date | Date the book was borrowed |
| Due Date | Expected return date |
| Return Date | Actual return date |
| Status | Borrowed, Returned or Overdue |

---

## 7. System Constraints

1. Users must have a valid account to access protected features.
2. Only librarians can manage book records.
3. Only administrators can manage user accounts.
4. Students can borrow only available books.
5. The system requires a database to store information.
6. Internet access may be required for the web-based application.

---

## 8. Use Case Summary

| Actor | Use Case |
|---|---|
| Student | Register |
| Student | Login |
| Student | Search Book |
| Student | Check Book Availability |
| Student | Borrow Book |
| Student | Return Book |
| Student | View Borrowing History |
| Librarian | Add Book |
| Librarian | Update Book |
| Librarian | Delete Book |
| Librarian | Manage Transactions |
| Administrator | Manage Users |
| Administrator | View Reports |

---

## 9. Assumptions

- Every student has a unique student ID.
- Every book has a unique book ID.
- Users have valid login credentials.
- The library maintains correct book information.
- The application has access to a database.
- Librarians are responsible for maintaining book records.

---

## 10. Future Enhancements

The following features can be added in future versions:

- Online book reservation
- Email notifications
- Automatic fine calculation
- QR code or barcode scanning
- Digital book support
- Online fine payment
- Mobile application
- Advanced reports

---

## 11. Conclusion

The Library Management App provides an efficient way to manage library activities digitally. It reduces manual work, improves book tracking and provides quick access to library information. The system helps students, librarians and administrators manage library operations effectively.