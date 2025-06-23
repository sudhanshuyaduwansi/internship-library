# Library Management Database - SQL Internship Task

## 🧾 Description:
This project demonstrates a basic *Library Management System* schema using SQLite. It includes 3 main tables:

- Students
- Books
- IssueRecords

## 🛠 Tools Used:
- SQLiteStudio 3.4.1

## 📁 Tables:

### 1. Students
| Column       | Type    | Description             |
|--------------|---------|-------------------------|
| student_id   | INTEGER | Primary Key, Auto ID    |
| name         | TEXT    | Student full name       |
| email        | TEXT    | Unique student email    |
| course       | TEXT    | Enrolled course         |
| year         | INTEGER | Academic year           |

### 2. Books
| Column       | Type    | Description             |
|--------------|---------|-------------------------|
| book_id      | INTEGER | Primary Key, Auto ID    |
| title        | TEXT    | Book title              |
| author       | TEXT    | Author name             |
| publisher    | TEXT    | Publisher               |
| category     | TEXT    | Genre                   |
| isbn         | TEXT    | Unique ISBN             |
| quantity     | INTEGER | Available copies        |

### 3. IssueRecords
| Column       | Type    | Description                      |
|--------------|---------|----------------------------------|
| issue_id     | INTEGER | Primary Key, Auto ID             |
| student_id   | INTEGER | Foreign Key (Students)           |
| book_id      | INTEGER | Foreign Key (Books)              |
| issue_date   | TEXT    | Date of issue                    |
| return_date  | TEXT    | Date of return                   |

## 🔗 Relationships:
- IssueRecords.student_id → Students.student_id
- IssueRecords.book_id → Books.book_id

---

## 🔚 How to Run:
1. Open SQLiteStudio
2. Connect to LibraryDB.sqlite
3. Paste schema.sql in SQL editor and run
4. Tables will be created!

---