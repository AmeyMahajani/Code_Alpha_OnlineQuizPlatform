# Code_Alpha_OnlineQuizPlatform

# Online Quiz Platform

## Overview
The **Online Quiz Platform** is a Java-based console application that allows users to participate in a multiple-choice quiz. It provides a dynamic interface for answering questions and stores the results in a MySQL database, making it an excellent tool for learning and evaluating Java programming and database integration skills.

---

## Features
- **Dynamic Quiz System**:
  - Presents 10 multiple-choice questions to the user.
  - Validates user input in real-time to ensure valid answers.

- **Result Calculation**:
  - Tracks user responses and calculates the total score.
  - Provides immediate feedback after quiz completion.

- **Database Integration**:
  - Stores user names and scores in a MySQL database for persistent record-keeping.

- **Interactive Experience**:
  - Offers a user-friendly interface with clear instructions and error handling.

---

## How It Works
1. **Quiz Execution**:
   - The user is presented with a series of multiple-choice questions.
   - Answers are validated to ensure correctness before proceeding to the next question.

2. **Result Management**:
   - The system calculates the user’s score based on their answers.
   - Results are displayed at the end of the quiz.

3. **Database Storage**:
   - User names and scores are stored in a MySQL database for future reference.

---

## Prerequisites
1. **Java**: Ensure JDK 8 or higher is installed.
2. **MySQL**: A running MySQL server is required.
3. **JDBC Driver**: MySQL Connector/J must be added to the project.

---

## Database Setup
1. **Create Database**:
   ```sql
   CREATE DATABASE quiz_platform_db;
   ```

2. **Create Table**:
   ```sql
   USE quiz_platform_db;

   CREATE TABLE quiz_results (
       id INT AUTO_INCREMENT PRIMARY KEY,
       student_name VARCHAR(100) NOT NULL,
       score INT NOT NULL
   );
   ```

---

## How to Run
1. Clone the repository from GitHub:
   ```bash
   git clone https://github.com/AmeyMahajani/Code_Alpha_OnlineQuizPlatform.git
   ```
2. Set up the MySQL database using the instructions above.
3. Update database credentials in the code:
   ```java
   static final String JDBC_URL = "jdbc:mysql://localhost:3306/quiz_platform_db?useSSL=false&serverTimezone=UTC";
   static final String JDBC_USER = "YOUR_USERNAME";
   static final String JDBC_PASS = "YOUR_PASSWORD";
   ```
4. Compile and run the Java program:
   ```bash
   javac OnlineQuizPlatform.java
   java OnlineQuizPlatform
   ```

---

## Skills Demonstrated
- **Java Programming**: Implementing console applications with user-friendly interfaces.
- **JDBC Integration**: Managing database connectivity and data persistence.
- **Database Management**: Creating and querying MySQL databases.
- **Problem Solving**: Designing solutions for interactive applications.

---

## Acknowledgments
Special thanks to **CodeAlpha Technology** for providing this opportunity to enhance my programming and database management skills.

