# FoodDeliveryPro

**FoodDeliveryPro** is a robust and easy-to-use system built to help manage customers, inventory, and orders seamlessly. Designed with security in mind, it includes user authentication and role-based access control to ensure the right people have access to the right features. The application is powered by Spring Boot and Thymeleaf, using MySQL to handle data storage efficiently. Whether you're an admin or a staff member, FoodDeliveryPro offers a smooth and intuitive experience.

---

## Key Features

- **Customer Management**  
  Quickly add, update, or remove customer information to keep your records up to date.

- **Inventory Management**  
  Track your products, monitor stock levels, and adjust pricing easily.

- **Order Handling**  
  Create and manage customer orders, update their status, and keep everything organized.

- **Secure Login System**  
  Protect your data with login authentication for admins and staff.

- **Role-Based Access Control**  
  Assign different permissions to users based on their roles to maintain security.

- **Dynamic UI with Thymeleaf**  
  Enjoy a responsive and user-friendly interface powered by Thymeleaf templates.

- **Database Integration**  
  Reliably store and manage your data using MySQL.

---

## Technology Overview

- **Backend:** Spring Boot, Java 8, Spring MVC, Spring Data JPA (Hibernate)  
- **Frontend:** Thymeleaf, HTML, CSS, JavaScript  
- **Database:** MySQL  
- **Development Environment:** Eclipse or Spring Tool Suite (STS)

---

## Prerequisites

Before running FoodDeliveryPro, make sure you have the following installed on your system:

- Java 8  
- MySQL Server  
- Maven  
- Eclipse IDE or Spring Tool Suite (STS)

---

## Installation and Setup

1. **Clone the repository:**

    ```bash
    git clone https://github.com/Shashank-1K/FoodDeliveryPro.git
    ```

2. **Enter the project directory:**

    ```bash
    cd FoodDeliveryPro
    ```

3. **Set up your MySQL database:**

    - Create a new database in MySQL (for example, `fooddeliverypro`).
    - Open `src/main/resources/application.properties` and update the database connection details:

    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/fooddeliverypro
    spring.datasource.username=your_mysql_username
    spring.datasource.password=your_mysql_password
    spring.jpa.hibernate.ddl-auto=update
    ```

4. **Build and run the project:**

    ```bash
    mvn spring-boot:run
    ```

5. **Access the application:**  
   Open your browser and visit: `http://localhost:8080`

---

## Preview

Here are some screenshots showcasing the FoodDeliveryPro interface and its features:

![Screenshot 1](https://github.com/user-attachments/assets/3e34f54c-c986-42ac-96a4-ed7ad18035a6)  
![Screenshot 2](https://github.com/user-attachments/assets/a4046d4e-8c3d-4629-8913-5543d709e80e)  
![Screenshot 3](https://github.com/user-attachments/assets/09c92348-ec06-4607-9ae4-88b28cc1e0ec)

*(Add or update screenshots as needed)*

---

## Project Structure

```plaintext
src/
├── main/
│   ├── java/
│   │   └── com.example.fooddeliverypro/
│   │       ├── controller/      # Handles web requests and responses
│   │       ├── model/           # Defines entity classes for database tables
│   │       ├── repository/      # Interfaces for data access
│   │       └── service/         # Contains business logic
│   ├── resources/
│   │   ├── templates/           # Thymeleaf HTML templates
│   │   ├── static/              # CSS, JavaScript, and images
│   │   └── application.properties  # Configuration settings
│   └── webapp/
│       └── WEB-INF/
│           └── views/           # Additional JSP or view files (if any)
└── test/                        # Unit and integration tests
