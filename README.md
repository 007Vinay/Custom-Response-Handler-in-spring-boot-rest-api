# Cloud Vendor REST API Project with Custom Handler and Exception Handling

This is a Spring Boot RESTful web service for managing cloud vendors. It includes a custom exception handling mechanism, a standard response structure, and database operations using Spring Data JPA and MySQL. The application was tested using Postman.

----------

## Tech Stack

- Java 17
- Spring Boot 3.3
- Spring Web
- Spring Data JPA
- MySQL
- Maven
- Postman (for API testing)

----------

## 📁 Project Structure

com.thinkconstructive.restdemo
│
├── controller
│ └── CloudVendorController.java
│
├── exception
│ ├── CloudVendorException.java
│ ├── CloudVendorExceptionHandler.java
│ └── CloudVendorNotFoundException.java
│
├── model
│ └── CloudVendor.java
│
├── repository
│ └── CloudVendorRepository.java
│
├── response
│ └── ResponseHandler.java
│
├── service
│ ├── CloudVendorService.java
│ └── impl
│ └── CloudVendorServiceImpl.java
│
└── RestDemoApplication.java

----------


## ⚙️ How to Run the Application

1. Make sure MySQL is running and a database is created (e.g., `cloudvendor_db`).
2. Configure your `application.properties`:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/cloudvendor_db
   spring.datasource.username=root
   spring.datasource.password=your_password
   spring.jpa.hibernate.ddl-auto=update
   
-----------

# API Endpoints

Method	   Endpoint	              Description
GET	     /cloudvendor	            Get all vendors
GET	     /cloudvendor/{id}	      Get vendor by ID
POST	   /cloudvendor	            Create new vendor
PUT	     /cloudvendor/{id}	      Update existing vendor
DELETE	 /cloudvendor/{id}	      Delete vendor


