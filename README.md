# Spring boot, Hibernate, MySQL REST API

A simple Spring boot application that demonstrates the usage of RESTful API using Spring boot, Hibernate and MySQL. 

## Tools and Technologies used

* Java 1.8
* Spring boot 2.1.1
* MySQL
* JPA
* Hibernate
* Maven
* Eclipse Oxygen

## Steps to install

**1. Clone the application**

```bash
git clone https://github.com/scbushan05/spring-boot-hibernate-mysql-rest-api.git
```

**2. Create MySQL database**

```sql
CREATE DATABASE crudapi
```
	
**3. Create table or Run the SQL script file**

```sql
CREATE TABLE tbl_employee
(
	id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    	name VARCHAR(255),
    	gender VARCHAR(255),
    	department VARCHAR(255),
    	dob DATE
)
```
	
**4. Change MySQL Username and Password as per your MySQL Installation**
	
+ open `src/main/resources/application.properties` file.

+ change `spring.datasource.username` and `spring.datasource.password` as per your installation
	
**5. Run the app**

You can run the spring boot app by typing the following command -

```bash
mvn spring-boot:run
```

You can also package the application in the form of a `jar` file and then run it like so -

```bash
mvn package
java -jar target/crudapi-0.0.1-SNAPSHOT.jar
```

The server will start on port 8080.
	
## Explore Rest APIs

The app defines following CRUD APIs.

    GET /api/employee
    
    POST /api/employee
    
    GET /api/employee/{id}
    
    PUT /api/employee
    
    DELETE /api/employee/{id}

You can test them using postman or any other rest client.

postman collection : https://www.getpostman.com/collections/79b34e5606d66d88881e
