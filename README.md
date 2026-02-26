# Greeter Service

Minimal Spring Boot 3.x (Java 21) REST service for connectivity testing. Returns a simple greeting when the endpoint is called.

## Run

```bash
mvn spring-boot:run
```

## Endpoint

- **GET** `http://localhost:8080/api/greet`  
  Response: greeting with server date/time (port 8080).

## Build JAR

```bash
mvn clean package
java -jar target/greeter-svc-1.0.0-SNAPSHOT.jar
```

## Docker

Build and run:

```bash
docker build -t greeter-svc .
docker run -p 8080:8080 greeter-svc
```

Then call **GET** `http://localhost:8080/api/greet`. Map a different host port if needed, e.g. `docker run -p 9090:8080 greeter-svc` for host 9090.
