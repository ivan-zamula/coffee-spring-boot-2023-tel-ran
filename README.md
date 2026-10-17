# Coffee catalogue (Tel-Ran, 2023)

[English](README.md) | [Русский](README.ru.md)

A Java course project for managing a coffee catalogue with Spring Boot. It combines server-rendered pages, form validation and database access.

## Features and stack

- List, add, edit, delete and search coffee entries.
- Render pages with Thymeleaf and validate submitted forms.
- Store entries through Spring Data JPA in an in-memory H2 database.
- Load a small set of sample coffees on startup.

The project uses Java 17 and Spring Boot 3.0.2. Controllers, entities and repositories are in [src/main/java/com/example/coffee](src/main/java/com/example/coffee); page templates are in [src/main/resources/templates](src/main/resources/templates).

## Run locally

Install JDK 17 and Maven, and make `java` and `mvn` available in your terminal.

```bash
git clone https://github.com/ivan-zamula/coffee-spring-boot-2023-tel-ran.git
cd coffee-spring-boot-2023-tel-ran
```

```bash
mvn spring-boot:run
```

Open [the catalogue](http://localhost:8080/coffees) in a browser. The H2 database lives in memory, so changes last for the current application session. Connection settings are in [application.properties](src/main/resources/application.properties).
