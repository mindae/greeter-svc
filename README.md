# Greeter Service

Minimal Spring Boot 3.x (Java 21) REST service for connectivity testing. Returns a simple greeting when the endpoint is called.

## Run

```bash
mvn spring-boot:run
```

## Endpoint

- **GET** `http://localhost:8080/api/greet`  
  Response: `Hello, Your company name here!`

## Build JAR

```bash
mvn clean package
java -jar target/greeter-svc-1.0.0-SNAPSHOT.jar
```
