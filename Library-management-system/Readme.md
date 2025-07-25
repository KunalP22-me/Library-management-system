### 🚀 CANTILEVER: Java Programming Internship

### 📚 Library Management System

A desktop-based Library Management System built using **Java Swing** and **MySQL**, designed to manage books, students, and lending operations. It features a modern UI, admin controls, statistics tracking, and database connectivity using JDBC.

---

### 🚀 Features

* ✅ **Login / Registration** with role-based access (Admin / User)
* 📚 Add, search, issue, and return books
* 👤 Manage student accounts and users
* 📊 View usage statistics
* 🛠 Admin panel for user management (promote, delete)
* 🖥 Responsive dashboard layout with icons
* 🔐 Secure DB interaction using **JDBC + MySQL**

---

### 🛠 Technologies Used

* Java 17+
* Swing GUI
* MySQL 8+
* JDBC (mysql-connector-j-9.3.0.jar)

---

### 📁 Project Structure

```
📦 library-management
 ┣ 📂 dao              → Data access layer (UserDAO, BookDAO, etc.)
 ┣ 📂 db               → DB connection class
 ┣ 📂 model            → User & Book model classes
 ┣ 📂 ui               → GUI Panels (LoginScreen, DashboardUI, etc.)
 ┣ 📂 lib              → JDBC JAR (mysql-connector-j-9.3.0.jar)
 ┣ 📄 Main.java        → Application entry point
 ┣ 📄 schema.sql       → MySQL table schema
 ┗ 📄 README.md        → This file
```

---

### 🧑‍💻 How to Run

1. **Start MySQL** and create the DB from `schema.sql`:

   ```sql
   CREATE DATABASE library_db;
   USE library_db;
   -- Then run the table creation script
   ```

2. **Compile:**

   ```bash
   javac -cp ".;lib/mysql-connector-j-9.3.0.jar" -d . (Get-ChildItem -Recurse -Filter *.java | ForEach-Object { $_.FullName })
   ```

3. **Run:**

   ```bash
   java -cp ".;lib/mysql-connector-j-9.3.0.jar" Main
   ```

---
