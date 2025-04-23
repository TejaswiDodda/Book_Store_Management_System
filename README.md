# Book_Store_Management_System

This is a **Spring Boot** web application built using **MySQL**, **JPA**, and **Thymeleaf**. It allows users to register, view, and manage a list of books.

---

## 🚀 Features

- 📘 Add, update, delete, and view books  
- ❤️ Save books to your personal "My Book List"  
- 🖥️ Simple and responsive UI using Thymeleaf  
- 🛢️ Data persistence using Spring Data JPA and MySQL

---

## 🛠 Tech Stack

- Java 17+  
- Spring Boot  
- Spring MVC  
- Spring Data JPA  
- Thymeleaf  
- MySQL  
- Maven

---

## 📁 Project Structure

```
BookStore/
├── src/
│   ├── main/
│   │   ├── java/com/bookStore/
│   │   │   ├── controller/             # Web controllers
│   │   │   ├── entity/                 # JPA Entities
│   │   │   ├── repository/             # Repositories (DAO layer)
│   │   │   ├── service/                # Service layer
│   │   │   └── BookStoreApplication.java # Main class
│   │   └── resources/
│   │       ├── templates/             # Thymeleaf templates
│   │       ├── static/images/         # Static assets
│   │       └── application.properties # App configuration
│   └── test/
│       └── BookStoreApplicationTests.java
├── pom.xml
```

---

## ⚙️ Configuration

Set your database connection in `src/main/resources/application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/book_store_db
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

---

## ▶️ How to Run

1. **Clone the repo**  
   ```bash
   git clone https://github.com/yourusername/book-store-app.git
   cd book-store-app
   ```

2. **Set up the database**  
   - Create a database named `book_store_db` in MySQL.

3. **Update credentials in `application.properties`**

4. **Run the application**  
   - In your IDE: Run `BookStoreApplication.java`
   - Or via terminal:  
     ```bash
     ./mvnw spring-boot:run
     ```

5. **Visit in browser**  
   ```
   http://localhost:8080/
   ```

---

## 👨‍💻 Endpoints

- `/` → Home Page  
- `/book_register` → Add Book  
- `/available_books` → List of All Books  
- `/my_books` → User's Saved Books  
- `/editBook/{id}` → Edit Book  
- `/deleteBook/{id}` → Delete Book

---


