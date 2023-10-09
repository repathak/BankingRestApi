# Banking Portal Rest API Using Spring Boot & Spring Security


The Banking Portal API provides a set of endpoints for managing user accounts, fund transfers, and transactions. This project aims to facilitate secure and efficient banking operations for users.

## Features

- User Registration: Users can register by providing their details, such as name, email, address, and phone number.
- PIN Management: Users can create and update their PINs for added security.
- Cash Deposit and Withdrawal: Users can deposit and withdraw cash from their accounts.
- Fund Transfer: Users can transfer funds to other accounts within the system.
- Transaction History: Users can view their transaction history.

## Technologies Used

- Java Spring Boot Framework
- Spring Security for authentication
- JWT (JSON Web Token) for secure API authentication
- MySQL for data storage
- Hibernate for object-relational mapping
- Maven for project management
- Postman for API testing

## TODO
- UI Fix for Dashboard Charts
- Pagination in table
- Save JWT Token in db and remove on logout
- Email trigger on account login
- Send Bank Statement on Email
  
## Installation and Setup

1. Clone the repository: `git clone https://github.com/yourusername/banking-portal-api.git`
2. Navigate to the project folder: `cd banking-portal-api`
3. Configure MySQL: Set up a MySQL database and update the database credentials in `application.properties`.
4. Build and run the project: `mvn spring-boot:run`

## Screenshots
<img width="960" alt="Screenshot 2023-07-23 200531" src="https://github.com/abhi9720/BankingPortal-API/assets/68281476/1c3a614b-a87d-4603-9eb8-0a21da6e1ee2">

---

<img width="959" alt="Screenshot 2023-07-23 212415" src="https://github.com/abhi9720/BankingPortal-API/assets/68281476/277e50f5-43b6-403d-b336-3431655dfe8a">

---

<img width="960" alt="Screenshot 2023-07-23 212110" src="https://github.com/abhi9720/BankingPortal-API/assets/68281476/13e15e7b-a8c5-4ba9-99e3-31bed25d8b3c">

---

<img width="960" alt="Screenshot 2023-07-23 212533" src="https://github.com/abhi9720/BankingPortal-API/assets/68281476/e8e15160-5bcb-4574-88df-9e300ae5bc59">

---

<img width="960" alt="Screenshot 2023-07-23 200346" src="https://github.com/abhi9720/BankingPortal-API/assets/68281476/29b8d193-4298-48ab-9e0d-110e66b186de">

---

<img width="960" alt="Screenshot 2023-07-23 212118" src="https://github.com/abhi9720/BankingPortal-API/assets/68281476/2654311c-7af9-4425-adea-36ab709d9c48">



## sample Application.properties file
```
server.port=8180
spring.datasource.url=jdbc:mysql://localhost:3306/bankingapp
spring.datasource.username=root
spring.datasource.password=root
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.jpa.database-platform = org.hibernate.dialect.MySQL5Dialect
spring.jpa.generate-ddl=true
spring.jpa.show-sql=true
spring.jpa.hibernate.ddl-auto = update
spring.main.allow-circular-references=true
server.error.include-message=always
# JWT Configuration
jwt.secret=your-secret-key
jwt.expiration=86400000 # Token expiration time in milliseconds (e.g., 24 hours)
jwt.header=Authorization
jwt.prefix=Bearer
```

spring.mail.host=smtp.gmail.com
spring.mail.port=587
spring.mail.username=example@gmail.com
spring.mail.password=x88p99qxzmdvgmdu
spring.mail.properties.mail.smtp.auth=true
spring.mail.properties.mail.smtp.starttls.enable=true 
