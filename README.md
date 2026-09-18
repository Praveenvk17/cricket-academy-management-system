# 🏏 Cricket Academy Management System

The **Cricket Academy Management System** is a Java-based application designed to manage cricket academy activities, including coaches, players, training details, and academy-related records.

## 📌 Project Overview

This system helps cricket academies organize and manage their daily operations digitally. It reduces manual work and makes it easier to maintain academy information in a structured way.

## ✨ Features

* Coach management
* Player management
* Academy record management
* Add, update, view, and delete records
* File upload management
* Data access using DAO classes
* Organized project structure
* Database connectivity
* Easy-to-maintain Java code

## 🛠️ Technologies Used

* **Java**
* **JDBC**
* **SQL Database**
* **Maven**
* **Eclipse IDE**
* **Git and GitHub**

## 📂 Project Structure

```text
cricket-academy-management
│
├── src
│   └── main
│       └── java
│           └── com
│               └── academy
│                   ├── dao
│                   │   ├── CoachDAO.java
│                   │   ├── UploadedFileDAO.java
│                   │   └── ...
│                   │
│                   ├── model
│                   ├── service
│                   ├── controller
│                   └── ...
│
├── pom.xml
└── README.md
```

## ⚙️ Requirements

Before running the project, install the following:

* Java JDK 21 or later
* Eclipse IDE
* Maven
* SQL Database
* Database driver/JDBC connector

## 🚀 How to Run the Project

1. Clone the repository:

```bash
git clone https://github.com/your-username/cricket-academy-management.git
```

2. Open Eclipse IDE.

3. Select:

```text
File → Import → Existing Maven Projects
```

4. Select the project folder.

5. Configure the database connection in the project configuration file.

6. Update the database username, password, and URL.

7. Right-click the project and select:

```text
Run As → Java Application
```

## 🗄️ Database Configuration

Update the database configuration according to your local database setup.

Example:

```java
String url = "jdbc:mysql://localhost:3306/cricket_academy";
String username = "root";
String password = "your_password";
```

> Replace the database URL, username, password, and database name with your actual configuration.

## 🔐 Security Note

Do not upload real database passwords, API keys, or other confidential information to GitHub. Use environment variables or a separate configuration file for sensitive details.

## 🔮 Future Enhancements

* Admin login and authentication
* Player attendance tracking
* Coach scheduling
* Fee payment management
* Training performance reports
* Dashboard with academy statistics
* Email notifications
* Role-based access control

## 👨‍💻 Developer

**PRAVEEN** JAVA FULLSTACK DEVELOPER

Computer Science and Engineering Graduate

## 📄 License

This project is created for educational and learning purposes.
