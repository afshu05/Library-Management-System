📚 Library Management System

A beginner-friendly console-based application developed using Python and SQLite to manage library operations such as book management, member handling, and borrow/return processes.

The Library Management System helps automate basic library tasks and supports both Admin and User roles. It allows managing books (add, update, delete, view), user registration and login, borrowing and returning of books with fine calculation, and maintaining borrowing records. The project uses Python for application logic, SQLite for database management, and Tabulate for displaying data in a clean tabular format.

⚙️ How to Run the Project

1️⃣ Install Python  
Download and install Python from: https://www.python.org/downloads/

2️⃣ Install Required Library  
Open terminal or command prompt and run:
pip install tabulate

3️⃣ Open the Project Folder  
Navigate to the folder containing the project files.

4️⃣ Run the Program  
python Library_Management_System.py

🔐 Admin Login Setup

Initially, the database will be empty. To access Admin functionality, an admin record must be inserted manually using the following SQL query:

INSERT INTO Members(member_name, username, password, contact, email, role, join_date)
VALUES('Admin', 'admin', 'admin123', '9999999999', 'admin@gmail.com', 'admin', '2025-01-01');

This query can be executed using DB Browser for SQLite, SQLite command line, or a Python database cursor.

👤 User Features

✔ Register and login  
✔ View all available books  
✔ Search books by title, author, or genre  
✔ Borrow books  
✔ Return books with fine calculation  
✔ View borrowed books  
✔ View and update user profile  

👑 Admin Features

✔ Add new books  
✔ Update book details  
✔ Delete books (only if not currently borrowed)  
✔ View all books  
✔ View all registered members  
✔ View borrowed book records  
✔ Track members who have borrowed specific books and not returned them  

📦 Database Tables

The application uses the following database tables: Author, Genre, Books, Members, and Borrow. Foreign key constraints are implemented to maintain relationships between authors, genres, books, members, and borrowing details.

🧪 Validations Implemented ✔ Name: alphabets only ✔ Username: must be unique ✔ Contact number: 10 digits (Regex) ✔ Email format validation ✔ Borrow quantity based on availability ✔ Prevent deleting books that are borrowed i want this is same only anpother version
