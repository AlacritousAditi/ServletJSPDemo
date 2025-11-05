# ServletJSPDemo
3.1(java)
# ServletJSPDemo1

A simple *Java web application* built using *Servlets, **JSP, and **MySQL, deployed on **Apache Tomcat*.  
It demonstrates user authentication, employee management, and attendance tracking features.

---

##  Features
- User login with credential validation (from database)
- Employee listing and search by ID
- Attendance submission form (name, date, status)
- JSP-based front-end and servlet-based back-end
- MySQL integration using JDBC

---

##  Technologies Used
- Java 17
- Jakarta Servlet 6.0
- JSP 3.0
- MySQL 8+
- Apache Tomcat 10
- Maven (for dependency management)

---

##  Setup Instructions

###  Database Setup
Create a database named **servlet_demo** in MySQL:
```sql
CREATE DATABASE servlet_demo;
USE servlet_demo;

CREATE TABLE users (
  id INT AUTO_INCREMENT PRIMARY KEY,
  username VARCHAR(50),
  password VARCHAR(50)
);

CREATE TABLE employees (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100),
  department VARCHAR(100)
);

CREATE TABLE attendance (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100),
  date DATE,
  status VARCHAR(20)
);
