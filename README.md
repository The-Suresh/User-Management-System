# User Management System

## Description
The **User Management System** is a desktop application built using **Java Swing**. It allows administrators to manage users by performing operations such as adding, updating, deleting, and viewing user information.

## Features
- Add new users
- Edit existing user details
- Delete users from the system
- View a list of all users
- Search for users by name or ID
- Basic authentication for administrator access
- Data persistence using **MySQL

## Technologies Used
- **Java Swing** (GUI)
- **JDBC** (Database Connectivity)
- **MySQL / SQLite** (Database)

## Installation
### Prerequisites:
- Install **Java JDK (11 or above)**
- Install **MySQL / SQLite** (if using a database)
- Configure your database with the required schema

### Steps:
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/user-management-system.git
   ```
2. Navigate to the project directory:
   ```sh
   cd user-management-system
   ```
3. Compile and run the application:
   ```sh
   javac -cp .:lib/mysql-connector-java.jar Main.java
   java -cp .:lib/mysql-connector-java.jar Main
   ```
   *(Modify classpath accordingly for Windows using `;` instead of `:`)*

## Database Schema (MySQL Example)
```sql
CREATE DATABASE IF NOT EXISTS dbjoes;
USE dbjoes;
 
DROP TABLE IF EXISTS users;
CREATE TABLE users (
  ID int(11) NOT NULL AUTO_INCREMENT,
  NAME varchar(50) DEFAULT NULL,
  AGE int(11) DEFAULT NULL,
  CITY varchar(50) DEFAULT NULL,
  PRIMARY KEY (ID)
) ENGINE=InnoDB AUTO_INCREMENT=4;
 
 
INSERT INTO users (ID,NAME,AGE,CITY) VALUES 
 (1,'Ram Kumar',25,'Salem'),
 (2,'Sam Kumar',25,'Salem'),
 (3,'Rakesh',25,'Salem');
```

## Usage
1. Launch the application.
2. Log in with administrator credentials.
3. Use the interface to add, edit, delete, or search for users.


## License
This project is licensed under the **MIT License**.

## Author
**Sudalai Suresh** - [GitHub Profile](https://github.com/The-Suresh)

