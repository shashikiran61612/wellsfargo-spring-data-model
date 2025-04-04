# Wells Fargo Investment Management System – Data Model Implementation

This project is part of the Wells Fargo Certificate Software Program. It represents the backend data model for a portfolio management system used by financial advisors to manage client investments efficiently.

## 💼 Project Description

The backend system is built using **Java Spring Boot** and **JPA (Java Persistence API)** to model relationships between advisors, clients, portfolios, and securities. These entities are persisted to a relational database using object-relational mapping.

## 📦 Technologies Used

- Java 17+
- Spring Boot
- Spring Data JPA
- Maven (or Gradle)
- H2 / MySQL (any relational DB)
- IntelliJ IDEA
- Git & GitHub

## 🧱 Entity Overview

- **Advisor**: Manages multiple clients
- **Client**: Has one or more portfolios
- **Portfolio**: Belongs to one client and holds multiple securities
- **Security**: Represents a stock/bond/asset within a portfolio

## 📁 Folder Structure

```
src/
└── main/
    └── java/
        └── com/
            └── yourcompany/
                └── project/
                    └── entities/
                        ├── Advisor.java
                        ├── Client.java
                        ├── Portfolio.java
                        └── Security.java
```

## 🚀 How to Run the Project

1. Open the project in IntelliJ IDEA
2. Ensure your database config is set in `application.properties`
3. Run the Spring Boot application
4. (Optional) Add a `CommandLineRunner` to insert sample data for testing

## ✅ Requirements Met

- ✅ Used `@Entity`, `@Id`, `@GeneratedValue` annotations
- ✅ Set up relationships: `@OneToMany`, `@ManyToOne`
- ✅ Added constructors, getters, and setters for all fields
- ✅ No setter for `id` fields
- ✅ Followed Spring Boot and JPA standards

## 📌 Notes

This project fulfills Task 2 of the Wells Fargo program: “Implement the data model using Spring + JPA.” All entities reflect the data model approved in Task 1 (ERD).

---

## 🔗 Author

- Developer: [Your Name]
- LinkedIn: [Add your LinkedIn]
- GitHub: [github.com/yourusername]