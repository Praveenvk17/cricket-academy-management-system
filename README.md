# 🏏 Cricket Academy Management System

The **Cricket Academy Management System** is a Java-based web application designed to manage cricket academy activities, including coaches, players, batches, training details, performance evaluations, documents, and academy-related records.

## 📌 Project Overview

This system helps cricket academies organize and manage their daily operations digitally. It reduces manual work and makes it easier to maintain player, coach, batch, and performance information in a structured way.

## ✨ Features

### 👨‍💼 Admin
- Admin login and authentication
- Coach management
- Player management
- Member directory
- Search and filter players
- Create and manage batches
- Assign players to batches
- Maximum 15 members per batch
- Prevent duplicate player assignments
- View academy records

### 🧑‍🏫 Coach
- Coach login
- View assigned players
- View player details
- Evaluate player performance
- Record runs scored
- Record balls faced
- Record wickets taken
- Record overs bowled
- Record runs conceded
- Give fitness ratings
- Add coach feedback

### 🏏 Player
- Player login
- View player profile
- View assigned batch
- View coach details
- View batch timing
- View skill level
- View monthly fee
- View batch member count
- Upload documents
- Download uploaded documents
- View performance and match evaluations
- View coach feedback

## 🛠️ Technologies Used

- **Java**
- **JSP**
- **Servlets**
- **JDBC**
- **MySQL**
- **HTML**
- **CSS**
- **Bootstrap**
- **Apache Tomcat**
- **Maven**
- **Eclipse IDE**
- **Git and GitHub**

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
│                   │   ├── BatchDAO.java
│                   │   ├── EnrollmentDAO.java
│                   │   ├── PerformanceDAO.java
│                   │   ├── UploadedFileDAO.java
│                   │   ├── UserDAO.java
│                   │   └── ...
│                   │
│                   ├── model
│                   │   ├── Batch.java
│                   │   ├── Performance.java
│                   │   ├── UploadedFile.java
│                   │   ├── User.java
│                   │   └── ...
│                   │
│                   ├── servlet
│                   │   ├── AssignPlayerServlet.java
│                   │   ├── BatchServlet.java
│                   │   └── ...
│                   │
│                   └── util
│                       └── DBConnection.java
│
├── WebContent
│   ├── admin-dashboard.jsp
│   ├── coach-dashboard.jsp
│   ├── player-dashboard.jsp
│   ├── login.jsp
│   └── ...
│
├── database
│   └── cricket_academy_db.sql
│
├── pom.xml
└── README.md
## ⚙️ Requirements

Before running the project, install the following:

- Java JDK 21 or later
- Eclipse IDE
- Apache Tomcat
- Maven
- MySQL
- MySQL JDBC Driver / Connector

## 🚀 How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/cricket-academy-management.git

## 2. Open the Project

Open **Eclipse IDE**.

Select:

File → Import → Existing Maven Projects

Select the cloned project folder.

## 3. Configure the Database

Open MySQL and run:

database/cricket_academy_db.sql

Database name:

cricket_academy_db

## 4. Configure Database Connection

Open:

DBConnection.java

Update your MySQL credentials:

```java
String url = "jdbc:mysql://localhost:3306/cricket_academy_db";
String username = "root";
String password = "your_password";

5. Run the Application

Configure Apache Tomcat in Eclipse.

Then:

Right Click Project → Run As → Run on Server

Select Apache Tomcat and start the application.

🗄️ Database

The project uses the following main tables:

users
batches
enrollments
performance_records
uploaded_files
Batch Capacity

Each batch supports a maximum of:

15 Players

The system prevents additional players from being assigned after the batch reaches its maximum capacity.

🔐 Demo Login Credentials
Admin
Email: Rcb@academy.com
Password: rcb2526
Coach
Email: bhuvi@academy.com
Password: coach123
Player
Email: rohit@academy.com
Password: player123

These are demo credentials created for project testing and demonstration purposes.

🔄 System Workflow
ADMIN
  │
  ├── Manage Coaches
  ├── Manage Players
  ├── Create Batches
  └── Assign Players
          │
          ▼
       COACH
          │
          ├── View Assigned Players
          └── Evaluate Performance
                    │
                    ▼
                 PLAYER
                    │
                    ├── View Batch
                    ├── Upload Documents
                    └── View Performance
📊 Performance Evaluation

Coaches can record:

Runs Scored
Balls Faced
Wickets Taken
Overs Bowled
Runs Conceded
Fitness Rating
Coach Feedback

Players can view their performance records from their dashboard.

📄 Document Management

Players can upload:

PDF
JPG
JPEG
PNG

Maximum file size:

10 MB

Players can also download their uploaded documents from the dashboard.

🔒 Role-Based Access
ADMIN
→ Academy Management

COACH
→ Assigned Players & Performance Evaluation

PLAYER
→ Personal Batch, Documents & Performance
🔮 Future Enhancements
Player attendance tracking
Coach scheduling
Fee payment management
Training performance reports
Dashboard with academy statistics
Email notifications
Online fee payment
Advanced player performance analytics
Match scheduling
👨‍💻 Developer

PRAVEEN

Java Full Stack Developer

Computer Science and Engineering Graduate

📄 License

This project is created for educational and learning purposes.
