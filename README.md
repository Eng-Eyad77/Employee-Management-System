
# 🧑‍💼 Employee Management System

This is a simple **Spring Boot** application designed to manage employee records. It provides basic CRUD operations (Create, Read, Update, Delete) through RESTful APIs and uses an in-memory **H2 database** for data storage.

## 🚀 Features

- Add new employees
- View all employees
- Update employee details
- Delete employees
- H2 console for database inspection

## 🛠️ Tech Stack

- **Backend:** Java 21, Spring Boot 3.4.1
- **Database:** H2 (in-memory)
- **Build Tool:** Maven

## 🗂️ Project Structure

```
employeemanagement/
├── controller/       # REST API endpoints
├── model/            # Employee entity
├── repository/       # Spring Data JPA interface
├── resources/
│   ├── application.properties
└── EmployeemanagementApplication.java
```

## ⚙️ Configuration

The app uses an H2 in-memory database. You can access the H2 console at:

```
http://localhost:8080/h2
```

Use the following settings to log in:
- **JDBC URL:** `jdbc:h2:mem:testdb2`
- **User:** `sa`
- **Password:** *(leave blank)*

## ▶️ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/employeemanagement.git
   cd employeemanagement
   ```

2. Run the application using Maven:
   ```bash
   ./mvnw spring-boot:run
   ```

3. Open your browser and go to:
   ```
   http://localhost:8080
   ```

## 📬 API Endpoints

| Method | Endpoint           | Description         |
|--------|--------------------|---------------------|
| GET    | `/employees`       | Get all employees   |
| POST   | `/employees`       | Add new employee    |
| PUT    | `/employees/{id}`  | Update employee     |
| DELETE | `/employees/{id}`  | Delete employee     |

## 📄 License

This project is for educational/demo purposes.

---
*Developed by Eyad Maccawy using Spring Boot.*


