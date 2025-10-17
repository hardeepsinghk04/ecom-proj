# 🛒 ecom-proj — Spring Boot E-Commerce Backend

This is a simple e-commerce backend application built with **Spring Boot**, using **H2 in-memory database**, **Spring Data JPA**, and **RESTful APIs**. It manages product data and exposes endpoints for CRUD operations.

## 🚀 Features

- REST API for managing products
- In-memory H2 database for quick testing
- Auto schema generation via JPA
- SQL data initialization on startup
- JSON serialization with custom date formatting

## 🧱 Tech Stack

- Java 17+
- Spring Boot
- Spring Data JPA
- H2 Database
- Maven
- Lombok

## 📦 Project Structure

```plaintext
src/
├── main/
│   ├── java/com/Hardeep/ecom_proj1/
│   │   ├── controller/         # REST controllers
│   │   ├── model/              # JPA entities
│   │   ├── repo/               # Spring Data repositories
│   │   ├── service/            # Business logic
│   │   └── EcomProj1Application.java
│   └── resources/
│       ├── application.properties
│       ├── data1.sql           # Sample data
│       ├── static/
│       └── templates/
└── test/
    └── java/com/Hardeep/ecom_proj1/
        └── EcomProj1ApplicationTests.java
```


## 🔧 Configuration

Located in `application.properties`:

```properties
spring.application.name=ecom-proj1
spring.datasource.url=jdbc:h2:mem:hardeep
spring.datasource.username=hardeep
spring.datasource.password=singh
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.defer-datasource-initialization=true
spring.h2.console.enabled=true
spring.h2.console.path=/h2-console
```

## 📮 API Endpoints

| Method | Endpoint              | Description        |
|--------|-----------------------|--------------------|
| GET    | `/api/products`       | Fetch all products |
| POST   | `/api/products`       | Add a new product  |
| PUT    | `/api/products/{id}`  | Update a product   |
| DELETE | `/api/products/{id}`  | Delete a product   |

## 🧪 Testing

Use Postman or curl to interact with the API. Sample GET request:

```bash
curl http://localhost:8080/api/products
```

## 🖥️ H2 Console

Access the H2 database console at:

```text
http://localhost:8080/h2-console
```

## 📄 License

This project is licensed under the MIT License.


---

Let me know if you want to add badges, deployment instructions, or a frontend link. I can also help you set up GitHub Actions or write a `CONTRIBUTING.md` next!
