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


<img width="524" height="300" alt="Screenshot 2024-12-07 at 8 42 56 AM" src="https://github.com/user-attachments/assets/15acb726-3a35-4913-866e-da25343f1791" />
<img width="670" height="475" alt="Screenshot 2024-12-07 at 8 42 24 AM" src="https://github.com/user-attachments/assets/c3294509-a5f0-4c43-ba47-16f3d31df18f" />
<img width="788" height="361" alt="Screenshot 2024-12-07 at 8 36 22 AM" src="https://github.com/user-attachments/assets/ac7394b4-742c-4928-81e2-9d53aba31e23" />
<img width="478" height="375" alt="Screenshot 2024-12-07 at 8 36 06 AM" src="https://github.com/user-attachments/assets/54365878-b48b-46ac-8219-60b3dfa793cb" />
<img width="1237" height="662" alt="Screenshot 2024-12-07 at 8 35 51 AM" src="https://github.com/user-attachments/assets/50ddae9a-c48f-48ff-bfac-4aaa4390624b" />
<img width="909" height="710" alt="Screenshot 2024-12-07 at 8 35 37 AM" src="https://github.com/user-attachments/assets/33594f6a-dfcf-4e81-8127-39fbc2138ab1" />


