#
# Spring Boot Rest Api

This project contains the api for thefoodu

## Table of Contents

1. [Tools](https://github.com/ealili/springboot-rest-api/tree/develop#tools)
2. [Dependencies](https://github.com/ealili/springboot-rest-api/tree/develop#dependencies)
3. [Getting Started](https://github.com/ealili/springboot-rest-api/tree/develop#getting-started)
4. [Database](https://github.com/ealili/springboot-rest-api/tree/develop#database)
5. [REST Endpoints](https://github.com/ealili/springboot-rest-api/tree/develop#rest-endpoints)

## Tools
You will need:

* [Maven](https://maven.apache.org/) as your build tool
* Your favorite IDE
* JDK 1.8+
* [PostgreSQL](https://www.postgresql.org/)

## Table of Contents

1. [Tools](#tools)
1. [Dependencies](#dependencies)
1. [Getting Started](#getting-started)
1. [Database](#database)
1. [REST Endpoints](#rest-endpoints)

## Dependencies

You will need:

- [Spring Data JPA](https://mvnrepository.com/artifact/org.springframework.boot/spring-boot-starter-data-jpa)
- [PostgreSQL Connector](https://mvnrepository.com/artifact/mysql/mysql-connector-java)
- [Spring WEB](https://mvnrepository.com/artifact/org.springframework/spring-web)
- [JUnit](https://mvnrepository.com/artifact/junit/junit)
- [JUnit Vintage Engine](https://mvnrepository.com/artifact/org.junit.vintage/junit-vintage-engine)
- [Spring Boot Test Starter](https://mvnrepository.com/artifact/org.springframework.boot/spring-boot-starter-test)
- [Spring Boot Maven Plugin](https://mvnrepository.com/artifact/org.springframework.boot/spring-boot-maven-plugin)

## Getting Started

First, clone the project:

$ https://github.com/Lenarty/java.git

Second, open the project using your favorite IDE and install all the listed dependencies above and you should be able to run the application.

If everything works, you should see an Index Page [here](http://127.0.0.1:8080/).

## Database

1. Create a PostgreSQL database using the thefoodu.sql script provided in the root folder.
2. Add credentials to /src/main/resources/application.properties

The default ones are:

```

spring.datasource.driverClassName=org.postgresql.Driver

spring.datasource.url=jdbc:postgresql://localhost:5432/thefoodu

spring.datasource.username=postgres

spring.jpa.database-platform=org.hibernate.dialect.PostgreSQLDialect

spring.jpa.show-sql=true

```

#

## REST Endpoints

### Company Endpoints

Get all companies

- URL (localhost:8080/companies), METHOD = GET

Save a company

- URL (localhost:8080/company), METHOD = POST, expects JSON body (only company\_name is required)

Find company by id

- URL (localhost:8080/company/{id}), METHOD = GET

Delete a company

- URL (localhost:8080/company/{id}), METHOD = DELETE